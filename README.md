# 🔒 SecureEncryptionUtil for ServiceNow (Scoped + Global Apps)

> Production-ready 🔥 Secure Encryption & Decryption Utility  
> Built with ❤️ for ServiceNow Developers who need **Scoped App** data security.

---

## 🛡️ About

ServiceNow doesn't allow easy encryption in Scoped Apps.  
This plugin solves that pain — with a **plug-and-play** utility you can use anywhere!

- ✨ Lightweight and fast
- ✨ Scoped Apps + Global Apps ready
- ✨ Encrypt & Decrypt easily
- ✨ System Properties driven 🔥
- ✨ Customizable secret keys
- ✨ Base64-based secure layer
- ✨ No GlideEncryptor dependency
- ✨ Non-predictable output
- ✨ Highly extensible for future versions

---

## 🔥 Features

- **Scoped Encryption/Decryption** (without native API)
- **Masked output** for unauthorized users
- **Dynamic secret key management**
- **Simple API interface (like GlideRecord)**

---

## 🛠️ Installation

1. Import the **Update Set** into your ServiceNow instance.
2. Create **System Properties**:
   
| Name | Type | Example Value |
|:-----|:-----|:--------------|
| `secure_util.secret_key` | String | `3x$Tr0ngP@ssKey!7eNRY` |
| `secure_util.password2` | Password | `B0nusP@ssL@yer!` |

✅ That's it! You're ready.

---

## ⚡ How to Use

```javascript
var secure = new SecureEncryptionUtil();

// Encrypt data
var encrypted = secure.encrypt('Sensitive Passport Number 123456789');
gs.info('Encrypted: ' + encrypted);

// Decrypt data
var decrypted = secure.decrypt(encrypted);
gs.info('Decrypted: ' + decrypted);

```

## 🧠 How It Works

🔑 Secret key fetched from system properties

🧂 Optional password2 adds double security

🔄 XOR + Base64 transformation

🔁 Non-predictable and safe for scoped apps

## 🌟 Why Use SecureEncryptionUtil?

ServiceNow Scoped Apps don't allow native encryption easily.

Secure sensitive fields like Passport Numbers, SSN, Bank Accounts.

Minimal setup, maximum protection.

Extensible: Future versions will include Role-based Decryption, Dynamic Salt, Field Policies, and more!

##🛡️ Upcoming V2 Features (Sneak Peek)
🎯 Role-Based Decryption

🎭 Partial Masking for unauthorized users

🧂 Dynamic Salt per record

📝 Decryption Audit Logging

🔄 Key Rotation Support

🧠 Multi-Algorithm Encryption Support (AES, Base58)

## 🤝 Contributing
Pull Requests and Suggestions are welcome!
Let's make Scoped Apps more secure together. 🔥

📢 Author
Made with 💻 + ☕ by <b>Abhishek Aggarwal</b>
Connect on  and Twitter <a href=">www.linkedin.com/in/abhishek-aggarwal-179085192">LinkedIn</a>

📜 License
This project is licensed under the MIT License.
Feel free to use and build amazing things! 🚀
