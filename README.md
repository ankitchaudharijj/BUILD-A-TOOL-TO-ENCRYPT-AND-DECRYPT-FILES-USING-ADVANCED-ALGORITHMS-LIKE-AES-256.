# 🔐 Advanced File Encryption Tool

A secure file encryption and decryption tool built using Python and Tkinter. It leverages AES-256 encryption with PBKDF2 key derivation to provide strong protection for your files.

## 📦 Features

- AES-256 encryption using CBC mode
- Secure password-based key derivation (PBKDF2 with SHA-256)
- Random salt and IV for each encryption
- Graphical User Interface (GUI) built with Tkinter
- Automatic padding and depadding (PKCS7)
- Easy-to-use file selection dialogs
- Error handling with user-friendly messages

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ankitchaudharijj/encryption_tool.git
   cd encryption_tool
   ```

2. Install dependencies:
   ```bash
   pip install cryptography
   ```

## 🚀 Usage

Run the application:

```bash
python encryption_tool.py
```

### GUI Options:

- **Encrypt File**: Select any file you want to encrypt. Enter a strong password when prompted. The output will be saved as `filename.ext.enc`.
- **Decrypt File**: Select an `.enc` file. Enter the password used during encryption. The decrypted file will be saved as `filename.ext.dec`.

## 🧠 How It Works

- A random 16-byte salt and IV are generated for each encryption.
- A secure 256-bit key is derived from the password using PBKDF2 with 100,000 iterations.
- Data is encrypted using AES-CBC and padded to a multiple of 16 bytes.
- Decryption reverses the process using the original salt and IV from the encrypted file.

## 🔐 Security Notes

- Always use a strong password.
- This tool does not store or transmit your password.
- If the password is lost, the encrypted data cannot be recovered.

## 📁 File Structure

```bash
encryption_tool.py   # Main GUI and logic script
README.md            # Project documentation
```

## 🧑‍💻 Author

**Ankit Chaudhari**  
Certified Ethical Hacker (CEH v12) 
- 🌐 GitHub: [ankitchaudharijj](https://github.com/ankitchaudharijj)  
- 💼 LinkedIn: [ankit-chaudhari](https://www.linkedin.com/in/ankit-chaudhari-40346b318/)

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
