### Chapter Four Authenticated Encryption
1. Symmetric encryption is a cryptographic primitive that can be used to protect data confidentiality. It relies on a symmetric key that must remain secret.
2. AES: Advanced Encryption Standard
3. Symmetric encryption must be be authenticated or ciphertexts could be tampered with
4. Authenticated encryption can be used with a symmetric encryption algorithm and a MAC, but prefer to use AEAD or similar constructions as they are harder to misuse.
5. AEAD: Authenticated Encryption with Associated Data
6. IV: Initialization Vector
7. SIV Synthetic Initialization Vector
    1. SIV is more tolerance to nonce repetitions as the nonce is generated from the original plaintext making it unlikely two different plain texts would be encrypted with the same nonce.
8. Real world cryptography has constraints and not every algorithm will fit for every scenario. For Example, database or disk encryption may require different encryption than messages.
