Build a simple Sudoku solver using backtracking in Python.
# Sudoku Solver

This is a Python code that solves a Sudoku puzzle using a backtracking algorithm. The Sudoku puzzle is represented as a 9x9 grid, where the empty cells are represented by 0.

The code consists of two main functions:

## `is_valid_move(grid, row, col, number)`

This function checks if a given number can be placed at the specified position (row, col) in the grid without violating the Sudoku rules. It checks for conflicts in the same row, same column, and the same 3x3 subgrid.

**Parameters:**
- `grid`: The Sudoku grid represented as a 9x9 list of lists.
- `row`: The row index of the cell to be checked.
- `col`: The column index of the cell to be checked.
- `number`: The number to be placed in the cell.

**Returns:**
- `True` if the number can be placed at the specified position without conflicts.
- `False` otherwise.

## `solve(grid, row, col)`

This function solves the Sudoku puzzle using a recursive backtracking algorithm. It starts at the given position (row, col) and tries to fill in the remaining cells with valid numbers.

**Parameters:**
- `grid`: The Sudoku grid represented as a 9x9 list of lists.
- `row`: The current row being processed.
- `col`: The current column being processed.

**Returns:**
- `True` if a solution is found for the Sudoku puzzle.
- `False` if no solution is found.

**Note:** The `solve` function modifies the `grid` in-place to fill in the numbers.

## Usage

To use the Sudoku solver, you can create a Sudoku grid as a 9x9 list of lists, where empty cells are represented by 0. Then, call the `solve` function with the grid and the initial position (0, 0). If a solution is found, the solved grid will be printed. Otherwise, a message indicating no solution will be displayed.

id if a solution is found, or a message indicating no solution if no valid solution exists for the given puzzle.
