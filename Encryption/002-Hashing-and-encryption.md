# Hashing vs Encryption: Explanation and Differences

## What is Hashing?

Hashing is a one-way cryptographic process that transforms input data (such as a password) into a fixed-length string (hash value). The output, called a hash, cannot be reversed to retrieve the original data. Hashing is commonly used for data integrity verification and password storage.

### Characteristics of Hashing:
- **One-way function:** Once data is hashed, it cannot be reversed.
- **Fixed-length output:** Produces a fixed-length hash value, regardless of input size.
- **Used for data integrity checks and password storage.**
- **Collision resistance:** Different inputs should always produce different hashes.
- **Common hash functions:** SHA-256, MD5, and SHA-1.

### Use Cases of Hashing:
- **Password Storage:** Instead of storing actual passwords, systems store their hash values.
- **Data Integrity Verification:** Ensures data has not been modified (e.g., file checksums).
- **Digital Signatures & Blockchain:** Used in cryptographic applications like digital signatures and blockchain transactions.

---

## What is Encryption?

Encryption is a two-way cryptographic process that converts readable data (plaintext) into unreadable data (ciphertext) to prevent unauthorized access. The encrypted data can be decrypted back to its original form using a secret key.

### Characteristics of Encryption:
- **Two-way function:** Data can be encrypted and later decrypted.
- **Key-based security:** Uses encryption keys to lock and unlock the data.
- **Confidentiality:** Protects data from unauthorized access.
- **Types:** Can be symmetric (same key for encryption & decryption) or asymmetric (different keys).
- **Common encryption algorithms:** AES, RSA, and Blowfish.

### Use Cases of Encryption:
- **Secure Communication:** HTTPS, email encryption (PGP), VPNs.
- **Data Protection:** Encrypting files, databases, or disk drives.
- **Secure Transactions:** Online banking, digital payments, and cryptocurrencies.

---

## Key Differences Between Hashing and Encryption

| Feature | Hashing | Encryption |
|---------|--------|------------|
| **Purpose** | Ensures data integrity and prevents modification | Ensures data confidentiality and restricts access |
| **Reversibility** | Irreversible (one-way function) | Reversible with a decryption key |
| **Output** | Fixed-length hash value (e.g., 256-bit for SHA-256) | Variable-length ciphertext |
| **Key Usage** | No key required | Requires a key (symmetric or asymmetric) |
| **Use Cases** | Password storage, checksums, blockchain | Secure communication, data protection, online transactions |
| **Examples** | SHA-256, MD5, SHA-1 | AES, RSA, Blowfish |
