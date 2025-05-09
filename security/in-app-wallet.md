---
description: Built for speed, security and scalability
icon: forklift
---

# In-app Wallet

### Overview

The aigent.run in-app wallet is a secure, browser-only tool that protects users' private keys. The private key is encrypted with a user-defined PIN code and never stored or transmitted in plaintext. Only the PIN can decrypt the encrypted key, ensuring user security and privacy. This wallet is not intended for storing personal funds. It provides a convenient way to transact within aigent.run, enabling users to launch and trade meme tokens and AI agents with ease.

#### Key Features

* **Browser-only wallet**: Operates entirely in the user’s browser. Private keys are never sent to servers.
* **PIN-based encryption**: Ensures that only the user can access their private key.
* **Strong security**: Uses advanced methods to prevent unauthorized access.

### Encryption Process for Wallet Storage

**Main Steps**

1. **Generate random salt**:
   * A unique random value is created to enhance security.
2. **Generate IV (initialization vector)**:
   * Another random value ensures unique encryption results.
3. **Convert PIN to encryption key**:
   * The user’s PIN is processed to create a secure encryption key.
4. **Encrypt private key**:
   * The private key is locked using the encryption key and additional safeguards.

### **Security Details**

* **Salt**: Protects against precomputed attacks (e.g., rainbow tables).
* **Unique encryption key**: Derived using the PIN and salt.
* **Authentication**: Ensures no tampering with encrypted data.

#### Storage Format

Encrypted wallet data includes:

* **Encrypted key**: The locked private key.
* **Salt**: Unique value for security.
* **IV**: Value ensuring unique encryption results.

These components enable decryption using the correct PIN.&#x20;

#### Decryption Process

1. Retrieve encrypted data, salt, and IV.
2. Use the PIN and salt to recreate the encryption key.
3. Unlock the private key using the encryption key and IV.
4. Confirm data hasn’t been tampered with.

#### Security Tips

* **Choose a strong PIN**: Avoid common or easy-to-guess numbers.
* **Keep devices secure**: Ensure your browser and device are safe from malware.
* **Stay updated**: Use the latest browser version to protect against vulnerabilities.
