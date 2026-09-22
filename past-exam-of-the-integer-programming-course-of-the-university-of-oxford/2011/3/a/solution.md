<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The assignment constraint [matrix](../../../../matrix.md) has one row for each outgoing sum and one for each incoming sum. The column for $x_{ij}$ has a one in outgoing row $i$ and incoming row $j$. Negate all incoming rows. Each column now has exactly one $+1$ and one $-1$, the [node-arc incidence matrix](../../../../oriented-incidence-matrix.md) of the directed bipartite [graph](../../../../graph-split.md) from row vertices to column vertices.

Here is a direct proof that this signed [matrix](../../../../matrix.md) is [totally unimodular](../../../../totally-unimodular-matrix.md). Consider any square submatrix and induct on its size. If a column has no nonzero entry, its [determinant](../../../../determinant.md) is zero. If a column has one nonzero entry, expansion along it reduces the [determinant](../../../../determinant.md) to plus or minus a smaller subdeterminant, hence to $0,1$ or $-1$. If every column has two nonzero entries, they have opposite signs, so each column sum is zero. The rows are then dependent and the [determinant](../../../../determinant.md) is zero. The size-one case is immediate, completing the induction.

Negating rows only changes signs of square subdeterminants. Thus the original assignment [matrix](../../../../matrix.md) is also a **[totally unimodular matrix](../../../../totally-unimodular-matrix.md)**. This proves the [total unimodularity of directed incidence matrices](../../../../total-unimodularity-of-directed-incidence-matrices.md) argument directly in the required setting.

The integrality theorem for totally unimodular systems says that $\{x\geq0:Ax=b\}$ has integral vertices when $A$ is totally unimodular and $b$ is integral. Redundant equalities cause no problem. Here the row sums also force $x_{ij}\leq1$, so every integral feasible vertex is a binary assignment. The bounded nonempty LP relaxation has an optimal vertex, and therefore an optimal assignment. Hence **the [assignment problem](../../../../assignment-problem.md) can be solved by [linear programming](../../../../linear-programming-split.md) without a binary search**; dedicated methods such as the [Hungarian algorithm](../../../../hungarian-algorithm.md) also exploit its polynomial-time structure. Multiple optimal assignments can have fractional [convex combinations](../../../../convex-combination.md), so the conclusion concerns an optimal integral vertex, not every optimal LP point.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
