# CMP 131 – Python Programming


> **Required file location:** Keep every Python file directly in the repository root. Do not create a `src` folder.

## Week 10 – Lab 1: Functions, Input Validation, and Random Choices

**Total Points: 100**

* Program 1: Days Out — 50 points
* Program 2: Rock, Paper, Scissors — 50 points

## Learning Objectives

After completing this lab, students should be able to:

* Organize a Python program using a `main()` function.
* Define and call functions.
* Pass arguments to functions.
* Receive information through function parameters.
* Return integer, floating-point, and string values from functions.
* Use loops to collect and process repeated input.
* Validate numeric and text input.
* Use an accumulator to calculate a total.
* Calculate and format an average.
* Generate random numbers using Python’s `random` module.
* Use conditional statements to determine a winner.
* Repeat a game when a tie occurs.
* Test programs using valid and invalid inputs.
* Use comments to explain major program sections.

## Assignment Overview

Create two separate Python programs demonstrating functions, loops, input validation, conditional statements, and returned values.

The programs will:

1. Calculate the average number of days a company’s employees were absent.
2. Allow the user to play Rock, Paper, Scissors against the computer.

Create the following Python files:

* `days_out.py`
* `rock_paper_scissors.py`

The instructor is not providing completed Python code or an exact output design. Students must design, write, and test their own programs.

# Program 1: Days Out

**Points: 50**

## Program Description

Create a program that calculates the average number of days a company’s employees were absent during the past year.

The program must:

* Ask for the number of employees.
* Ask how many days each employee missed.
* Calculate the total number of days missed.
* Calculate the average number of days missed per employee.
* Display a clearly formatted absence summary.

The program must be divided into functions.

## Required Python File

Create a Python file named:

`days_out.py`

Include a comment header containing:

* Student name
* Course number
* Week number
* Lab number
* Assignment title
* Date

## Part 1: Create the `get_number_of_employees` Function

Create a function named:

`get_number_of_employees`

This function must:

* Accept no arguments.
* Ask the user to enter the number of employees in the company.
* Convert the input to an integer.
* Validate the number of employees.
* Return the valid number of employees as an integer.

The company must have at least one employee.

If the user enters a number less than `1`, the function must:

* Display an appropriate error message.
* Ask for the number of employees again.
* Continue until a valid value is entered.

## Part 2: Create the `get_total_days_absent` Function

Create a function named:

`get_total_days_absent`

This function must:

* Accept the number of employees as an argument.
* Use a loop to ask for the number of days each employee missed.
* Clearly identify the employee in each input prompt.
* Convert each entry to an integer.
* Validate every entered value.
* Add the valid number of missed days to an accumulator.
* Return the total number of days absent as an integer.

For example, if there are three employees, the prompts should clearly request the missed days for:

* Employee 1
* Employee 2
* Employee 3

The number of days missed:

* May be zero.
* Must not be negative.

If the user enters a negative value:

* Display an appropriate error message.
* Reject the value.
* Ask for the missed days for that employee again.
* Do not add the negative value to the accumulator.

## Part 3: Create the `calculate_average_days_absent` Function

Create a function named:

`calculate_average_days_absent`

This function must accept two arguments:

* Number of employees
* Total number of days absent

The function must:

* Calculate the average number of days absent.
* Return the average as a floating-point value.
* Perform no user input.
* Perform no screen output.

Use the following calculation:

**Average days absent = Total days absent ÷ Number of employees**

This function must only perform the calculation and return the result.

## Part 4: Create the `main` Function

Create a `main()` function that controls the program.

The `main()` function must:

* Display a descriptive program title.
* Call `get_number_of_employees`.
* Store the returned number of employees.
* Pass the number of employees to `get_total_days_absent`.
* Store the returned total number of absent days.
* Pass the employee count and total absent days to `calculate_average_days_absent`.
* Store the returned average.
* Display the final company absence summary.

Call `main()` to begin the program.

## Part 5: Display the Absence Summary

Display a clearly formatted summary containing:

