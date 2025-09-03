# 1. Task Tracker (Beginner)

**🎯 Overview**
Build a CLI tool to manage your tasks. You can **add, update, delete, mark tasks as done or in-progress**, with data stored in a **JSON file**.

**✅ Features / Requirements**

* Run from the terminal using commands
* Store tasks in JSON (auto-create if missing)
* Commands:

  * `add`, `update <id>`, `delete <id>`
  * `mark-in-progress <id>`, `mark-done <id>`
  * `list` (all / todo / in-progress / done)
* Task properties: **id, description, status, createdAt, updatedAt**

**💻 Example CLI Commands**

```bash
task-cli add "Buy groceries"
task-cli update 1 "Buy groceries and cook dinner"
task-cli mark-done 1
task-cli list done
```

**🗂️ JSON Data Structure**

```json
{
  "id": 1,
  "description": "Buy groceries",
  "status": "todo",
  "createdAt": "2025-09-03T06:00:00Z",
  "updatedAt": "2025-09-03T06:00:00Z"
}
```

**🚀 Getting Started**

1. Create project folder and main CLI file
2. Implement argument parsing for commands
3. Create JSON helper functions (`load`, `save`, `nextId`)
4. Implement commands step by step
5. Test thoroughly in terminal

---
