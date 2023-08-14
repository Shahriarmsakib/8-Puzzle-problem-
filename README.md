# Eight-Puzzle Solver using Uniform Cost Search and A* Heuristics
This repository contains the implementation of an eight-puzzle solver as part of the Artificial Intelligence (CS205) class project. The eight-puzzle problem involves a 3x3 grid with eight numbered tiles and one empty space. The objective is to rearrange the tiles from a given initial state to a goal state using the minimum number of moves.
# Algorithms Used
The program implements three different search algorithms to solve the eight-puzzle problem:

Uniform Cost Search (UCS): A search algorithm that explores the search space by considering the cost of reaching each state. It guarantees an optimal solution but may not be very efficient for large state spaces.

A Search with Misplaced Tile Heuristic:* A* search is an informed search algorithm that uses a heuristic function to estimate the cost from the current state to the goal state. In this implementation, the Misplaced Tile heuristic is used, which counts the number of tiles that are not in their correct positions.

A Search with Manhattan Distance Heuristic:* Another A* variant that uses the Manhattan Distance heuristic. This heuristic calculates the sum of the horizontal and vertical distances of each tile from its goal position.
