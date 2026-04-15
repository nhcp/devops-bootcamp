# Module 2, Lesson 08: Working with Vim Editor

## 🧠 Part 1: Core Theory
Vim is the standard text editor for Linux. Since DevOps engineers manage remote servers without a mouse, you must know how to edit configuration files using only your keyboard.

### 🕹️ The 3 Modes You Must Know
1. **Normal Mode** (Default): For navigating and deleting. You cannot type here.
2. **Insert Mode**: For typing text. Press **`i`** to enter.
3. **Command Mode**: For saving and quitting. Press **`:`** from Normal mode.

### 🛠️ The "Survival" Commands
* **`i`**: Start typing (Insert mode).
* **`Esc`**: Stop typing (Return to Normal mode).
* **`:w`**: Save (Write).
* **`:q!`**: Quit without saving (Discard changes).
* **`:wq`**: Save and quit.



---

## 🎙️ Part 2: Top 10 Priority Interview Q&A

| # | Question | Answer |
| :--- | :--- | :--- |
| 1 | **What is Vim?** | A command-line text editor used to edit files directly in the terminal. |
| 2 | **How do you start typing in Vim?** | Press **`i`** to enter Insert Mode. |
| 3 | **How do you save a file?** | Press `Esc`, then type **`:w`** and hit Enter. |
| 4 | **How do you quit without saving?** | Press `Esc`, then type **`:q!`** and hit Enter. |
| 5 | **How do you delete a whole line?** | In Normal Mode, press **`dd`**. |
| 6 | **How do you undo a mistake?** | In Normal Mode, press **`u`**. |
| 7 | **How to jump to the end of a file?** | In Normal Mode, press **`G`** (Shift+g). |
| 8 | **How to jump to the beginning?** | In Normal Mode, press **`gg`**. |
| 9 | **Why use Vim instead of a GUI editor?** | It allows you to edit files on remote servers where no mouse is available. |
| 10 | **How do you search for a word?** | In Normal Mode, type **`/`** followed by the word. |

---

## 🛠️ Part 3: Hands-on Practice Challenge
Run these steps in your terminal right now to practice:
1. **Create a file**: `vim practice.txt`
2. **Enter Insert Mode**: Press `i`.
3. **Type something**: "DevOps is about automation."
4. **Exit Insert Mode**: Press `Esc`.
5. **Save and Quit**: Type `:wq` and hit Enter.
6. **Verify**: `cat practice.txt`
