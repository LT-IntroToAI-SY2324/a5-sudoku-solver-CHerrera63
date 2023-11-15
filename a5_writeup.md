# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

A: DFS is more quicker and gives less iterations, while BFS is not as quick and gives a lot of iterations, which makes DFS more preferable in Sudoku. BFS would be more preferebable if there were more categories, and more specific categories in sudoku, or anything else that has a very big and organized list. DFS might skip important things and not give a better outcome.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

A: It impacts how data is being applie into structures and how data is taken out. Example: with BFS, the last datapoint is the first/newest one added and the first datapoint is the last/oldest one out. Another alternative could be to go row by row, horizontally, instead of focusing on one column. It may or may not work, but it is a possibility.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

A: It can be adapted by adding the new things onto stacks/queues. The size of the puzzles would also need to be implemented to the solver to make sure it stops in the size of the puzzle, and not of one that was either smaller or bigger than the other one. This can be applied in the workforce, like in an office, and being able to find folders or important documents by following the patterns of DFS/BFS.
