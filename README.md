# Crossword Puzzle Generator

This project is an AI-based crossword puzzle generator that uses constraint satisfaction techniques to solve crossword puzzles. The program takes a crossword structure and a list of words as input and attempts to fill the crossword grid with the given words while satisfying all constraints.

---

## Features

- **Constraint Satisfaction Problem (CSP) Solver**: Implements techniques like node consistency, arc consistency (AC3), and backtracking search.
- **Heuristics**: Uses Minimum Remaining Values (MRV), Degree Heuristic, and Least Constraining Value (LCV) to optimize the solving process.
- **Customizable Inputs**: Accepts user-defined crossword structures and word lists.
- **Output Options**: Prints the solution to the terminal and optionally saves it as an image file.

---

## How It Works

1. **Input Files**:
   - **Structure File**: Defines the crossword grid using `_` for blank spaces and `#` for blocked cells.
   - **Words File**: Contains a list of words to be used in the crossword puzzle.

2. **Solving Process**:
   - The program enforces node consistency to ensure words fit the variable lengths.
   - Arc consistency is enforced using the AC3 algorithm to eliminate conflicts between overlapping variables.
   - Backtracking search is used to assign words to variables while satisfying all constraints.

3. **Output**:
   - If a solution is found, the crossword is printed to the terminal.
   - Optionally, the solution can be saved as an image file.

