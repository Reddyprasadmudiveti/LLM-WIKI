# Transportation Problem (TP)

**Summary**: A specialized type of linear programming problem that deals with minimizing the cost of distributing goods from multiple sources to multiple destinations.

**Sources**: Standard MBA OR Syllabus

**Last updated**: 2026-04-13

---

## Introduction
The Transportation Problem (TP) involves shipping products from $m$ sources to $n$ destinations at minimum cost, given the supply at each source and the demand at each destination.

## Initial Basic Feasible Solution (IBFS)
Before finding the optimal solution, we must find an initial basic feasible solution using one of these methods:
1. **North-West Corner Rule (NWCR)**: Starts from the top-left cell and allocates sequentially.
2. **Least Cost Method (LCM)**: Prioritizes cells with the lowest unit transportation costs.
3. **Vogel’s Approximation Method (VAM)**: Uses penalty costs (difference between the two lowest costs in each row/column) to find a solution closer to the optimum.

## Optimality Testing
Once an IBFS is obtained, we test it for optimality:
- **MODI Method (Modified Distribution / u-v Method)**: The most standard method for calculating cell evaluations and improving the solution.
- **Stepping Stone Method**: An alternative method using closed loops to evaluate non-basic cells.

## Special Cases
- **Unbalanced Problem**: When total supply $\neq$ total demand. Add a dummy row or column with zero costs to balance it.
- **Degeneracy**: Occurs when the number of allocated cells is less than $(m + n - 1)$.
- **Maximization**: Convert by subtracting all costs from the largest cost in the tableau.

## Related pages
- [[mba-403-operations-research-syllabus]]
- [[assignment-problem]]
