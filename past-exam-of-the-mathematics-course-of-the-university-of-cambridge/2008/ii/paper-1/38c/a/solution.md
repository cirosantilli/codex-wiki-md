<h1 id="38c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Number the interior grid vertices in any order. The diagonal of $A$ is $10/3$, and off-diagonal weights are $-2/3$ for axial neighbors and $-1/6$ for diagonal neighbors. Each link weight is symmetric, so $A$ is symmetric. Extend the interior grid values by zero to the boundary. Since the eight stencil weights sum to $10/3$, grouping links gives

$$
u^TAu=\sum_{\{i,j\}\text{ interior link}}w_{ij}(u_i-u_j)^2+
\sum_{i\text{ interior},\ j\text{ boundary link}}w_{ij}u_i^2,
$$

where $w_{ij}=2/3$ or $1/6$ and each interior link is counted once. Every term is nonnegative. If the [quadratic form](../../../../../../quadratic-form.md) vanishes, neighboring interior values agree, and every vertex linked to the boundary has value zero. The axial-link grid is connected and reaches the boundary, so all values are zero. Thus $\boxed{A\text{ is symmetric positive definite}}$. Reordering vertices replaces $A$ by $PAP^T$ for a [permutation matrix](../../../../../../permutation-matrix.md) $P$, preserving both properties.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38C](../../38c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
