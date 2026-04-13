# Duality in LPP

**Summary**: The concept that every Linear Programming Problem has a corresponding "dual" problem, and the methods used to exploit this relationship.

**Sources**: operations research - Sunitha.jpg

**Last updated**: 2026-04-13

---

## Primal vs. Dual Comparison
| Feature | Primal Problem | Dual Problem |
| :--- | :--- | :--- |
| **Objective** | Maximization (e.g.) | Minimization (e.g.) |
| **Coefficients** | Objective Function | RHS Constants |
| **RHS Constants** | Constraints | Objective Function |
| **Variables** | $n$ variables | $m$ constraints |
| **Constraints** | $m$ constraints | $n$ variables |
| **Matrix** | Matrix $A$ | Transpose $A^T$ |

## Concept of Duality
One of the most important discoveries in linear programming is the concept of Duality (source: operations research - Sunitha.jpg). It states that every [[linear-programming-problem]] (called the "Primal" problem) is intimately related to another linear programming problem called its "Dual" (source: operations research - Sunitha.jpg).

Key relationships between Primal and Dual:
- If the primal is a maximization problem, the dual is a minimization problem (source: operations research - Sunitha.jpg).
- The coefficients of the objective function in the primal become the right-hand side constants of the constraints in the dual (source: operations research - Sunitha.jpg).
- The right-hand side constants of the primal constraints become the objective function coefficients in the dual (source: operations research - Sunitha.jpg).
- The number of variables in the primal equals the number of constraints in the dual (source: operations research - Sunitha.jpg).

**Significance**: The optimal objective value of the primal is exactly equal to the optimal objective value of the dual (source: operations research - Sunitha.jpg).

## Dual Simplex Method
The **Dual Simplex Method** takes the opposite approach to the standard simplex algorithm (source: operations research - Sunitha.jpg). It starts with a basic solution that is *optimal* but is *infeasible*. The algorithm then iterates to restore feasibility while maintaining optimality (source: operations research - Sunitha.jpg). 

This method is particularly useful when a new constraint is added to a problem after it has already been solved (source: operations research - Sunitha.jpg).

## Related pages
- [[linear-programming-problem]]
- [[simplex-algorithm]]