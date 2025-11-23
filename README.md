# python-encrypt-decrypt-system-project-
A simple Python-based file encryption and decryption tool using the Fernet symmetric encryption algorithm. Supports secure key generation, file protection, and safe decryption.
Name- Shivanand Irappa Sangammanavar
Reg No. – 25BAI11346
Slot- A24+E21+F22
Subject - Introduction to problem solving and programming-CSE1021
Faculty - Dr. Manimaran


# File Encryption & Decryption System (Python)

This project provides a simple and secure *file encryption and decryption tool* using Python’s cryptography library- Fernet.

It allows users to generate a secret key, encrypt any file, and decrypt it back safely.

## Features
- Generate a secure encryption key
- Encrypt any type of file: text, image, PDF, etc
- Decrypt previously encrypted files
- Uses industry-standard AES-128 encryption (Fernet)
- Easy to run from terminal
- 
Requirements Install the required package before running the project: ```bash pip install cryptography

Code-
<img width="1056" height="874" alt="image" src="https://github.com/user-attachments/assets/e996d51c-5e56-4620-9f3c-c112688b5cfe" />
Output-
<img width="975" height="409" alt="image" src="https://github.com/user-attachments/assets/28f50192-e5af-4090-b67f-78f6b099e111" />
<img width="975" height="387" alt="image" src="https://github.com/user-attachments/assets/f1fcf0cd-749b-4485-8782-f7d430157bae" />

flowchart-
<img width="722" height="1051" alt="image" src="https://github.com/user-attachments/assets/085863dd-21a8-4b9f-b4d9-98c8d542fd9f" />
Encrypt-
<img width="975" height="581" alt="image" src="https://github.com/user-attachments/assets/0b027005-dc65-4759-9235-27482203b74b" />
Decrypt-
<img width="975" height="563" alt="image" src="https://github.com/user-attachments/assets/8a94c79a-60c1-4557-88b0-e7cb658874b5" />

Algorithm-
Step 1: Start
Step 2: Ask user
Display:
Enter 'E' to encrypt or 'D' to decrypt the file.
Read input into variable choice
Convert choice to lowercase.
Encryption Process (if choice == 'e')
Step 3: If choice = 'e',
Ask user:
"Enter the file name to encrypt (including file extension):"
Store in filename
Step 4: Check if file exists
If filename exists in the system:
1. Generate a key
call generate_key() → returns Secret.key
2. Load the generated key
key ← load_key()
3. Encrypt the file
Call encrypt(filename, key)
4. Print "File Encrypted Successfully!!!"
Else:
Display error: "File not found. Please check the file name and try again."
Decryption Process (if choice == 'd')
Step 5: If choice = 'd'
Ask user:
"Enter the file name to decrypt (including file extension):"
Store in filename
Step 6: Check if file exists
If filename exists:
1. Load existing key
key ← load_key()
2. Decrypt the file
Call decrypt(filename, key)
If key is invalid → show "Invalid key"
3. print - "File Decrypted Successfully!!!"
Otherwise:
Error Display: "File not found. Please check the file name and try again."
Invalid Choice
Step 7: If choice is neither 'e' nor 'd'
Display: "Invalid choice. Please enter 'E' to encrypt or 'D' to decrypt."
Step 8: Conclusion


How to Use-
1. Generate the Key
python main.py-generate

2. Encrypt a File
python main.py-encrypt file.txt

3. Decrypt a File
python main.py-decrypt file.txt.encrypted

The decrypted file will be restored automatically.