* Number of employees
* Total number of days absent
* Average number of days absent per employee

Display the average with exactly two digits after the decimal point.

The output should have a structure similar to:

```text
EMPLOYEE ABSENCE SUMMARY

Number of employees:          3
Total days absent:            6
Average days per employee: 2.00
```

Students may create their own output design, but all required information must be clearly labeled.

## Required Testing for Program 1

### Test 1: Three Employees

Use the following information:

|   Employee | Days Absent |
| ---------: | ----------: |
| Employee 1 |           2 |
| Employee 2 |           0 |
| Employee 3 |           4 |

Expected results:

* Number of employees: `3`
* Total days absent: `6`
* Average days absent: `2.00`

### Test 2: Four Employees

Use the following information:

|   Employee | Days Absent |
| ---------: | ----------: |
| Employee 1 |           0 |
| Employee 2 |           1 |
| Employee 3 |           3 |
| Employee 4 |           2 |

Expected results:

* Number of employees: `4`
* Total days absent: `6`
* Average days absent: `1.50`

### Test 3: No Absences

Use three employees and enter `0` days absent for every employee.

Expected results:

* Total days absent: `0`
* Average days absent: `0.00`

### Test 4: Invalid Number of Employees

First enter:

`0`

The program must display an error message and ask for the number of employees again.

Then enter:

`3`

The program must accept the new value and continue.

Also test a negative number of employees.

### Test 5: Invalid Number of Absent Days

First enter:

`-2`

The program must:

* Display an error message.
* Reject the negative value.
* Ask for that employee’s absent days again.

Then enter:

`2`

The program must accept the new value and continue.

## Program 1 Point Distribution

* Program title and complete comment header: 4 points
* Correct `main()` function organization: 5 points
* Correct `get_number_of_employees` function: 7 points
* Employee-count validation: 5 points
* Correct `get_total_days_absent` function: 8 points
* Loop, accumulator, and absent-days validation: 8 points
* Correct `calculate_average_days_absent` function: 6 points
* Correct function calls, arguments, and returned values: 4 points
* Clear output formatting and successful testing: 3 points

**Program 1 Total: 50 points**

# Program 2: Rock, Paper, Scissors

**Points: 50**

## Program Description

Create a program that allows the user to play Rock, Paper, Scissors against the computer.

At the beginning of each round, the computer must randomly choose:

* Rock
* Paper
* Scissors

The computer’s choice must remain hidden until after the user enters a choice.

The program must then:

* Display the computer’s choice.
* Compare the two choices.
* Determine the winner.
* Display the result.
* Play another round if the choices are the same.

The program must be divided into functions that perform the major tasks.

## Required Python File

Create a Python file named:

`rock_paper_scissors.py`

Include a comment header containing:

* Student name
* Course number
* Week number
* Lab number
* Assignment title
* Date

## Part 1: Import the Random Module

Import Python’s `random` module.

Use it to generate a random integer from `1` through `3`, including both endpoints.

Use the following mapping:

| Random Number | Computer Choice |
| ------------: | --------------- |
|             1 | Rock            |
|             2 | Paper           |
|             3 | Scissors        |

## Part 2: Create the `get_computer_choice` Function

Create a function named:

`get_computer_choice`

This function must:

* Accept no arguments.
* Generate a random number from `1` through `3`.
* Convert the random number to the corresponding game choice.
* Return `"rock"`, `"paper"`, or `"scissors"`.

The function must not display the computer’s choice.

The choice must remain hidden until the user has entered a choice.

## Part 3: Create the `get_user_choice` Function

Create a function named:

`get_user_choice`

This function must:

* Accept no arguments.
* Ask the user to enter `rock`, `paper`, or `scissors`.
* Remove unnecessary spaces from the beginning and end of the entry.
* Convert the entry to lowercase.
* Validate the user’s choice.
* Return the valid choice as a string.

If the user enters anything other than `rock`, `paper`, or `scissors`, the function must:

* Display an appropriate error message.
* Ask the user to enter another choice.
* Continue until a valid choice is entered.

The program should accept capitalization differences such as:

