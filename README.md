# Foundations of Network Security Programming Project

Symmetric cryptography encodes message via transformations using a secret key known only to the sender and receiver. The original message can be viewed by going through reversing these transformations using the same pre-shared key. The process of obfuscating the original text is called encryption, while the reverse is decryption. The Data Encryption Standard (DES) was one of the most widely used symmetric block ciphers and was based on the Fiestel Cipher Structure. A similar encryption standard based upon the Fiestel cipher structure is the Tiny Encryption Algorithm (TEA).

### Project Tasks:
###### Task 1:
Investigate TEA in further detail and write a one-page write-up on the specific properties of TEA.
###### Task 2:
Implement any *two* of the modes of operation of your choice from the following: cipher block chaining (CBC), counter mode (CTR), or output feedback (OFB) for TEA. This implementation must be done in the C programming language. Use the TEA source code and add the two additional functions for each block cipher mode you're implementing. For example: cbc_encrypt and cbc_decrypt. Each of the new functions must call the original encrypt and decrypt functions of TEA.

From there, write the C code for encryption and decryption using the corresponding block cipher modes in the DES implementation using the OpenSSL or GNUPG Libcrypt library. You do *not* have to implement these block cipher modes in DES from the ground-up. You may use appropriate OpenSSL or Libcrypt library functions already available for DES.
###### Task 3:
Do performance measurements for TEA and DES in the block cipher modes of operation that you implemented earlier. What is needed is to record the time it takes for encryption and decryption for various message sizes. Your C program should be able to read the data to be encrypted from a file and write the output to a file. You should create text files of sizes 64, 512, 4096, and 32768 ASCII characters as input files from which data will be read as input to your program. The code should be able to encrypt and decrypt the information as well as measure the time it takes to perform both operations in both modes of operations you have implemented.