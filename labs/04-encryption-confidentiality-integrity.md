# Lab: Encryption for Confidentiality & Integrity

**Tools:** GPG / Kleopatra, symmetric and asymmetric encryption

## What I did
- Generated **public/private key pairs**, checked fingerprints, and exchanged public keys between two users' certificate stores.
- **Signed and encrypted** a file with the recipient's public key, then decrypted and verified it on the other side.
- Encrypted a file symmetrically with a passphrase and compared the two approaches.
- Used **hybrid cryptography**: a symmetric key for the data, protected with asymmetric encryption for transfer.
- Digitally signed a document with GPG.

## Takeaway
Asymmetric keys solve the key-exchange problem, symmetric encryption is what makes bulk data fast, and real systems use both. A signature proves who sent a file and that it wasn't changed. I later built my own AES-256 tool in C (see my `aes256-file-encryptor` repo).
