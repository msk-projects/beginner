### 5. 📝 To-Do List  
**Category:** CLI · Productivity · Filesystem  
**Level:** Beginner  
**Suggested Languages:** Python, JavaScript (Node.js), Java, C#  

**🎯 Overview**  
A simple command-line to-do list manager where users can add, complete, delete, and list tasks. Data should be stored in a local JSON file.  

**✅ Requirements / Features**  
- Add new tasks with a description  
- Mark tasks as **done** or **pending**  
- Delete tasks by ID  
- List all tasks or filter by status (done/pending)  
- Save tasks persistently in a JSON file  

**💻 Example Usage**  
```bash
todo add "Finish Python homework"
# Output: Task added (ID: 1)

todo add "Read a book"
todo list
# Output:
# [1] Finish Python homework (pending)
# [2] Read a book (pending)

todo done 1
# Output: Task 1 marked as done ✅

todo list done
# Output:
# [1] Finish Python homework (done)

todo delete 2
# Output: Task 2 deleted 🗑️
```

**🗂️ Data Model (JSON Example)**  
```json
{
  "tasks": [
    {
      "id": 1,
      "description": "Finish Python homework",
      "status": "done",
      "createdAt": "2025-09-03T11:20:00Z"
    }
  ]
}
```

**🚀 Getting Started**  
1. Create CLI entry (`todo`)  
2. Implement JSON storage for tasks  
3. Build commands: `add`, `list`, `done`, `delete`  
4. Add filtering by status (`list done`, `list pending`)  
5. Test persistence across multiple runs  

---
