# Sudoku-solver

- Implemented a Depth-first search backtracking algorithm with constraint propagation.

    Given that there are tens of thousands of possible solution patterns of sudokus, this algorithm has a linear space complexity and thus it
    has lower memory requirements. In comparison, a breadth-first search algorithm would have an undesirable
    exponential space complexity and therefore the more blank squares there are in the sudoku, the larger amount of
    memory will be required of the algorithm to find a solution. Although this DFS algorithm might struggle with
    execution time compared to other algorithms, it still does not perform worse than a BFS, and it cannot get stuck
    into a local minimum similar to a local search.

- Improved execution time by updating singleton cells, whenever they appear during the DFS execution.

    An optimisation to the algorithm implemented is the update of singleton cells on the grid,
    whenever they appear during the DFS execution. Although it does not change the time or space complexity of the
    algorithm, it significantly reduces the time that the algorithm needs to solve a sudoku given that the closer the
    partial state is to the goal state, the more occurrences of singleton cells will appear, which would decrease runtime.
