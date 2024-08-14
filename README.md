# Sudoku Solver

This repository contains a Sudoku solver implemented in Python using the numpy library.

## How to Use the Sudoku Solver

### Step 1: Install Required Library

Make sure you have the numpy library installed. If you haven't installed it yet, you can do so using pip:

```bash
pip install numpy
```

### Step 2: Set Up the Puzzle
You can define your own Sudoku puzzles by modifying the puzzle variable. The puzzle should be a 9x9 grid, where empty cells are represented by 0. For example:
```bash
pythonCopypuzzle = [
    [0, 0, 0, 0, 0, 0, 0, 0, 6],
    [8, 6, 0, 0, 0, 0, 0, 5, 0],
    [4, 0, 0, 0, 0, 2, 0, 0, 8],
    [0, 0, 7, 0, 0, 0, 9, 1, 0],
    [0, 0, 2, 4, 0, 0, 0, 0, 0],
    [0, 5, 0, 0, 0, 1, 0, 0, 0],
    [0, 0, 0, 6, 8, 4, 0, 0, 0],
    [0, 0, 0, 0, 5, 0, 3, 0, 0],
    [0, 0, 0, 0, 2, 0, 5, 0, 7]
]
```
### Step 3: Run the Solver
Once you have defined your puzzle, simply run the script. The iterate() function will be called, which will attempt to solve the Sudoku puzzle. If a solution is found, it will be printed in a matrix format.

### Notes:
**Backtracking Algorithm:** The iterate() function uses a backtracking approach to fill in the Sudoku puzzle. It tries to place numbers from 1 to 9 in each empty cell and checks if the placement is valid using the valid() function.
Output: If a solution is found, the completed Sudoku grid will be printed in the console. If the puzzle is unsolvable, the program will terminate without outputting a solution.
