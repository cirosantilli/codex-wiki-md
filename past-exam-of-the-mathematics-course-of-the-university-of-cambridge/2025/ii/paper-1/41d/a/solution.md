<h1 id="41d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Starting with $A_0=A$, suppose columns $1,\ldots,j-1$ have already been reduced to tridiagonal form. Let $x$ be the part of column $j$ in rows $j+1,\ldots,n$. A [Householder reflection](../../../../../../householder-transformation.md) $P_j$ on these coordinates can map $x$ to $\pm\lVert x\rVert e_1$. Extend it by the identity on the first $j$ coordinates and call the resulting orthogonal [matrix](../../../../../../matrix.md) $U_j$.

The update

$$
A_j=U_j^TA_{j-1}U_j
$$

zeros every entry below row $j+1$ in column $j$. Because it is an [orthogonal similarity](../../../../../../orthogonal-similarity.md), it preserves [eigenvalues](../../../../../../eigenvalue.md); because the same transformation is applied on both sides, it preserves symmetry and zeros the corresponding row entries without disturbing earlier columns. After $n-2$ such steps,

$$
H=U^TAU,\qquad U=U_1U_2\cdots U_{n-2},
$$

is symmetric and tridiagonal and has the same [eigenvalues](../../../../../../eigenvalue.md) as $A$. Every reflector is obtained from finitely many [matrix](../../../../../../matrix.md) entries using finitely many arithmetic operations and a square root, so this is a finite construction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41D](../../41d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
