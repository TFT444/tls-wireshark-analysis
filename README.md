# SSL/TLS Traffic Analysis using Wireshark

## 📌 Overview
This project demonstrates the analysis of SSL/TLS network traffic using Wireshark. The objective is to understand how secure communication is established through the TLS handshake process.

---

## 🛠️ Tools Used
- Wireshark

---

## 🔑 Key Concepts
- TLS Handshake
- Encryption (Symmetric & Asymmetric)
- Cipher Suites
- Network Packet Analysis

---

## 🔍 Analysis

### 🔹 Client Hello
![Client Hello](client-hello.png)

The Client Hello message represents the first step of the TLS handshake. The client initiates a secure connection by proposing the supported TLS version, a list of cipher suites, and a random value used for key generation. It also includes the Server Name Indication (SNI), which specifies the target domain.

---

### 🔹 Server Hello
![Server Hello](server-hello.png)

The Server Hello message is the server’s response to the Client Hello. It confirms the TLS version and selects a cipher suite from the client’s list. This chosen cipher suite defines the encryption, key exchange, and hashing algorithms used for the secure session.

---

### 🔹 Certificate
![Certificate](certificate.png)

The Certificate message is sent by the server to authenticate its identity. It contains the server’s public key and is issued by a trusted Certificate Authority (CA). This allows the client to verify the server and establish trust.

---

### 🔹 Client Key Exchange
![Client Key Exchange](key-exchange.png)

The Client Key Exchange message is used to establish a shared session key. The client generates a pre-master secret and encrypts it using the server’s public key. Both client and server then derive a session key for secure communication.

---

### 🔹 Change Cipher Spec
![Change Cipher Spec](change-cipher.png)

The Change Cipher Spec message indicates the transition to encrypted communication. After this step, both client and server use the established session key and selected cipher suite to securely exchange data.

---

## 📊 Outcome
- Analysed full TLS handshake process
- Understood secure communication mechanisms
- Gained practical experience using Wireshark

---

## 💡 Skills Gained
- Network Traffic Analysis
- Wireshark
- TLS/SSL Understanding
- Cybersecurity Fundamentals
- Packet Inspection
