# suduko-solver-

Language used: C++.

Method used: Backtracking.

Approach: Like all other Backtracking problems, Sudoku can be solved by one by one assigning numbers to empty cells. Before assigning a number, check whether it is safe to assign. Check that the same number is not present in the current row, current column and current 3X3 subgrid. After checking for safety, assign the number, and recursively check whether this assignment leads to a solution or not. If the assignment doesn’t lead to a solution, then try the next number for the current empty cell. And if none of the number (1 to 9) leads to a solution, return false and print no solution exists.

Functions used:

FindUnassignedLocation(): This function finds an entry in grid that is still unassigned.

SolveSudoku(): Takes a partially filled-in grid and attempts to assign values to all unassigned locations in such a way to meet the requirements for Sudoku solution.

UsedInRow():Returns a boolean which indicates whether an assigned entry in the specified row matches the given number.

UsedInCol(): Returns a boolean which indicates whether an assigned entry in the specified column matches the given number.

UsedInBox(): Returns a boolean which indicates whether an assigned entry within the specified 3x3 box matches the given number.

isSafe(): Checks whether it will be legal to assign num to the given row, col

printGrid(): A utility function to print grid.