* `Rock`
* `ROCK`
* `rock`

## Part 4: Create the `determine_winner` Function

Create a function named:

`determine_winner`

This function must accept two arguments:

* User’s choice
* Computer’s choice

The function must compare the choices and return a result indicating:

* The user won.
* The computer won.
* The round was a tie.

Apply the following rules:

* Rock defeats scissors because rock smashes scissors.
* Scissors defeat paper because scissors cut paper.
* Paper defeats rock because paper wraps rock.
* Matching choices create a tie.

The function should determine and return the result. It should not ask the user for input.

## Part 5: Create the `main` Function

Create a `main()` function that controls the game.

The `main()` function must:

* Display a descriptive game title.
* Generate the computer’s choice.
* Keep the computer’s choice hidden.
* Ask for the user’s choice.
* Display both choices after the user enters a valid choice.
* Call `determine_winner`.
* Display an appropriate result message.
* Repeat the game when a tie occurs.
* Stop when either the user or computer wins.

Call `main()` to begin the program.

## Part 6: Handle a Tie

If the computer and user make the same choice:

* Display a message explaining that the round is a tie.
* Generate a new computer choice.
* Ask the user for another choice.
* Compare the new choices.
* Continue until the game has a winner.

Do not end the program immediately after a tie.

The computer must generate a new random choice for every new round.

## Part 7: Display the Game Result

After the user has entered a valid choice, display:

* User’s choice
* Computer’s choice
* Result of the round

When appropriate, include an explanation such as:

* Rock smashes scissors.
* Scissors cut paper.
* Paper wraps rock.
* Both players selected the same choice.

Students may create their own output design, but the result must be clear.

## Required Testing for Program 2

Because the computer’s choice is random, run the program multiple times and verify the following outcomes.

| User Choice | Computer Choice | Expected Result |
| ----------- | --------------- | --------------- |
| Rock        | Scissors        | User wins       |
| Rock        | Paper           | Computer wins   |
| Paper       | Rock            | User wins       |
| Paper       | Scissors        | Computer wins   |
| Scissors    | Paper           | User wins       |
| Scissors    | Rock            | Computer wins   |
| Rock        | Rock            | Tie             |
| Paper       | Paper           | Tie             |
| Scissors    | Scissors        | Tie             |

### Input-Validation Testing

Test the following invalid entries:

* `stone`
* `r`
* An empty entry
* A number such as `2`

For every invalid entry, confirm that:

* An error message is displayed.
* The entry is rejected.
* The user is asked to enter another choice.

### Capitalization Testing

Test the following entries:

* `Rock`
* `PAPER`
* `sCiSsOrS`

Confirm that the program accepts all three entries.

### Tie Testing

Continue running the program until a tie occurs.

Confirm that:

* The tie is displayed.
* The program does not end.
* A new computer choice is generated.
* The user is asked to play another round.
* The game continues until a winner is determined.

## Program 2 Point Distribution

* Program title and complete comment header: 4 points
* Correctly import and use the `random` module: 5 points
* Correct `get_computer_choice` function: 7 points
* Correct `get_user_choice` function: 6 points
* User-choice validation and capitalization handling: 5 points
* Correct `determine_winner` function: 10 points
* Correct game rules and result messages: 5 points
* Correct tie-handling loop: 5 points
* Clear output, comments, and successful testing: 3 points

**Program 2 Total: 50 points**

# Function Requirements

Both programs must:

* Include a `main()` function.
* Call `main()` to begin the program.
* Use the exact required function names.
* Pass information using arguments when required.
* Receive information using parameters.
* Return values to the calling function.
* Store or appropriately use returned values.
* Keep each function focused on one major task.
* Avoid using global variables to transfer information between functions.

# Code Comments

Use comments to identify and explain the major sections of both programs.

Include comments for:

* Program information header
* Module imports
* Function definitions
* Parameters and returned values
* Main function
* User input
* Input validation
* Loop processing
* Accumulator processing
* Random-choice generation
* Conditional statements
* Calculations
* Function calls
* Tie handling
* Final output

