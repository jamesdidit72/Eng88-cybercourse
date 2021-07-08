# Cryptology
- Encryption:
  - encryption is a process which transforms the original information into an unrecognisable form
- Decryption:
  - decryption is a process of converting encoded/ encrypted data in a form that is readable and understood by a human or a computer 

## Ciphers
A cipher is an algorithm that consists of a series of well-defined steps that can be followed as a procedure when encrypting and decrypting messages
- Two Types:
  - Substitution cipher (Cesar)
  - transposition cipher (Rail fence)
## Encryption classes
- Two Types of encryption algorithm:
  - Symmetric:
    - uses the same key to encrypt and decrypt
  - Asymmetric:
    - uses one key to encrypt and another key to decrypt
    - public and private keys (can encrypt and decrypt with either)

### Symmetric vs Asymmetric
- Symmetric
  - same key
  - shorter keys (40-256 bits)
  - faster
  - commonly used for encrypting bulk data (VPN traffic)
- Asymmetric
  - different keys
  - longer keys (512-4096 bits)
  - slower (computationally tasking)
  - quick data transactions (HTTPS when accessing banking data)

## Hash operations
### Used for authentication (add a secret key)
- each value that is different will have a different hash value
- Example: Contents of plaintext.txt
    - OG contents = "123": hash = hash1
    - 1st updated contents = "abc": hash = hash2
    - 2nd updated contents = "123": hash = hash1
## Cryptanalysis: Code Breaking
All algorithms are breakable (if you have the needed resources and time)
- Methods
  - Brute-force 
  - Ciphertext
  - Known-plaintext
  - Chosen-plaintext
  - Chosen-ciphertext
  - Meet-in-the-middle