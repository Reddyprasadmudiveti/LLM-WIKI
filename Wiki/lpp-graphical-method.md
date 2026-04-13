# LPP Graphical Method

**Summary**: A visual method for solving Linear Programming Problems with two decision variables.

**Sources**: operations research - Sunitha.jpg

**Last updated**: 2026-04-13

---

## Visual Steps
```text
[1. Plot Constraints]  -->  [2. Shade Feasible Area]
                                     │
                                     ▼
[4. Select Best Value] <--  [3. Identify Corner Points]
       (Optimal)
```

## Overview
The Graphical Method is a simple and visual technique used to solve a [[linear-programming-problem]] (LPP) (source: operations research - Sunitha.jpg). However, its primary limitation is that it can only be effectively applied to problems involving exactly two decision variables (source: operations research - Sunitha.jpg).

## Steps for the Graphical Method
1.  **Formulate the LPP**: Ensure the problem is expressed mathematically with two variables (source: operations research - Sunitha.jpg).
2.  **Plot the Constraints**: Treat each inequality constraint as an equation and plot the corresponding line on a 2D coordinate system (source: operations research - Sunitha.jpg).
3.  **Identify the Feasible Region**: For each constraint line, determine which side of the line satisfies the inequality. The intersection of all these satisfying regions, along with the non-negativity restrictions, forms the "feasible region" (source: operations research - Sunitha.jpg).
4.  **Find the Corner Points**: Identify the coordinates of the vertices (corner points) of the feasible region (source: operations research - Sunitha.jpg).
5.  **Evaluate the Objective Function**: Substitute the coordinates of each corner point into the objective function (source: operations research - Sunitha.jpg).
6.  **Determine the Optimal Solution**: 
    - For a maximization problem, the corner point that yields the highest value is the optimal solution (source: operations research - Sunitha.jpg).
    - For a minimization problem, the corner point that yields the lowest value is the optimal solution (source: operations research - Sunitha.jpg).

This method illustrates the **Fundamental Theorem of LPP**, which states that if a linear programming problem has an optimal solution, it must occur at one of the extreme points (corner points) of the feasible region (source: operations research - Sunitha.jpg).

For problems with more than two variables, algebraic methods like the [[simplex-algorithm]] must be used.

## Related pages
- [[linear-programming-problem]]
- [[simplex-algorithm]]