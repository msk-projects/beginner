# 8. 📇 Contact Book CLI

**Category:** CLI · Filesystem · Productivity
**Level:** Beginner
**Suggested Languages:** Python, Java, C++, JavaScript (Node.js), Ruby

**🎯 Overview**
A simple contact management tool that runs in the terminal. Users can add, update, delete, and search contacts. Data is stored locally (JSON, CSV, or plain text).

**✅ Requirements / Features**

* Add new contacts with details: `name, phone, email, address`
* Update existing contacts
* Delete contacts by ID or name
* Search contacts (by name, phone, or email)
* List all saved contacts
* Store data in a **JSON file** (auto-create if not present)

**💻 Example Usage**

```bash
contacts add "John Doe" --phone 9876543210 --email john@example.com --address "Delhi, India"
# Output: Contact added successfully (ID: 1)

contacts list
# Output: 
# 1. John Doe | 9876543210 | john@example.com | Delhi, India

contacts search "John"
# Output: Found: John Doe | 9876543210 | john@example.com

contacts update 1 --phone 9123456789
# Output: Contact updated successfully

contacts delete 1
# Output: Contact deleted successfully
```

**🗂️ Data Model (contacts.json)**

```json
{
  "contacts": [
    {
      "id": 1,
      "name": "John Doe",
      "phone": "9876543210",
      "email": "john@example.com",
      "address": "Delhi, India",
      "createdAt": "2025-09-03T14:20:00Z",
      "updatedAt": "2025-09-03T14:25:00Z"
    }
  ]
}
```

**🚀 Getting Started**

1. Create CLI entry (`contacts`)
2. Implement CRUD operations (Create, Read, Update, Delete)
3. Use JSON file for persistent storage
4. Add search functionality
5. Optional: export/import contacts to CSV

---
