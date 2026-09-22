<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The reduced graph Laplacian is $L^{(0)}=\Delta(I-P^{(0)})$. By the [matrix-tree theorem](../../../../../../kirchhoff-s-theorem.md), the number $\tau(D)$ of spanning trees is

$$
\tau(D)=\det L^{(0)}=\Delta^n\det(I-P^{(0)}).
$$

Combining this with part (a) gives

$$
\prod_{j=1}^n g_{D\setminus\{x_0,\ldots,x_{j-1}\}}(x_j)
=\frac{\Delta^n}{\tau(D)}.
$$

This is also the normalization behind [Wilson algorithm](../../../../../../wilson-s-algorithm.md): loop-erased random walks attach the vertices successively, and the order-independent product ensures that every rooted spanning tree has probability $1/\tau(D)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
