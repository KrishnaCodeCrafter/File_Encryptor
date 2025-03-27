# File Encryptor

A simple command-line application that encrypts and decrypts files using the XOR cipher. Built with C++, this tool allows users to protect their files by encoding them with a numeric key.

## Features
- Encrypts and decrypts any file type (text, images, videos, executables, etc.).
- Uses XOR-based encryption for lightweight file security.
- Reads and writes files in binary mode to preserve content integrity.
- Command-line interface for easy operation.

## How It Works
XOR encryption works by applying the XOR (`^`) operation between each byte of the file and a numeric key. The same key is used for both encryption and decryption.

## Installation
### Prerequisites
- A C++ compiler (GCC, MinGW, or MSVC)
- Command-line interface (Terminal, Command Prompt, or PowerShell)

### Compilation
```sh
# Compile the program
 g++ file_encryptor.cpp -o file_encryptor
```

## Usage
Run the compiled executable:
```sh
./file_encryptor  # On Linux/macOS
file_encryptor.exe  # On Windows
```

### Encrypting a File
```
1. Encrypt File
Enter file name to encrypt: myfile.txt
Enter encryption key (numeric): 123
File encrypted successfully! Saved as myfile.txt.enc
```

### Decrypting a File
```
2. Decrypt File
Enter file name to decrypt: myfile.txt.enc
Enter decryption key (same as encryption key): 123
File decrypted successfully! Saved as decrypted_myfile.txt
```

## Limitations
- XOR encryption is weak and should not be used for highly sensitive data.
- If the wrong key is used for decryption, the file will become unreadable.
- The decrypted file may not retain its original extension; manual renaming may be required.


