# 🪙 Head or Tail Game

A beginner-friendly Python command-line game where the player chooses **Head** or **Tail**, and the computer randomly generates an outcome. The program compares the two choices and displays whether the player wins.

## ✨ Features

- Simple text-based interaction.
- Uses Python's built-in `random` module to generate the computer's result.
- Compares the player's choice with the computer's output.
- Displays a win or try-again message.

## 🛠️ Requirements

- Python 3.x
- No third-party packages are required.

## 🚀 Getting Started

### 1. Save the code

Save the program in a file named `head_or_tail.py`.

### 2. Add the required import

The code uses `random.randint()`, so add this line at the beginning of the file:

```python
import random
```

### 3. Run the game

Open a terminal in the folder containing the file and run:

```bash
python head_or_tail.py
```

On some systems, you may need to use:

```bash
python3 head_or_tail.py
```

## 🎮 How to Play

1. Run the program.
2. Enter `Head` or `Tail` when prompted.
3. The computer generates an outcome.
4. The program compares your input with the computer's outcome and prints a result.

### Example Output

```text
Welcome to Head or Tail Game :
Choose between Head or Tail : Head
Your Choose : Head
Computer Output is : Tail
Try Again ! Computer output and You're Output Note match
```

The computer result is random, so your output may differ each time.

## ⚙️ How the Code Works

- `a = "Head"` and `b = "Tail"` store the two possible outcomes.
- `random.randint(0, 1)` generates an integer from `0` to `1`, inclusive.
- If the generated number is `1`, the computer chooses `Head`; otherwise, it chooses `Tail`.
- The program compares `computer_output` with `Choose` to determine the displayed result.

## ⚠️ Current Limitations

- **Uneven probabilities:** `random.randint(0, 1)` can generate `0`, `1`. Only `1` produces `Head`, while `0` produce `Tail`. Therefore, Head has a 1 in  chance and Tail has a 0 in chance.
- **Input is case-sensitive:** `head`, `HEAD`, or extra spaces will not match `Head` or `Tail` exactly.
- **Missing import in the snippet:** `import random` must be included before calling `random.randint()`.
- **Redundant final `else`:** The final `else: pass` is unnecessary because the preceding `if` and `elif` already cover all possible comparisons.
- **No input validation:** Any input other than the exact strings `Head` and `Tail` is treated as a non-match.

## 💡 Suggested Improvements

- Use `random.choice(["Head", "Tail"])` to give both outcomes an equal chance.
- Normalize user input with `.strip().capitalize()` so entries such as `head` are accepted.
- Add input validation and let the user play multiple rounds.

## 🧰 Technologies Used

- **Language:** Python
- **Interface:** Command-line interface (CLI)
- **Standard library:** `random`

## 👨‍💻 Author

**Ritu Raj**

## 📄 License

This project is provided for learning and practice. Add a license file if you plan to distribute it publicly.
