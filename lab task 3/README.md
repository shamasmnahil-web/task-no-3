# AI Lab -- Search Algorithms

## Project Overview

This project demonstrates common Artificial Intelligence search
algorithms using a small graph of nodes (`A` to `G`). It includes:

1.  **Breadth-First Search (BFS)** -- explores nodes level by level and
    returns a path to the goal.
2.  **Depth-First Search (DFS)** -- explores a branch deeply before
    backtracking and returns a path to the goal.
3.  **Depth-Limited Search (DLS)** -- performs depth-first search up to
    a specified depth limit.
4.  **Iterative Deepening Depth-First Search (IDDFS)** -- repeats
    depth-limited search with increasing depth limits.
5.  **Uniform-Cost Search (UCS)** -- searches for a lowest-total-cost
    path using edge weights and a priority queue.

## Project Files

-   `Task3_1.ipynb` -- implementation and examples of BFS and DFS.
-   `Task3_2.ipynb` -- implementation and examples of DLS and IDDFS.
-   `ucs.py` (or your chosen Python filename) -- Uniform-Cost Search
    implementation shared in the project chat.

## Graph Used

The notebooks use this directed graph:

-   `A → B`, `A → C`
-   `B → D`, `B → E`
-   `C → F`
-   `E → G`

The UCS example uses weighted edges:

-   `A → B` with cost 1; `A → C` with cost 6
-   `B → D` with cost 2; `B → E` with cost 1
-   `C → F` with cost 2; `C → G` with cost 12
-   `E → G` with cost 1

## Requirements

-   Python 3
-   Jupyter Notebook (to open and run the `.ipynb` files)

The code uses Python standard-library modules only (`collections.deque`
and `heapq`), so no additional Python packages are required.

## How to Run

1.  Install Python 3.

2.  To run the notebooks, install Jupyter Notebook if it is not already
    installed:

    ``` bash
    pip install notebook
    ```

3.  Open a terminal in the project folder and start Jupyter:

    ``` bash
    jupyter notebook
    ```

4.  Open `Task3_1.ipynb` and `Task3_2.ipynb`, then run their cells.

5.  Save the Uniform-Cost Search code in a Python file such as `ucs.py`
    and run:

    ``` bash
    python ucs.py
    ```

## Expected UCS Example

For the weighted graph in the provided code, the lowest-cost route from
`A` to `G` is `A → B → E → G`, with a total cost of `3`.

## Notes

-   BFS and DFS use an unweighted graph.
-   DLS and IDDFS use a depth limit to control how far the search
    explores.
-   UCS considers edge costs and finds the least-cost path when edge
    costs are non-negative.
