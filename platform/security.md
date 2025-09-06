---
description: Our approach to security
icon: shield-check
---

# Security

aigent.run is built around the principle that **users should always remain in control of their assets**.\
Your account is flexible, you can use the default background wallet, link an external wallet, or delegate funds to your agent. Each option has its own security profile, and we’ve designed safeguards around all of them.

### **Account Security**

#### **Default Account (Auto-Wallet)**

* When you create an account, a secure wallet is generated in the background.
* You can choose between:
  * **Passkey authentication** (recommended) — Uses device-based cryptography for passwordless, phishing-resistant logins.
  * **PIN-based authentication** — A user-defined PIN encrypts and decrypts your wallet locally.

Both methods ensure your private key is **never transmitted to servers or stored in plaintext**.

#### **External Wallets**

* You can link wallets like **Xaman** or **Joey** for full custody control.
* All transactions require explicit approval in your external wallet app.
* This is the **most secure option** for users managing significant funds.

#### **Agent-Managed Wallet**

* You may fund your agent’s wallet directly.
* This allows your agent to transact autonomously, without needing your approval each time.
* Best for users running automated strategies, but requires trust in the agent’s rules and settings.

***

### **Authentication & Encryption**

#### **Passkeys**

* Passkeys replace traditional passwords with device-level cryptography.
* They are resistant to phishing, credential leaks, and reuse attacks.
* With passkeys, your device generates and stores the private key securely, ensuring seamless and secure access.

#### **PINs**

* PINs remain available for users who prefer a simple setup.
* When used, your PIN is transformed into an encryption key that locks your private key locally.
* Private keys are only decrypted in-browser with the correct PIN.

***

### **Best Practices**

To keep your account secure, we recommend:

* **Use passkeys wherever possible** → They are more secure than PINs and provide a smoother login experience.
* **Choose strong PINs if you use them** → Avoid simple sequences like “1234.”
* **Use external wallets for large holdings** → Default/agent accounts are best for daily activity, external wallets for major funds.
* **Keep your device secure and updated** → Avoid malware and outdated software.
* **Withdraw long-term funds** → Treat the terminal as a hot wallet, not a vault.

***

### **Important Note**

aigent.run prioritizes **speed, usability, and interaction,** not long-term storage.\
For maximum safety:

* Treat the terminal as a **hot wallet interface**.
* Use it for trading, automation, and agent interaction.
* Store significant holdings in external or cold wallets.
