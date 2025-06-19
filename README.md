

---

# ✊✋✌️ Rock Paper Scissors Game

A simple **Rock Paper Scissors** game implemented in Python — perfect for beginners learning input/output, conditionals, and basic logic!
This version runs easily in **Google Colab**, making it accessible for anyone to play and tweak.

## 📌 Features

* Play Rock, Paper, Scissors against the computer.
* Random computer choices.
* Clear game outcome messages.
* Beginner-friendly, clean Python code.

## 🛠️ How to Run

1. Open [Google Colab](https://colab.research.google.com/).
2. Copy the Python code from [`rock_paper_scissors.py`](./rock_paper_scissors.py) (or this README).
3. Paste it into a new Colab notebook cell.
4. Run the cell and follow the prompts to play!

## 🧑‍💻 Code Example

```python
import random

def get_choices():
    player_choice = input("Enter a choice (rock, paper, scissors): ")
    options = ["rock", "paper", "scissors"]
    computer_choice = random.choice(options)
    choices = {"player": player_choice, "computer": computer_choice}
    return choices

def check_win(player, computer):
    print(f"You chose {player}, computer chose {computer}")
    if player == computer:
        return "It's a tie!"
    elif player == "rock":
        if computer == "scissors":
            return "Rock smashes scissors! You win!"
        else:
            return "Paper covers rock! You lose."
    elif player == "paper":
        if computer == "rock":
            return "Paper covers rock! You win!"
        else:
            return "Scissors cuts paper! You lose."
    elif player == "scissors":
        if computer == "paper":
            return "Scissors cuts paper! You win!"
        else:
            return "Rock smashes scissors! You lose."

choices = get_choices()
result = check_win(choices["player"], choices["computer"])
print(result)
```

## 🙏 Acknowledgement

This simple project was inspired by the **"Python for Beginners – Full Course"** available for free on [YouTube - freeCodeCamp](https://www.youtube.com/watch?v=rfscVS0vtbw).
A huge thanks to freeCodeCamp for providing high-quality, free educational content.

## 📄 License

This project is for educational purposes. Feel free to fork, modify, and learn!

---
