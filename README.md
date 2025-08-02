# 🔐 Random Password Generator (Python)

This is a simple Python script that generates a **random password** using letters (A-Z, a-z) and special characters (punctuation). It helps you quickly create secure passwords for your accounts or systems.

---

## 🧪 Features

- Generates a password of random characters
- Uses both letters and punctuation symbols
- Adjustable password length (default is 10 characters)
- Lightweight and easy to use

---

## 🧰 Built With

- Python Standard Library:
  - `random`
  - `string`

---

## 💡 How It Works

```python
import random
import string

def generate_password(length: int = 10):
    alphabet = string.ascii_letters + string.punctuation
    password = ''.join(random.choice(alphabet) for i in range(length))
    return password

password = generate_password()
print(f"Generated password: {password}")
