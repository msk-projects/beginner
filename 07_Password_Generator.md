# 7. 🔐 Password Generator

**Category:** CLI · Security · Randomization
**Level:** Beginner
**Suggested Languages:** Python, JavaScript (Node.js), Java, C++, Go

**🎯 Overview**
A command-line tool that generates secure, random passwords. Users can specify the password length and which character sets (uppercase, lowercase, digits, symbols) to include.

**✅ Requirements / Features**

* Accept password length as input
* Options to include/exclude:

  * ✅ Uppercase letters (A–Z)
  * ✅ Lowercase letters (a–z)
  * ✅ Numbers (0–9)
  * ✅ Special characters (!, @, #, \$, etc.)
* Generate multiple passwords at once
* Ensure strong randomness (use system libraries like `secrets` in Python or `crypto` in Node.js)
* Optionally save generated passwords into a file (JSON or text)

**💻 Example Usage**

```bash
passgen 12 --upper --lower --digits --symbols
# Output: A$k9rX!bT2zP

passgen 16 --upper --lower --digits
# Output: N4kP7tW8xQ9sL2dH

passgen 8 --lower --digits
# Output: g5h2k1r8
```

**🗂️ Optional JSON for Storage (if saving history)**

```json
{
  "passwords": [
    {
      "id": 1,
      "value": "A$k9rX!bT2zP",
      "length": 12,
      "options": ["upper", "lower", "digits", "symbols"],
      "generatedAt": "2025-09-03T14:10:00Z"
    }
  ]
}
```

**🚀 Getting Started**

1. Set up a CLI entry (`passgen`)
2. Implement flags for password length and options
3. Use a secure random generator (avoid simple `rand()`)
4. Print the generated password(s) to the terminal
5. Optional: add export option to save into a file

---
