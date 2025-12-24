# Encoding : 

- The process of converting data from one format to other(machine understandable) so it can correctly stored, sent and processed. Commonly used in Storage and file safe transfer.

 **Text to Binary Encoding** : 
 
 - ASCII converts alphabets to binary. Example : Text: Hello → Binary: 01001000 01100101 01101100 01101100 01101111
 - Unicode converts all characters from all languages and symbols/emojis into binary. Example : Character 😊 UTF-8(Unicode Transformation format) binary encoding: 11110000 10011111 10011000 10001010


 **Binary to Text Encoding** : 

 - Hexadecimal : Binary into base-16 digits (0–9, A–F). Example: Binary: 01001000 01100101 01101100 01101100 01101111 -> Hex: 48 65 6C 6C 6F
 - Base64 : Binary data into 64 printable characters (A–Z, a–z, 0–9, +, /). Example: Binary: 01001000 01100101 01101100 01101100 01101111 -> Base64: SGVsbG8=


# Encryption : 

-  The process of converting information into the ciphertext(unreadable) so that only authorised person can read it. It uses an algorithm and key to scramble the data and can be get back to its original form by decryption with a secret key. Commoly used to save and protect passwords, messages and online transactions. 


## Types of Encryption :

**Symmetric Encryption** :  Uses same key for encrypting and decrypting the data. Faster and commonly used for large amount of data. 

1. AES (Advanced Encryption Standard) : Modern & Very secure encryption. Uses IV(Initializing Vector) for mode like cbc, cfb, ofb, ctr and ebc doesn't need IV and a key to encrypt
2. DES (Data Encryption Standard) : Older encryption standard
3. 3DES(Triple DES) : Encrypts 3 times using DES make it stronger.
4. Blowfish & Twofish

**Asymmetric Encryption** : Uses two different key for encrypting and decrypting the data. Public key to encrypt and private key to decrypt. Slower but more secure.

1. RSA(Rivest–Shamir–Adleman) : Widely used for secure data transmission. It is used for encrypting small messages or keys



