# Secure CSV-Based Authentication System (PHP + SHA-256)

This project implements a secure signup and login system using PHP and CSV as the backend storage.

Passwords are never stored in plaintext. They are converted to SHA-256 hash values before being written to the database, following industry-standard cybersecurity practices.

## Features

- User signup with password confirmation
- Password hashing using SHA-256
- Secure credential storage in CSV
- Login authentication using hash verification
- Protection against direct access to backend scripts
- Information disclosure prevention

## Technologies Used

- HTML
- PHP
- CSV (as database)
- SHA-256 Cryptographic Hashing

## How It Works

1. User signs up using the signup form.
2. The password is converted into a SHA-256 hash.
3. The username and hash are stored in a CSV file.
4. During login, the entered password is hashed again.
5. The system checks if the hash matches the stored value.
6. If matched, access is granted.

## Security Design

- Plaintext passwords are never stored.
- Backend PHP scripts cannot be accessed directly via URL.
- The system prevents information leakage.

This project demonstrates the implementation of secure authentication logic similar to real-world web applications.

