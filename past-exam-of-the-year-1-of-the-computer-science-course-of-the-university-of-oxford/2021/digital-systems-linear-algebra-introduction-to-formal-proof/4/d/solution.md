<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [diagonalization](../../../../../diagonalization-of-a-matrix.md) gives $A=SDS^{-1}$ and hence $A^{n-1}=SD^{n-1}S^{-1}$: the intervening factors $S^{-1}S$ cancel. The [diagonal matrix](../../../../../diagonal-matrix.md) power has entries $\alpha^{n-1},\beta^{n-1}$. Since $1-\beta=\alpha$ and $\alpha-1=-\beta$,

$$
S^{-1}\begin{pmatrix}1\\1\end{pmatrix}=\frac1{\sqrt5}\begin{pmatrix}\alpha\\-\beta\end{pmatrix},\qquad
V_n=\frac1{\sqrt5}\begin{pmatrix}\alpha^{n+1}-\beta^{n+1}\\\alpha^n-\beta^n\end{pmatrix}.
$$

Reading the second component gives the [Binet formula](../../../../../binet-formula.md)

$$
\boxed{U_n=\frac{\left((1+\sqrt5)/2\right)^n-\left((1-\sqrt5)/2\right)^n}{\sqrt5}.}
$$

The derivation includes $n=1$, and the expression gives $U_1=U_2=1$, consistent with the specified indexing.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
