### 6. 🧮 Calculator

**Category:** CLI · Math · Utilities
**Level:** Beginner
**Suggested Languages:** Python, JavaScript (Node.js), Java, C, C#

**🎯 Overview**
A command-line calculator that performs basic arithmetic operations such as addition, subtraction, multiplication, and division. Optional advanced features include square roots, exponents, and memory functions.

**✅ Requirements / Features**

* Perform basic operations: `+`, `-`, `*`, `/`
* Accept input as command-line arguments
* Handle invalid inputs and division by zero gracefully
* Optionally support advanced operations: `sqrt`, `pow`, `mod`
* Display results in a clean format

**💻 Example Usage**

```bash
calc add 10 5
# Output: 15

calc sub 20 7
# Output: 13

calc mul 6 9
# Output: 54

calc div 50 5
# Output: 10

calc sqrt 81
# Output: 9
```

**🗂️ Data Model (Optional JSON if storing history)**

```json
{
  "history": [
    {
      "id": 1,
      "operation": "add",
      "operands": [10, 5],
      "result": 15,
      "executedAt": "2025-09-03T12:00:00Z"
    }
  ]
}
```

**🚀 Getting Started**

1. Create CLI entry (`calc`)
2. Implement argument parsing for operations
3. Add functions for each operator (`add`, `sub`, `mul`, `div`)
4. Add error handling (e.g., divide by zero, missing args)
5. Optional: store calculation history in JSON file

---
