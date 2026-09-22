<h1 id="17g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A$ be the [adjacency matrix of a graph](../../../../../../adjacency-matrix.md). Since $G$ is a [regular graph](../../../../../../regular-graph.md) of degree $d$, every row of $A$ sums to $d$. Therefore, for $\mathbf e=(1,\ldots,1)^T$,

$$
\boxed{A\mathbf e=d\mathbf e},
$$

so $d$ is a [graph eigenvalue](../../../../../../graph-eigenvalue.md).

If $Av=dv$, then the quadratic form of the [Graph Laplacian](../../../../../../laplacian-matrix.md) $L=dI-A$ gives

$$
0=v^*(dI-A)v
=\sum_{\{i,j\}\in E(G)}|v_i-v_j|^2.
$$

Every summand is nonnegative, so $v_i=v_j$ along every edge. The graph is [connected](../../../../../../connected-graph.md), hence all coordinates of $v$ are equal and $v$ is a scalar multiple of $\mathbf e$. Thus the $d$-eigenspace is one-dimensional. Since $A$ is a [symmetric matrix](../../../../../../symmetric-matrix.md), the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) makes it diagonalizable, so the algebraic multiplicity is also one. This proves the [constant eigenvector of a regular graph](../../../../../../constant-eigenvector-of-a-regular-graph.md) result.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
