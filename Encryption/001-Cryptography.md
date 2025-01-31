# Encryption / Cryptography Control Overview

## Definition of Encryption

Encryption is a method that ensures the confidentiality and security of data by converting readable information into an unreadable code, making it impossible for unauthorized parties to access. It works by using cryptographic algorithms and keys to transform plaintext (human-readable data) into ciphertext (unreadable, encoded data). The main goal is to protect sensitive data from unauthorized access, especially in situations where information is being transmitted over networks or stored in databases.

## Purpose

- **Protects Sensitive Data**: Encryption is crucial for securing personal, financial, and communication data, preventing unauthorized access during storage or transit.
- **Prevents Data Breaches**: By converting information into code, it ensures that even if hackers intercept the data, they will not be able to read it without the proper key to decrypt it.
- **Ensures Integrity and Confidentiality**: It guarantees that the data remains confidential and unaltered during transit.

## How Encryption Works

Encryption transforms readable data into unreadable data using an algorithm and a cryptographic key. This process ensures that the data is secure, with only authorized users possessing the necessary decryption key to reverse the process.

### Algorithm and Key

- **Algorithm**: A set of rules that govern how the data will be encrypted.
- **Encryption Key**: A secret parameter used to encode and decode the data. This key is unique and is kept confidential.

### Transformation of Data

- When data is encrypted, it becomes unintelligible to anyone who does not have the decryption key.
- The two-way function means that data can be both encrypted (to secure it) and decrypted (to retrieve the original data).

## Types of Encryption

There are two primary types of encryption systems:

### Symmetric Encryption

- **Definition**: This method uses a single secret key to both encrypt and decrypt data.
- **How it Works**: Both the sender and receiver must possess the same key. If the key is compromised, the entire encrypted data becomes vulnerable.
- **Example Algorithms**: AES, DES, Triple DES.
- **Use Case**: Symmetric encryption is best used for data at rest, like files stored on a hard drive or in a database.
- **Pros**: Faster than asymmetric encryption due to simpler operations.
- **Cons**: Key management is challenging because the same key is used by both parties.

### Asymmetric Encryption (Public Key Cryptography)

- **Definition**: This method uses two keys: a public key (shared openly) and a private key (kept secret).
- **How it Works**:
  - **Public Key**: Used to encrypt data. It is shared with anyone who wants to send a secure message.
  - **Private Key**: Used to decrypt the data. Only the intended recipient knows this key.
- This method ensures that only the intended recipient can decrypt the message, even if it is intercepted during transmission.
- **Example Algorithms**: RSA, Elliptic Curve Cryptography (ECC).
- **Use Case**: Ideal for data in transit, like email communication or HTTPS connections.
- **Pros**: More secure than symmetric encryption in open communication channels, since the private key is never shared.
- **Cons**: Slower compared to symmetric encryption due to more complex algorithms.

## Encryption Algorithms

Encryption algorithms determine how the data is encrypted and decrypted. They are the core of both symmetric and asymmetric encryption.

### AES (Advanced Encryption Standard)

- AES is the most widely used encryption algorithm today, especially for data-at-rest.
- It supports key sizes of 128, 192, or 256 bits, with 256-bit AES being the most secure and commonly used.
- It provides a good balance between speed and security.

### Triple DES (3DES)

- Triple DES applies the DES algorithm three times to each data block, making it more secure than DES alone.
- However, it is becoming obsolete due to its relatively slow performance and vulnerability to modern attacks.

### Blowfish

- A symmetric encryption algorithm that is known for its speed and simplicity.
- While still in use, it has been largely replaced by more secure algorithms like AES.

### RSA

- An asymmetric encryption algorithm widely used for securing data transmission.
- It relies on large prime numbers and is commonly used in public key infrastructure (PKI).

## Encryption for Internet Browsing

When browsing the internet, encryption is crucial to ensuring secure communication between a user's browser and a web server. Encryption protects sensitive data, such as passwords, credit card numbers, and personal details, while they are being transferred between the server and client.

### TLS (Transport Layer Security)

- TLS is the protocol that replaces SSL (Secure Sockets Layer) to encrypt communication over networks.
- TLS ensures that data transmitted between a web server and browser remains secure.
- TLS 1.2 or above is considered the standard for secure communication.

### SSL (Secure Sockets Layer)

- SSL is the predecessor to TLS and is now deprecated.
- While older websites may still use SSL, it is no longer considered secure.
- TLS 1.2 or 1.3 is the recommended version for internet security.

### How to Identify Encryption on Websites

The most common sign that a website uses encryption is the **"HTTPS"** prefix in the URL, followed by a **padlock icon** in the browser address bar.

## Symmetric vs Asymmetric Encryption Use Cases

### Symmetric Encryption

- **Best for Data-at-Rest**: Symmetric encryption is used for securing data stored in databases or on servers.
- It ensures that data is encrypted while it is at rest, making it inaccessible to unauthorized users.

### Asymmetric Encryption

- **Best for Data-in-Transit**: Asymmetric encryption is often used for data that is transmitted over the internet, such as email communications or secure web browsing (HTTPS).
- The public and private keys ensure that even if data is intercepted, only the intended recipient can decrypt it.

## Encryption in Transit & at Rest

### Data-at-Rest

- **Definition**: Data that is stored in a static state, such as in a hard drive, cloud storage, or database.
- **Examples of Encryption Tools for Data-at-Rest**:
  - **eCryptfs**: Linux file-based encryption.
  - **Amazon EBS Encryption**: Amazon Elastic Block Store (EBS) encryption for cloud-based data.
  - **File Vault**: Apple's full-disk encryption for macOS.
  - **BitLocker**: Microsoft's disk encryption software for Windows.
  - **OpenPGP**: Encryption standard for securing email and file data.

### Data-in-Transit

- **Definition**: Data being transmitted over networks, often over the internet.
- **Examples of Encryption Tools for Data-in-Transit**:
  - **SSL Labs**: Tools for checking SSL/TLS configurations.
  - **Qualys**: Provides SSL/TLS security assessments.
  - **TLS Certificates**: Digital certificates used for encrypting communication between web servers and browsers.
  - **HTTPS**: A secure version of HTTP that uses SSL/TLS to encrypt data in transit.
