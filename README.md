# 🔐 SecureVault – Client-Side File Encryption Tool

## 📌 Overview

SecureVault is a browser-based file encryption tool that allows users to securely encrypt and decrypt files using a password. The application performs all cryptographic operations directly in the user's browser using the **Web Crypto API**, ensuring that sensitive data never leaves the device.

This project demonstrates practical implementation of modern cryptographic techniques such as **AES-256-GCM encryption** and **PBKDF2 key derivation** for secure file protection.

---

## 🎯 Features

* Upload any file and encrypt it with a password
* Decrypt encrypted files using the correct password
* Client-side encryption (no server involved)
* Drag and drop file upload
* Password strength indicator
* Secure key generation using PBKDF2
* Modern user interface
* Progress indicator for encryption and decryption

---

## 🔐 Security Techniques Used

### AES-256-GCM Encryption

Advanced Encryption Standard (AES) with GCM mode is used to securely encrypt files. It provides strong confidentiality and authentication.

### PBKDF2 Key Derivation

Password-Based Key Derivation Function 2 is used to derive a strong encryption key from the user's password.

### Random Salt & Initialization Vector

Each encryption generates:

* Random **Salt**
* Random **Initialization Vector (IV)**

These ensure that the same password always produces different encrypted outputs.

---

## ⚙️ Technologies Used

* **HTML5**
* **CSS / TailwindCSS**
* **JavaScript**
* **Web Crypto API**

---

## 🛠 How the System Works

### Encryption Process

1. User uploads a file.
2. User enters a password.
3. PBKDF2 derives a secure encryption key from the password.
4. AES-256-GCM encrypts the file.
5. Salt, IV, and encrypted data are combined.
6. Encrypted file is downloaded.

### Decryption Process

1. User uploads the encrypted file.
2. User enters the same password.
3. Salt and IV are extracted.
4. PBKDF2 regenerates the encryption key.
5. AES decrypts the file.
6. Original file is downloaded.

---

## 📂 Project Structure

SecureVault
│
├── index.html
├── style.css
└── script.js

---

## 🚀 How to Run the Project

1. Download or clone the repository

git clone https://github.com/yourusername/securevault.git

2. Open the project folder

3. Run **index.html** in a browser

No installation or backend setup is required.

---

## 🔒 Security Note

All encryption and decryption operations occur locally w
