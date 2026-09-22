<h1 id="38e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Gershgorin circle theorem](../../../../../../gershgorin-circle-theorem.md) says that every [eigenvalue](../../../../../../eigenvalue.md) of a square [matrix](../../../../../../matrix.md) lies in at least one disc centred at a diagonal entry with radius the sum of the absolute values of the off-diagonal entries in that row.

For interior unknowns write the update as $u^{n+1}=Bu^n$. The [matrix](../../../../../../matrix.md) is real symmetric and tridiagonal, with diagonal $1-\mu(a_{m-1/2}+a_{m+1/2})$ and adjacent entries $\mu a_{m+1/2}$. Each Gershgorin radius is at most $\mu(a_{m-1/2}+a_{m+1/2})$. Its real interval is therefore contained in

$$
[1-2\mu(a_{m-1/2}+a_{m+1/2}),1]\subset[1-4\mu a_+,1].
$$

For **$0<\mu\leq1/(2a_+)$**, every [eigenvalue](../../../../../../eigenvalue.md) lies in $[-1,1]$. Symmetry gives an orthogonal diagonalization, so $\|B^n\|_2\leq1$ for every $n$: errors in initial data cannot grow. This is stability in the discrete $\ell^2$ norm, also in its $h$-weighted version. One can additionally see maximum-norm stability directly: the update weights are nonnegative with row sums at most one once the zero boundary unknowns are removed. Hence $\|B\|_\infty\leq1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38E](../../38e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
