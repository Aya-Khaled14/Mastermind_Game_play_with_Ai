# Mastermind Solver Game 

## Project Description

The **Mastermind Solver** is a Python-based implementation of the classic code-breaking game **Mastermind**, where the computer attempts to guess the player’s secret code. The game features an interactive GUI built using Tkinter, allowing players to provide feedback about the computer's guesses until the code is cracked or attempts are exhausted.

---

## Features

### Gameplay Mechanics
- **Computer as the Solver**: The computer makes educated guesses to deduce the player's secret 4-digit code, consisting of numbers from 1 to 6.
- **Feedback-Based Guessing**:
  - **Correct Positions**: The number of digits in the correct position.
  - **Correct Numbers**: The number of correct digits but in the wrong position.
- **Attempts**: The computer has a maximum of 10 attempts to guess the code.

### User Interaction
- **Graphical Interface**:
  - Interactive fields for feedback input.
  - Buttons for controlling game flow, including feedback submission and verifying the current guess.
- **Feedback System**:
  - Players provide feedback after each guess using two input fields for "correct positions" and "correct numbers."
- **Real-Time Updates**:
  - A detailed output box logs the computer's guesses and feedback history.

### Visual and Usability Enhancements
- **Clean Interface**: Intuitive layout with clear instructions and user-friendly design.
- **Error Handling**:
  - Validates player feedback inputs.
  - Alerts users if no possible guesses remain due to invalid feedback.
- **Victory Detection**:
  - Displays a success message if the computer cracks the code.
  - Ends the game if all attempts are exhausted without success.

---

## How to Play
1. **Start the Game**:
   - Click the "Start" button to begin. The computer will make its first guess.
2. **Provide Feedback**:
   - Enter the number of correct positions and correct numbers in the respective fields.
   - Click "Submit Feedback" after each guess.
3. **Right Guess**:
   - If the computer guesses the correct code, confirm by clicking "Is it the right guess?".
4. **Game Over**:
   - The game ends after 10 attempts or when the correct code is guessed.

---

## Technologies Used
- **Python**: For logic and application flow.
- **Tkinter**: For creating the graphical user interface.

---

## Code Logic
1. **Combination Generation**:
   - Generates all possible 4-digit combinations (1-6) for efficient guessing.
2. **Feedback Matching**:
   - Filters possible guesses based on the feedback provided by the player.
3. **Heuristic Guessing**:
   - Randomly selects the next guess from the filtered possibilities.
4. **Victory Detection**:
   - Stops the game when feedback indicates all 4 digits are in the correct position.

---

## Controls and UI Elements
- **Start Button**: Begins the guessing process.
- **Feedback Inputs**:
  - **Correct Positions**: Enter the number of digits in the correct positions.
  - **Correct Numbers**: Enter the number of correct digits in incorrect positions.
- **Submit Feedback**: Processes the player's feedback and provides the next guess.
- **Is it the Right Guess?**: Confirms that the computer’s guess is correct.

---

## How to Run
1. Install Python if not already installed.
2. Save the code to a file named `mastermind_solver.py`.
3. Run the script:
   ```bash
   python mastermind_solver.py
