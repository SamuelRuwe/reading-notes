## Message Authentication Codes (MAC)

1. Message authentication codes are the combination of a hash function and a
   secret code
2. The output of a mac is called an "authentication tag"
3. mac(someSecretKey, someUsername) -> authenticationTag
4. Cookies are an example of MACs in practice. They can take a secret key from
   a user and their username to produce an authentication tag for the user
5. Both sides need to share the same key for MACs to work

### Goal of MACs
1. Prevent authentication tag forgery
    1. Without knowledge of secret key k, a user cannot compute authentication
       tag t = MAC(k, m) on messages m of their choice
    2. MACs are protected against forgeries AS LONG AS THE SECRET KEY STAYS SECRET

### Timing Attacks
1. Comparing two authentication tags must be done in constant time
2. If the computation is not done in constant time, it is because the algorithm returned at the first non-matching bit

HMAC: Hash-based MAC
KMAC: Uses cSHAKE to encode message in a way that is not vulnerable to extension attacks


### Notes
1. Message authentiction codes are symmetric cryptographic algorithms that allow one or more parties who share the same key to verify the integrity and authenticity of messages
2. A message's authenticity is validated by computing the authentication tag using the message and secret key, then comparing the new authentication tag with the received authentication tag
3. MACs do not detect when messages are replayed
4. Authentication tags should be a minimum of 128 bits to prevent collision
