# Assignment Problem (AP)

**Summary**: A special case of the transportation problem where the objective is to assign $n$ tasks to $n$ resources on a one-to-one basis to minimize total cost or time.

**Sources**: Standard MBA OR Syllabus

**Last updated**: 2026-04-13

---

## Introduction
The Assignment Problem (AP) deals with allocating resources (e.g., workers, machines) to tasks (e.g., jobs) such that each resource is assigned to exactly one task and each task is performed by exactly one resource.

## Mathematical Formulation
The problem is represented by a square cost matrix $C$ of size $n \times n$. The decision variable $x_{ij}$ is 1 if resource $i$ is assigned to task $j$, and 0 otherwise.

## Hungarian Method
The standard algorithm to solve the Assignment Problem:
1. **Row Reduction**: Subtract the minimum element of each row from all elements in that row.
2. **Column Reduction**: Subtract the minimum element of each column from all elements in that column.
3. **Zero Covering**: Draw the minimum number of lines to cover all zeros.
4. **Optimality Check**: If the number of lines equals $n$, an optimal assignment exists.
5. **Matrix Modification**: If not optimal, find the smallest uncovered element and adjust the matrix.

## Special Cases
- **Unbalanced Assignment**: When the number of rows $\neq$ number of columns. Add dummy rows/columns.
- **Maximization**: Subtract all elements from the largest element in the matrix.
- **Restricted Assignment**: Assign a very high cost ($M$) to prohibited assignments.
- **Travelling Salesman Problem (TSP)**: A variation where a salesman visits every city exactly once and returns to the starting point.

## Related pages
- [[mba-403-operations-research-syllabus]]
- [[transportation-problem]]
