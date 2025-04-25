# pyca/cryptography

[![Latest Version](https://img.shields.io/pypi/v/cryptography.svg)](https://pypi.org/project/cryptography/)
[![Latest Docs](https://readthedocs.org/projects/cryptography/badge/?version=latest)](https://cryptography.io)
[![CI](https://github.com/pyca/cryptography/workflows/CI/badge.svg?branch=main)](https://github.com/pyca/cryptography/actions?query=workflow%3ACI+branch%3Amain)

`cryptography` is a Python package designed to provide cryptographic recipes and primitives for developers. Its goal is to serve as your "cryptographic standard library." The package supports **Python 3.7+** and **PyPy3 7.3.11+**.

---

## 🚀 Features

`cryptography` offers both:
- **High-level recipes**: For easy-to-use cryptographic operations.
- **Low-level interfaces**: For common cryptographic algorithms, such as symmetric ciphers, message digests, and key derivation functions.

### Example: Symmetric Encryption
Here's how to encrypt and decrypt a message using the high-level symmetric encryption recipe:

```python
from cryptography.fernet import Fernet

# Generate and store this key securely!
key = Fernet.generate_key()
cipher = Fernet(key)

# Encrypt the message
encrypted_message = cipher.encrypt(b"A really secret message. Not for prying eyes.")
print(encrypted_message)

# Decrypt the message
decrypted_message = cipher.decrypt(encrypted_message)
print(decrypted_message)
```

For more details, visit the [documentation](https://cryptography.io/).

---

## 📦 Installation

Install `cryptography` using pip:

```bash
pip install cryptography
```

For comprehensive installation instructions, see the [Installation Guide](https://cryptography.io/en/latest/installation/).

---

## 💬 Discussion & Support

### Reporting Issues
Encounter a bug? File an issue in our [issue tracker](https://github.com/pyca/cryptography/issues).

### Development Discussions
Join our [cryptography-dev mailing list](https://mail.python.org/mailman/listinfo/cryptography-dev) for development-related discussions.

### Community Chat
Connect with the community in the `#pyca` channel on [irc.libera.chat](https://libera.chat/).

---

## 🔒 Security

If you discover a security issue, please consult our [security reporting guide](https://cryptography.io/en/latest/security/) for instructions on how to report it responsibly.

---

## 📚 Resources

- **Documentation**: [https://cryptography.io/](https://cryptography.io/)
- **Installation Guide**: [https://cryptography.io/en/latest/installation/](https://cryptography.io/en/latest/installation/)
- **Issue Tracker**: [https://github.com/pyca/cryptography/issues](https://github.com/pyca/cryptography/issues)
- **Mailing List**: [cryptography-dev](https://mail.python.org/mailman/listinfo/cryptography-dev)
- **Security Reporting**: [https://cryptography.io/en/latest/security/](https://cryptography.io/en/latest/security/)

---

`cryptography`: Secure, simple, and robust cryptographic tools for Python developers.
