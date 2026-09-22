<h1 id="6a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $A_{ji}$ denotes the matrix obtained by deleting row $j$ and column $i$, then the [adjugate matrix](../../../../../../adjugate-matrix.md) is

$$
\operatorname{adj}(A)_{ij}
=(-1)^{i+j}\det A_{ji}.
$$

For nonsingular $A$,

$$
\operatorname{adj}(A)=\det(A)A^{-1}.
$$

Therefore, when $A$ and $B$ are nonsingular,

$$
\begin{aligned}
\operatorname{adj}(AB)
&=\det(A)\det(B)(AB)^{-1}\\
&=\det(B)B^{-1}\det(A)A^{-1}\\
&=\boxed{\operatorname{adj}(B)\operatorname{adj}(A)}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6A](../../6a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
