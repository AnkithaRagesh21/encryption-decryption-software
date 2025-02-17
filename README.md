# encryption-decryption-software
🔐 Encryption Decryption Software
📌 Overview
This is a Python-based GUI application for file encryption and decryption using AES encryption. It allows users to securely encrypt any file and later decrypt it using a secret key. The software is built using Tkinter for GUI and PyCryptodome for encryption.

🔧 Features
✔ Encrypt any file (Images, PDFs, Text, etc.)
✔ Decrypt previously encrypted files
✔ Uses AES encryption for high security
✔ Simple and user-friendly GUI
✔ Progress tracking during encryption & decryption
✔ Cancel encryption/decryption mid-process
✔ Remembers encryption key for correct decryption

📂 File Structure
main.py → The main script containing GUI and encryption logic
README.md → Project documentation
requirements.txt → Dependencies for the project
🚀 Installation & Usage
📌 Prerequisites
Make sure you have Python 3.x installed on your system.

🔧 Install Dependencies
Run the following command to install required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
🔄 Running the Application
Run the following command to start the Encryption Decryption Software:

bash
Copy
Edit
python main.py
📖 How to Use
📌 Steps for Encryption
Select the file you want to encrypt by clicking the "SELECT FILE" button.
Enter a secret key (This is required for decryption later).
Click the "ENCRYPT" button.
A new encrypted file with .kryp extension will be created in the same directory.
You can reset the input fields by clicking the "RESET" button.
📌 Steps for Decryption
Select the encrypted file (.kryp file).
Enter the same secret key that was used for encryption.
Click the "DECRYPT" button.
The original file will be restored with the suffix __dekrypted__.
If the wrong key is used, decryption will fail.
📌 Canceling Encryption/Decryption
You can cancel the process at any time by clicking the "CANCEL" button.
🔒 How It Works
Uses AES encryption (CFB mode) for secure file encryption.
The key and salt are hashed using SHA256 for added security.
Encryption Output File: filename.extension.kryp
Decryption Output File: filename__dekrypted__.extension
🛠️ Technologies Used
Python 3.x
Tkinter (GUI Framework)
PyCryptodome (AES Encryption)
OS & File Handling
📌 Known Issues & Future Improvements
🚨 Issues
Does not support bulk file encryption.
Incorrect key input results in corrupted decrypted files.
🚀 Future Enhancements
✅ Add password verification before encryption
✅ Support drag-and-drop file selection
✅ Implement bulk encryption for multiple files
✅ Improve UI design for better user experience
