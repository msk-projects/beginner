# 4. 🎲 Number Guessing Game

**Category:** CLI · Game · Randomization
**Level:** Beginner
**Suggested Languages:** Python, JavaScript (Node.js), Java, C, C#

**🎯 Overview**
A simple command-line game where the computer generates a random number and the user tries to guess it. The program gives hints (“too high”, “too low”) until the correct number is guessed.

**✅ Requirements / Features**

* Generate a random number within a user-defined range (e.g., 1–100)
* Accept user guesses from the command line
* Show hints for each guess
* Track the number of attempts
* Option for difficulty levels (easy, medium, hard)
* Restart or exit option after winning

**💻 Example Usage**

```bash
guess-cli start --range 1-100
# Output: "Guess a number between 1 and 100"
> 50
Too low!
> 75
Too high!
> 62
Correct! You guessed it in 3 attempts 🎉
```

**🗂️ Data Model (Optional JSON if storing scores)**

```json
{
  "games": [
    {
      "id": 1,
      "range": "1-100",
      "target": 62,
      "attempts": 3,
      "completedAt": "2025-09-03T10:15:00Z"
    }
  ]
}
```

**🚀 Getting Started**

1. Create CLI entry (`guess-cli`) to start the game
2. Implement random number generator for the target number
3. Accept guesses from user input in a loop
4. Add feedback logic (`too low`, `too high`)
5. Count attempts and end game when guessed correctly
6. Optional: Save scores in a JSON file for later

---
