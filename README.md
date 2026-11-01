# Eight-Puzzle Solver: Uniform-Cost Search and A*

![Python](https://img.shields.io/badge/python-3-blue)
![Type](https://img.shields.io/badge/CS%20205%20Artificial%20Intelligence-UC%20Riverside-lightgrey)

The program solves the 3×3 sliding-tile puzzle optimally and compares how much search each algorithm needs to find the solution.

*Project 1 for CS 205 (Artificial Intelligence), UC Riverside. The write-up is in [`CS_205_Project-1_Report.pdf`](CS_205_Project-1_Report.pdf).*

## Algorithms

| Algorithm | Heuristic h(n) | Notes |
|---|---|---|
| Uniform-cost search | h(n) = 0 | Optimal but expands the most nodes |
| A* | Misplaced-tile count | Admissible; prunes much of the search |
| A* | Manhattan distance | Admissible and tighter; expands the fewest nodes |

The solver uses a priority queue (`heapq`) ordered by f(n) = g(n) + h(n). It reports the solution depth, the number of nodes expanded and the maximum queue size, and can print the trace of expanded states.

## Run

```bash
pip install numpy
python 8_puzzle.py          # choose the default puzzle or enter your own, then pick an algorithm
```

`8_puzzle.ipynb` contains the same code with example runs.
