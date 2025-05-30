## EXP NO: 1 - IMPLEMENTATION OF CAESAR CIPHER

```
NAME: B. DHANUSH KUMAR
REG NO: 212224240034
```
 

## AIM:

To implement the simple substitution technique named Caesar cipher using C language.

## DESCRIPTION:

To encrypt a message with a Caesar cipher, each letter in the message is changed using a simple rule: shift by three. Each letter is replaced by the letter three letters ahead in the alphabet. A becomes D, B becomes E, and so on. For the last letters, we can think of the
alphabet as a circle and "wrap around". W becomes Z, X becomes A, Y bec mes B, and Z
becomes C. To change a message back, each letter is replaced by the one three before it.

## EXAMPLE:



![image](https://github.com/Hemamanigandan/CNS/assets/149653568/eb9c6c43-8c80-4cdd-b9d4-91705a311c79)


## ALGORITHM:

### STEP-1: Read the plain text from the user.
### STEP-2: Read the key value from the user.
### STEP-3: If the key is positive then encrypt the text by adding the key with each character in the plain text.
### STEP-4: Else subtract the key from the plain text.
### STEP-5: Display the cipher text obtained above.


PROGRAM :-

### Caesar Cipher encryption function

def caesar_encrypt(text, shift): encrypted_text = ""
 # Traverse the text and encrypt each character
 for char in text:
 if char.isalpha():
 # Get the ASCII code of the character
 start = 65 if char.isupper() else 97
 encrypted_text += chr((ord(char) - start + shift) % 26 + start)
def caesar_decrypt(text, shift): decrypted_text = ""
 if name == "main": text = input("Enter the text: ") shift = int(input("Enter the shift value: "))
    else:
        encrypted_text += char  # Non-alphabet characters are not encrypted
 return encrypted_text
 
### Caesar Cipher decryption function
 # Traverse the text and decrypt each character
 for char in text:
    if char.isalpha():
        # Get the ASCII code of the character
        start = 65 if char.isupper() else 97
        decrypted_text += chr((ord(char) - start - shift) % 26 + start)
    else:
        decrypted_text += char  # Non-alphabet characters are not decrypted
 return decrypted_text
 
 ### Test the Caesar Cipher
 # Encrypt the text
 encrypted_text = caesar_encrypt(text, shift)
 print(f"Encrypted Text: {encrypted_text}")
 # Decrypt the text
 decrypted_text = caesar_decrypt(encrypted_text, shift)
 print(f"Decrypted Text: {decrypted_text}")
 decrypted_text = caesar_decrypt(encrypted_text, shift)
 print(f"Decrypted Text: {decrypted_text}")



OUTPUT :-

![Screenshot 2025-03-24 195215](https://github.com/user-attachments/assets/74c28cf0-d419-41ab-b5a1-4f02f6c064f9)

