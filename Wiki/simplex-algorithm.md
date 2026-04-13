# Simplex Algorithm

**Summary**: The fundamental iterative algebraic procedure for solving Linear Programming Problems.

**Sources**: operations research - Sunitha.jpg

**Last updated**: 2026-04-13

---

## Overview
The Simplex Algorithm is a widely used mathematical method for solving a [[linear-programming-problem]] (LPP) (source: operations research - Sunitha.jpg). While the [[lpp-graphical-method]] is limited to two variables, the Simplex algorithm can handle problems with any number of decision variables and constraints (source: operations research - Sunitha.jpg).

## Process Flowchart
```text
START: Formulate LPP & Add Slack/Surplus
          │
          ▼
   Set up Initial Tableau
          │
          ▼
   Check Optimality (Z-row) ◄───────┐
          │                         │
   Is it Optimal? ──── NO ──► Pivot Operation:
          │                  1. Find Entering Var
         YES                 2. Find Departing Var
          │                  3. Row Operations
          ▼                         │
    STOP: Optimal Solution ─────────┘
```

## Concept
The algorithm is an iterative process. It starts at a basic feasible solution and systematically moves to an adjacent basic feasible solution that improves the value of the objective function (source: operations research - Sunitha.jpg). It continues this process until it reaches a solution where no further improvement is possible, which is the optimal solution (source: operations research - Sunitha.jpg).

It relies on the **Fundamental Theorem of LPP**, searching only the extreme points (vertices) of the feasible region, but it does so algebraically using matrices and row operations (source: operations research - Sunitha.jpg).

## Key Steps
1.  **Standard Form**: Convert all inequality constraints into equations by adding "slack" variables or subtracting "surplus" variables (source: operations research - Sunitha.jpg).
2.  **Initial Tableau**: Set up an initial matrix called a simplex tableau, representing the initial basic feasible solution (source: operations research - Sunitha.jpg).
3.  **Optimality Check**: Examine the "index row" to see if the current solution is optimal (source: operations research - Sunitha.jpg).
4.  **Pivot Operation**: If the solution is not optimal, identify the entering variable and departing variable, then perform row operations to pivot (source: operations research - Sunitha.jpg).
5.  **Iterate**: Repeat the optimality check and pivot operation until the optimal solution is reached (source: operations research - Sunitha.jpg).

When problems involve $\ge$ or $=$ constraints, standard slack variables aren't enough to start the algorithm easily, requiring advanced techniques like [[artificial-variables-simplex]].

## Related pages
- [[linear-programming-problem]]
- [[lpp-graphical-method]]
- [[artificial-variables-simplex]]
- [[lpp-duality]]