# Assignment 3: Shipping Cost Calculator

## Description

In this assignment, you will design and implement a Python program that calculates the cost of shipping a package based on its weight and shipping distance.

Unlike Assignment 2, you will not be given a step-by-step development sequence or prescribed Git commit messages. You are now responsible for deciding how to break the problem into meaningful stages, when to test your work, and when a coherent unit of development is ready to commit.

The primary programming concepts in this assignment are:

- values and data types;
- variables and program state;
- expressions and arithmetic;
- input and output;
- Boolean expressions;
- decision-making with `if`, `elif`, and `else`;
- boundary conditions;
- validation; and
- systematic testing.

You will continue using Git, GitHub, Classroom 50, and generative AI as part of the development process.

## Learning Objectives

By completing this assignment, you should be able to:

- translate written requirements into a working program;
- select appropriate data types for program input;
- use expressions to perform calculations;
- create Boolean expressions that represent decision rules;
- use selection to implement multiple cases;
- reason correctly about boundary values;
- validate logically invalid input;
- test multiple execution paths;
- develop software incrementally using meaningful Git commits;
- use generative AI while independently understanding and verifying the resulting work; and
- document a small software project professionally.

## Background

Before beginning this assignment, you should have:

- completed **Assignment 1: Getting Started**;
- completed **Assignment 2: First Code**;
- watched the [video on programming with AI](https://youtu.be/CHhfy3fAMaA) and followed along with [the presentation](https://katrompas.accprofessors.com/assets/notes/Using_AI_effectively.pdf);
- reviewed the [Best Practices for Procedural Programming](https://katrompas.accprofessors.com/best-practice-procedural-programming) and identified the guidelines that apply to the programming concepts introduced so far;
- a working Python 3 development environment;
- Git and GitHub configured and working;
- completed the Introduction to Programming material; and
- completed the first Boolean Logic and Decision-Making material.

Assignment 2 walked you through the course development workflow in detail. Beginning with this assignment, you are expected to apply that workflow more independently.

## Starter Repository

Your repository initially contains:

```text
ASSIGNMENT.md
main.py
README.md
ESSAY.md
.gitignore
```

The supplied `main.py` contains the basic structure for the program:

```python
# don't forget your comment header here


def main():
    # don't forget your function header here

    # Erase the pass and write your program here
    pass


if __name__ == "__main__":
    main()
```

Write your program inside `main()` by replacing the `pass` statement.

Do not remove the supplied `main()` structure.

## Program Requirements

Write a program that calculates the shipping cost of a package.

The program must:

1. display the program title;
2. ask the user for the package weight in pounds;
3. ask the user for the shipping distance in miles;
4. accept integer or floating-point numeric input, such as `3`, `3.0`, or `3.33`;
5. validate that both weight and distance are greater than zero;
6. determine the correct shipping rate based on package weight;
7. calculate the shipping cost;
8. apply the minimum shipping charge when necessary; and
9. display the final shipping cost.

You may assume that the user enters numeric input. If the user enters nonnumeric input such as `dog`, the program may terminate with an error; handling that case is outside the scope of this assignment.

However, numeric values that are logically invalid, such as zero or a negative weight or distance, **must be detected and handled by the program**.

### Input

The program must ask for:

- package weight in pounds; and
- shipping distance in miles.

Weight and distance may contain decimal values.

Use the following prompts **exactly**:

```text
Enter package weight in pounds:
Enter shipping distance in miles:
```

Each input prompt should contain **one space** after the colon before the user's input.

### Validation

Both the package weight and shipping distance must be greater than zero.

If either value is less than or equal to zero, display:

```text
Error: weight and distance must be greater than zero.
```

When the input is invalid, the program must not calculate or display a shipping cost.

You may assume that the user enters numeric input. Handling nonnumeric input is not required for this assignment.

### Shipping Rates

The shipping rate is determined by package weight.

| Package Weight | Shipping Rate |
| --- | ---: |
| Up to and including 2 pounds | $0.05 per mile |
| Over 2 pounds through 10 pounds | $0.10 per mile |
| Over 10 pounds through 25 pounds | $0.15 per mile |
| Over 25 pounds | $0.20 per mile |

After determining the appropriate rate, calculate the shipping cost using the shipping distance.

### Minimum Shipping Charge

The minimum shipping charge is:

```text
$5.00
```

If the calculated shipping cost is less than $5.00, the final shipping cost must be $5.00.

### Output

The program must begin by displaying:

```text
Shipping Cost Calculator
```

For valid input, display the final shipping cost using exactly two digits after the decimal point.

For example:

```text
Shipping Cost Calculator
Enter package weight in pounds: 8
Enter shipping distance in miles: 120
Shipping cost: $12.00
```

A shipment whose calculated cost is below the minimum charge might produce:

```text
Shipping Cost Calculator
Enter package weight in pounds: 1
Enter shipping distance in miles: 20
Shipping cost: $5.00
```

For invalid input:

```text
Shipping Cost Calculator
Enter package weight in pounds: -2
Enter shipping distance in miles: 100
Error: weight and distance must be greater than zero.
```

**Note** that the program should read both input values before performing the validation described above.

The required prompts and output text are part of the program interface and should match the specification.

## Programming Constraints

Your solution should use programming concepts introduced in the course.

For this assignment, you should use concepts such as:

- variables;
- numeric data types;
- converting input into numeric types;
- arithmetic expressions;
- Boolean expressions;
- `if`;
- `elif`;
- `else`; and
- basic Boolean operators where appropriate.

The following are not needed for this assignment and should not be used:

- loops;
- additional user-defined functions;
- lists;
- dictionaries;
- exception handling;
- file input/output;
- external libraries.

Generative AI may suggest techniques that have not yet been introduced in the course. Do not use techniques outside the scope of this assignment simply because AI generated them. **You are responsible for understanding every part of the submitted program**.

You will also be evaluated on the readability, simplicity, structure, and quality of your code. A program that merely produces the correct output is not necessarily a good program.

Use AI to help you examine and improve your solution, but do not accept unnecessary complexity or techniques outside the scope of the course. Prefer clear, simple, well-structured code that you fully understand. The [best practices](https://katrompas.accprofessors.com/best-practice-procedural-programming) page will help.

## Development Process

Develop the program incrementally.

**Do not write the entire solution first** and then submit it as one completed commit.

Your repository history must contain **at least four meaningful student-created development commits** that show the program being built incrementally.

A meaningful commit represents a coherent improvement to the working program, not simply formatting or moving spaces around.

For example, a meaningful commit might represent completing a particular capability, correcting an important problem, or reaching another logical stage of development.

Each meaningful commit must also have a clear, descriptive commit message that follows the course [commit guidelines](https://katrompas.accprofessors.com/committing).

You are responsible for:

- deciding appropriate commit boundaries;
- writing your own descriptive commit messages;
- testing your work before committing;
- pushing your work regularly; and
- reviewing Classroom 50 feedback after pushes.

Commits that simply contain arbitrary portions of unfinished work solely to satisfy the required number of commits are not considered meaningful.

Changes made only to `README.md` or `ESSAY.md` do **not** count toward the four required program-development commits.

You may make more than four development commits. Four is the minimum, not the target.

## Generative AI

Use of generative AI is required as part of the development process.

You may use the generative AI system of your choice as a:

- tutor;
- programming partner;
- critic;
- debugging assistant;
- source of explanations; or
- aid in reasoning about the assignment.

You may show the AI the complete assignment and ask it to help you understand the requirements or develop the program.

AI may suggest or generate code. However, you remain responsible for:

- understanding all submitted code;
- understanding the conditions and calculations in your program;
- questioning AI output;
- testing AI suggestions;
- identifying incorrect assumptions;
- verifying boundary behavior; and
- making the final programming decisions.

Your use and verification of AI will be documented in `ESSAY.md`.

## Testing

Testing is part of the development process.

Do not test the program only once with a convenient input.

Your testing should exercise the different paths and important boundaries created by your decision logic.

At minimum, test cases should include:

- packages from each of the four weight categories;
- values slightly below, exactly at, and slightly above each weight boundary at 2, 10, and 25 pounds;
- a case in which the calculated shipping cost is below $5.00;
- a zero and a negative value for package weight;
- a zero and a negative value for shipping distance.

Think about what each test is intended to demonstrate before running it.

Classroom 50 will also test your program when you push your work. The autograder score represents **tests passed, not your assignment grade**.

Passing the available automated tests does not remove your responsibility to test and verify the program yourself.

## Code Documentation

Your program must follow the course [Commenting Guidelines](https://katrompas.accprofessors.com/commenting).

Update `main.py` so that it contains:

- the required file comment header; and
- the required function comment header for `main()`.

Follow the Python commenting example provided in the course guidelines.

Do not add unnecessary comments that merely restate obvious individual lines of code.

Before submission, remove:

- debugging statements;
- commented-out code;
- temporary code; and
- unnecessary comments.

## `README.md`

Complete the supplied `README.md` according to the course [README Guidelines](https://katrompas.accprofessors.com/readme-guidelines).

Your README should accurately document the program you actually submitted.

Complete all required sections and remove the instructional placeholder comments from the starter file.

All Markdown files must be properly formatted and professional. Spelling, grammar, and writing quality count.

## `ESSAY.md`

Complete the supplied `ESSAY.md`.

The file contains five questions concerning:

- your use of generative AI;
- your understanding of Boolean logic;
- boundary testing;
- verification of AI output; and
- your understanding of your own code.

Each question is worth **2 points**, for a total of **10 points**.

Answer each question clearly and specifically in your own words.

This is not a formal essay. Concise, substantive answers are preferred.

## Final Review and Submission

Before submitting the assignment, verify the complete repository.

### 1. Run the program

Run the program locally and test it one final time.

```bash
python3 main.py
```

Depending on your system configuration, the command may instead be:

```bash
python main.py
```

### 2. Check repository status

Run:

```bash
git status
```

Your working tree should be clean.

### 3. Review your development history

Run:

```bash
git log --oneline
```

Verify that your history contains at least four meaningful program-development commits and that the history reflects incremental development.

### 4. Review GitHub

Open the repository on GitHub and confirm that:

- your final `main.py` is present;
- your completed `README.md` is present;
- your completed `ESSAY.md` is present; and
- all final changes have been pushed.

### 5. Review Classroom 50

Review the final Classroom 50 autograding results and Feedback pull request.

Remember:

> **Autograder points represent tests passed, not the assignment grade.**

### 6. Submit through Blackboard

Copy the normal HTTPS URL for your GitHub repository and submit that URL in the Blackboard assignment.
