# SymmetricKeyCiphers

This repository, **SymmetricKeyCiphers**, provides implementations of various symmetric key cryptographic algorithms and modes. It includes classic ciphers like the Vigenère and transposition ciphers, as well as modern block cipher techniques using DES and AES. The repository is structured to offer both educational insights into cryptography and practical tools for encryption and decryption.

## **Contents**

- `transposition_cipher.py`
- `substitution_cipher.py`
- `vigenere_cipher.py`
- `additional_cipher_modes.py`
- `additional_cipher.py`
- `main.py`

## **Files and Features**

### **1. transposition_cipher.py**
This file implements transposition ciphers:
- **Simple Transposition Cipher:** Encrypts by rearranging the characters in the plaintext based on a key.
- **Double Transposition Cipher:** Uses two permutations (row and column) to encrypt and decrypt text, providing enhanced security over simple transposition.

### **2. substitution_cipher.py**
This file provides basic substitution ciphers:
- **Shift Cipher (Caesar Cipher):** Shifts characters in the plaintext by a fixed number of positions down the alphabet.
- **Permutation Cipher:** Rearranges the characters of the plaintext according to a specified permutation.

### **3. vigenere_cipher.py**
Implements the Vigenère cipher:
- A polyalphabetic substitution cipher that uses a keyword to encrypt and decrypt messages, making it more secure than simple substitution ciphers.

### **4. additional_cipher_modes.py**
Contains implementations for DES cipher modes:
- **ECB (Electronic Codebook) Mode:** Basic block encryption without chaining.
- **CBC (Cipher Block Chaining) Mode:** Uses an initialization vector (IV) to ensure identical plaintext blocks produce different ciphertexts.
- **CFB (Cipher Feedback) Mode:** Converts a block cipher into a self-synchronizing stream cipher.

### **5. additional_cipher.py**
Provides implementations for modern encryption algorithms:
- **AES (Advanced Encryption Standard):** Uses a 128-bit key in CBC mode.
- **DES (Data Encryption Standard):** Classic encryption method using a 56-bit key in CBC mode.
- **3DES (Triple DES):** Applies DES three times with either two or three keys for enhanced security.

### **6. main.py**
Acts as an interface for selecting and executing different encryption techniques:
- Supports both encryption and decryption operations.
- Allows users to choose from various ciphers and modes, enter messages, and specify keys.


Navigate to the directory and run main.py to interact with the different cryptographic algorithms:
`python main.py`

Follow the prompts to select a cipher, input your message, and provide necessary keys or permutations.
### Requirements
Ensure you have Python installed on your system along with any required libraries:  
`pip install pycryptodome`