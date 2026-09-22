<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Write $A=I_3+N$, where

$$
N=\begin{pmatrix}0&a&b\\0&0&c\\0&0&0\end{pmatrix},\qquad
N^2=\begin{pmatrix}0&0&ac\\0&0&0\\0&0&0\end{pmatrix},\qquad N^3=0.
$$

The [binomial theorem for commuting matrices](../../../../../../../binomial-theorem-for-commuting-matrices.md) applies because $I_3N=NI_3$. All terms of degree at least three vanish, so for every positive [integer](../../../../../../../integer-split.md) $n$,

$$
\boxed{A^n=I_3+nN+\binom n2N^2
=\begin{pmatrix}
1&na&nb+\dfrac{n(n-1)}2ac\\
0&1&nc\\
0&0&1
\end{pmatrix}.}
$$

The same expression directly gives $A$ when $n=1$, so no small exponent is excluded.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [1](../../../1.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
