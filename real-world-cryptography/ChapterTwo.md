## Chapter Two: Hash Functions

A hash function takes any input data and produces a unique string of bytes in
return

Given the same input, a hash function always reproduces the same output

The output of a hash function is called a digest or a hash

This is commonly used to verify downloads using a sha256sum to validate the
file you downloaded produces the hash of the file you expected to download.
This alone does not verify the integrity of the file because an attacker could
have modified the expected hash on the webpage, so we have to rely on othre
trusted mechanisms such as HTTPS to ensure the expected hash is valid

file -> Hash Function -> f63e...

### Security Properties of Hash Functions

1. Pre-image resistance
    1. For a given digest, it is impossible to find the original input
    2. Something too small or predictable cannot be hidden
        1. Ex: If you know the input is yes or no, you can hash both values and
           compare the result to identify the input
2. Second pre-image resistance
    1. For a given input and digest, a second input that hashes to the same
       digest does not exist
    2. We do not choose the input in this scenario
3. Collision resistance
    1. There does not exist a digest that can be produced by two different
       inputs
4. Random Oracle
    1. A model used to prove that hash functions return random data so that no
       part of the input can be identified from a given digest

### Security Considerations
1. 


###
