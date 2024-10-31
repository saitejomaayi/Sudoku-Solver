# Sudoku-Solver

Implementation: Advanced Algorithms, DataStructures in Python and Numpy <br />

Sudoku(9X9) is an interesting puzzle where digits from 1-9 are partially pre-filled in a 9X9 array. The grid should be completed in such a way that no digit from 1 to 9 is repeated within any of the 9 individual 3X3 boxes and in the entire row and column.<br />
Another variation is 16X16 Sudoku puzzle. The numbers range from 1-16 with 4X4 grids. The grid should be completed in such a way that no digit from 1 to 16 is repeated within any of the 16 individual 4X4 boxes and in the entire row and column. <br />
Since solving Sudoku involves large search space and computa5on intensity, different approaches and algorithms are explored to find efficient solu5ons to the puzzles.<br />

All possible choices of numbers are to be checked to find the solution for Sudoku. Backtracking algorithm, which is an extension to the brute force technique is used to find all solutions incrementally to the problem.<br />
Structure of the solver: Input-> Data Structure-> Constraint Checker -> Algorithm-> Output<br />
Let N= no.of permitted values in the cell (9/16)<br />
Let M=no.of cells = N*N = 9*9 , 16*16 = 81 , 256<br />
Probability of values in each cell = N<br />
Total probability of values to be checked to solve the puzzle = N^M<br />
For 9X9 Sudoku there are 9 grids and 81 cells. For 16X16 Sudoku there are 16 grids and 256 cells .The worst case time complexity of Sudoku is equal to the number of possible board configurations which is 9^81and 16^256 respectively (O(N^M)).<br />
We explore and implement different algorithms and approaches like Linear programming and least possible values heuristic to solve Sudoku puzzles to optimize and improve the efficiency of the solver by reducing the search space and provide early identification of the solution.<br />
Proposed Algorithms:<br />
• Backtracking<br />
• PuLP<br />
• MRV (Minimum RemainingValues)<br />

Backtracking Algorithm:<br />
The classic algorithm that approaches a problem recursively to solve it and eliminating solutions that fail to solve.<br />
<br />

PuLP Algorithm:<br />
Sudoku can also be solved using linear programming (LP) method which largely uses Python syntax with many industry-standard solvers.<br />
<br />

MRV(Minimum Remaining Value) Algorithm:<br />
The MRV (Minimum Remaining Values) heuristic is often used in combination with backtracking algorithms to efficiently solve constraint based problems like Sudoku.<br />
