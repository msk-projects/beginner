### 3. 💸 Expense Tracker

**Category:** CLI · Filesystem · Budgeting
**Level:** Beginner

**🎯 Overview**
A CLI application to record expenses and incomes, organize them by categories, and generate simple summaries. Data is stored locally in a JSON or CSV file.

**✅ Requirements / Features**

* Commands to add, list, delete, and summarize entries
* Each entry includes: `id, date, type (expense|income), amount, category, note`
* Option to set and check monthly budgets by category
* Store data in JSON or CSV format (auto-create file if missing)
* Summarize expenses by date, category, or month

**💻 Example Usage**

```bash
xp add --type expense --amount 350 --cat food --date 2025-09-03 --note "Lunch"
xp add --type income --amount 1000 --cat freelance --note "Website work"
xp list --cat food --from 2025-09-01 --to 2025-09-30
xp summary --by category --month 2025-09
xp budget set --cat food --amount 3000
xp budget status --month 2025-09
```

**🗂️ Data Model (JSON Example)**

```json
{
  "entries": [
    {
      "id": 1,
      "date": "2025-09-03",
      "type": "expense",
      "amount": 350,
      "category": "food",
      "note": "Lunch"
    }
  ],
  "budgets": {
    "food": 3000
  }
}
```

**🚀 Getting Started**

1. Set up a project folder with `xp-cli` entry file
2. Implement argument parsing with subcommands
3. Build storage helper to read/write JSON or CSV
4. Implement core commands (`add`, `list`, `summary`, `budget`) one by one
5. Test by adding multiple entries and checking budget limits

---
