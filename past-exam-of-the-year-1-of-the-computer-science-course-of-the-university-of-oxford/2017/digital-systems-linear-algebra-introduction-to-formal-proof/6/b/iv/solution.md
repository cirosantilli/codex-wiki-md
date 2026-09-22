<h1 id="6/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**Yes.** Part (a) diagonalizes $G=B$, whose [spectral radius](../../../../../../spectral-radius.md) is $3/8<1$. Thus

$$
G^n=S\operatorname{diag}(0^n,(3/8)^n)S^{-1}\longrightarrow0\qquad(n\geq1),
$$

and every initial error converges to zero. For the specified initial vector, solving $Ax=b$ gives $x=(1,-1)^T$ and $e_0=(-1,1)^T$. In fact,

$$
\boxed{e_n=(3/8)^n\begin{pmatrix}-2\\1\end{pmatrix},\quad
x_n=\begin{pmatrix}1-2(3/8)^n\\-1+(3/8)^n\end{pmatrix}\quad(n\geq1).}
$$

The special formula is not asserted for $n=0$, because the zero-eigenvalue component disappears only after the first step.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
