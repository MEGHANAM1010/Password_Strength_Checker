# 🔐 Password Strength Checker

A beginner-friendly Python tool that evaluates password strength across multiple security dimensions and returns a rating with actionable feedback — built as Project 1 for CyberSecurity portfolio.

---

## 📌 Project Overview

This tool analyzes a given password and checks it against key security criteria — length, character variety, and special characters. It gives a score out of 6 and a strength rating with specific feedback on what to improve.

---

## 🚀 Features

| Feature | Description |
|---|---|
| Length check | Flags passwords under 8 and 12 characters |
| Digit check | Ensures at least one number is present |
| Uppercase check | Validates presence of capital letters |
| Lowercase check | Validates presence of small letters |
| Special character check | Regex-based detection of symbols |
| Score-based rating | 4-tier strength rating (Very Weak → Strong) |
| Multi-issue feedback | Reports ALL issues at once, not just the first one |
| Interactive loop | Continuously checks passwords until user exits |

---

## 🧠 Concepts Demonstrated

| Concept | Where Used |
|---|---|
| Regular Expressions (Regex) | Special character detection via `re.search()` |
| List truthiness | `if issues:` to check for empty list |
| f-strings / string formatting | Clean output display |
| Modular functions | Separate `check_password_strength()` and `password_checker()` |
| Loop control | `while True` + `break` on exit |
| Password entropy basics | Scoring based on length + character diversity |

---

## 📊 Scoring System

| Score | Rating |
|---|---|
| 5 – 6 | 🟢 Strong Password |
| 3 – 4 | 🟡 Moderate Password |
| 1 – 2 | 🟠 Weak Password |
| 0 | 🔴 Very Weak Password |

---

## 🗂️ File Structure

```
password-strength-checker/
│
├── password_checker.ipynb    # Google Colab notebook
└── README.md                 # Project documentation
```

---

## ▶️ How to Run

### Google Colab
1. Open [Google Colab](https://colab.research.google.com)
2. Paste the code into a new cell
3. Run the cell and enter passwords when prompted

### Local (Python 3.x)
```bash
python password_checker.py
```
No external libraries needed — only Python's built-in `re` module.

---


