# CMP 131 – Python Programming

> **Required file location:** Keep every Python file directly in the repository root. Do not create a `src` folder.

## Week 10 – Lab 1: Functions, Input Validation, and Random Choices

**Total Points: 100**

- Program 1: Days Out — 50 points
- Program 2: Rock, Paper, Scissors — 50 points

## Learning Objectives

After completing this lab, students should be able to:

- Organize a program using a `main()` function.
- Define and call functions.
- Pass arguments and use parameters.
- Return integer, floating-point, and string values.
- Use loops to collect repeated input.
- Validate numeric and text input.
- Use an accumulator and calculate an average.
- Generate random numbers using Python's `random` module.
- Use conditional statements to determine a winner.
- Repeat a game when a tie occurs.
- Test programs using valid and invalid inputs.

## Assignment Overview

Create two separate Python programs:

1. `days_out.py` — calculate the average number of days a company's employees were absent.
2. `rock_paper_scissors.py` — allow the user to play Rock, Paper, Scissors against the computer.

The instructor is not providing completed Python code or an exact output design. Students must design, write, and test their own programs.

# Program 1: Days Out

**Points: 50**

Create `days_out.py`.

Your program must:

- Display a descriptive title.
- Ask for the number of employees.
- Reject an invalid employee count and ask again.
- Ask how many days each employee missed.
- Reject negative days missed and ask again.
- Use a loop to collect the days missed for every employee.
- Use an accumulator to calculate the total days missed.
- Calculate the average days missed per employee.
- Display the total and average clearly.
- Organize the work into functions rather than placing everything in one section.
- Use a `main()` function to coordinate the program.

Use functions appropriate to the assignment for tasks such as obtaining a valid employee count, collecting or totaling days missed, and calculating the average.

Test the program with different employee counts, including invalid input and at least one employee with zero days missed.

# Program 2: Rock, Paper, Scissors

**Points: 50**

Create `rock_paper_scissors.py`.

The program must allow a user to play against the computer.

Your program must:

- Import Python's `random` module.
- Generate a random computer choice representing Rock, Paper, or Scissors.
- Ask the user for a valid Rock, Paper, or Scissors choice.
- Validate the user's entry.
- Use functions to organize the program.
- Compare the user and computer choices.
- Determine whether the user wins, the computer wins, or the round is a tie.
- Display both choices and the result.
- If the round is a tie, repeat the game until there is a winner.
- Use a `main()` function to coordinate the program.

Use the standard rules:

- Rock beats Scissors.
- Scissors beats Paper.
- Paper beats Rock.
- Matching choices produce a tie.

Test every possible winning relationship and confirm that a tie causes another round.

# Code Comments

Each Python file must include a comment header containing:

- Student name
- Course number
- Week number
- Lab number
- Assignment title
- Date

Use comments to explain major sections such as function definitions, input validation, loops, calculations, random selection, winner determination, and final output.

# General Requirements

- Use meaningful variable and function names.
- Use functions as required instead of writing one long program.
- Validate input appropriately.
- Keep both Python files directly in the repository root.
- Test both programs carefully.
- Make sure both programs run without errors.
- Follow `AI-Use-Policy.md`.
- Complete `AI-Use-Report.md` honestly.

# Submission Requirements

Your repository must include:

- `CMP131-Week-10-Lab-01.md`
- `days_out.py`
- `rock_paper_scissors.py`
- `AI-Use-Policy.md`
- `AI-Use-Report.md`

Before submitting:

1. Run and test both programs.
2. Confirm filenames are correct.
3. Confirm the Python files are in the repository root.
4. Complete the AI-use report.
5. Commit and push your latest work.
6. Verify the newest files on GitHub.
7. Submit through Blackboard Ultra as directed.

**Do not push your work to the instructor's starter repository.**