Comments should briefly explain the purpose of each major section. They should not repeat every Python statement word for word.

# General Requirements

* Use Python to complete both programs.
* Create both required Python files.
* Use the exact required filenames.
* Use the exact required function names.
* Include and call a `main()` function in both programs.
* Use meaningful and consistent variable names.
* Convert user input to the appropriate data type.
* Validate all required input.
* Use loops where required.
* Use parameters, arguments, and returned values correctly.
* Do not use global variables to transfer information between functions.
* Include a complete comment header in both files.
* Include comments explaining the major program sections.
* Use clear prompts, headings, labels, and result messages.
* Test both programs using all required test cases.
* Check spelling, capitalization, grammar, and punctuation.
* Make sure both programs run without errors.
* Follow the course AI-use policy.
* Record any AI assistance in `AI-Use-Report.md`.

# Required Organization

Organize the assignment as follows:

* `Week-10`

  * `Lab-01`

    * `CMP131-Week-10-Lab-01.md`
    * `AI-Use-Report.md`
    * `src`

      * `days_out.py`
      * `rock_paper_scissors.py`

# Submission Requirements

Submit or push the complete `Lab-01` folder.

The submission must include:

* `days_out.py`
* `rock_paper_scissors.py`
* `AI-Use-Report.md`

Before submitting, verify that:

* Both required Python files are included.
* Both filenames are correct.
* Both programs contain a complete comment header.
* Both programs include and call a `main()` function.
* All required functions are correctly defined.
* Function names are spelled and capitalized correctly.
* Arguments and parameters are used correctly.
* Required functions return the correct values.
* The Days Out program accepts at least one employee.
* Invalid employee counts are rejected.
* Negative absent-day values are rejected.
* The total number of absent days is calculated correctly.
* The average is calculated correctly.
* The average displays two decimal places.
* The Rock, Paper, Scissors program generates random choices.
* The computer’s choice remains hidden until the user enters a choice.
* Invalid user choices are rejected.
* All game-winning combinations work correctly.
* A tied game repeats.
* A new computer choice is generated after a tie.
* Both programs were tested using the required values.
* Both programs run without errors.
* The AI-use report is complete.
* The latest work has been committed and pushed to GitHub.

# Suggested Git Commit Messages

* Create Week 10 Lab 1 Python files
* Add employee-count function and validation
* Add employee absence input loop
* Calculate total and average days absent
* Test Days Out functions
* Add random computer-choice function
* Add Rock Paper Scissors user input
* Add game-choice validation
* Add winner-selection function
* Add tie-handling loop
* Test all game outcomes
* Improve comments and output formatting
* Complete Week 10 Python lab

---

## GitHub Starter Repository

Use the following public starter repository:

[CMP131-Week-10-Lab-01](https://github.com/ahedhli12/CMP131-Week-10-Lab-01)

### Getting Started

1. Open the starter repository using the link above.
2. Select **Use this template → Create a new repository** when the template option is available.
3. Choose your personal GitHub account as the owner.
4. Name your repository `LastName-FirstName-CMP131-Week-10-Lab-01`.
5. Set your repository to **Public**.
6. Clone your own newly created repository—not the instructor’s starter repository.
7. Open the entire cloned folder in Visual Studio Code.
8. Complete and test every required Python file.
9. Commit and push your work to GitHub.
10. Verify that your latest files appear on GitHub.
11. Complete `AI-Use-Report.md`.
12. Submit the required work through Blackboard Ultra and include your public repository link when requested.

### Required Repository Files

- `CMP131-Week-10-Lab-01.md`
- `AI-Use-Policy.md`
- `AI-Use-Report.md`
- `days_out.py`
- `rock_paper_scissors.py`

### Before You Submit

- [ ] All required Python files are in the repository root.
- [ ] Every required filename is exact.
- [ ] Each program runs successfully.
- [ ] Required tests and screenshots are complete.
- [ ] `AI-Use-Report.md` is complete and accurate.
- [ ] The latest commit is visible on GitHub.
