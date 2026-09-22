<h1 id="14b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $D=f[x_0,\ldots,x_n]$ and let $D_i$ be the [divided difference](../../../../../../divided-difference.md) with $x_i$ omitted. By symmetry from part (a), reorder the full list so that its first node is $x_i$ and its last is $x_j$. The recurrence from part (b) then has first omitted-node term $D_i$ and second omitted-node term $D_j$, and gives

$$
\boxed{D=\frac{D_i-D_j}{x_j-x_i}}.
$$

This proves the requested identity for every pair $i\ne j$ and fixes its sign explicitly; it is one of the [omitted-node identities for divided differences](../../../../../../omitted-node-identities-for-divided-differences.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14B](../../14b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
