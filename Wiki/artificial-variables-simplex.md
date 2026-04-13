# Artificial Variables in Simplex

**Summary**: Techniques (Big-M and Two-Phase) used in the Simplex algorithm when initial basic feasible solutions are not readily available.

**Sources**: operations research - Sunitha.jpg

**Last updated**: 2026-04-13

---

## The Concept of Artificial Variables
In a standard [[simplex-algorithm]], we add "slack" variables to $\le$ constraints to create an initial basic feasible solution (source: operations research - Sunitha.jpg). However, when constraints are $\ge$ or $=$, subtracting a "surplus" variable does not provide a positive unit vector for the initial basis (source: operations research - Sunitha.jpg). 

To resolve this, we introduce **Artificial Variables** (source: operations research - Sunitha.jpg). These are fictitious variables added to equations to mathematically create an initial identity matrix so the Simplex algorithm can begin (source: operations research - Sunitha.jpg). However, because they are artificial, they must be driven to zero for the final solution to be valid for the original problem (source: operations research - Sunitha.jpg).

There are two primary methods to handle artificial variables:

## 1. The Big-M Method (Method of Penalties)
In the Big-M method, a very large penalty coefficient, denoted as $M$, is assigned to the artificial variables in the objective function (source: operations research - Sunitha.jpg). 
- Because $M$ is overwhelmingly large, the Simplex algorithm will naturally prioritize driving the artificial variables out of the basis (source: operations research - Sunitha.jpg).
- If an artificial variable remains in the optimal basis with a positive value, the original problem has no feasible solution (source: operations research - Sunitha.jpg).

## 2. The Two-Phase Simplex Method
This method splits the problem into two phases:
- **Phase I**: The objective is to *minimize* the sum of the artificial variables. If Phase I ends with the sum of artificial variables greater than zero, the original problem has no feasible solution (source: operations research - Sunitha.jpg).
- **Phase II**: The original objective function is restored, and the standard Simplex algorithm continues to find the final optimal solution (source: operations research - Sunitha.jpg).

## Related pages
- [[simplex-algorithm]]
- [[linear-programming-problem]]