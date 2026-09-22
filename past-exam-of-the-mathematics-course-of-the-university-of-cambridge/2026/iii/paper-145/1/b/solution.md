<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Give every edge weight one and delete the row and column for $v_n$ from the out-Laplacian. Expanding the resulting banded determinant along its last available row gives

$$
a_n=a_{n-1}+2a_{n-2},
\qquad a_2=1,\quad a_3=3.
$$

The characteristic roots are $2$ and $-1$, and the initial values give

$$
a_n=\frac{2^n-(-1)^n}{3}.
$$

By the directed [matrix-tree theorem](../../../../../../kirchhoff-s-theorem.md), this determinant is exactly the number of directed spanning trees rooted towards $v_n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 145](../../../paper-145-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
