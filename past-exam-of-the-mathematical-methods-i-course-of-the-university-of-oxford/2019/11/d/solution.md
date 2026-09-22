<h1 id="11/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $M=\begin{pmatrix}a&b\\c&d\end{pmatrix}$. The two off-diagonal entries of $M^2=M$ give

$$
b(a+d)=b,\qquad c(a+d)=c,
$$

or $b(\operatorname{tr}M-1)=c(\operatorname{tr}M-1)=0$. If both $b,c$ vanish, $M$ is diagonal; if either is nonzero, the [trace](../../../../matrix-trace.md) must be one. Thus the [trace criterion for a two-by-two idempotent](../../../../trace-criterion-for-a-two-by-two-idempotent.md) is

$$
\boxed{M^2=M\quad\Longrightarrow\quad M\text{ is diagonal or }\operatorname{tr}M=1.}
$$

For the diagonal case, idempotence further forces $a,d\in\{0,1\}$. The stated alternative is only necessary: $\begin{pmatrix}1&1\\1&0\end{pmatrix}$ has [trace](../../../../matrix-trace.md) one but its square is $\begin{pmatrix}2&1\\1&1\end{pmatrix}$, so it is not idempotent. Among two-by-two [matrices](../../../../matrix.md) of [trace](../../../../matrix-trace.md) one, the additional condition $\det M=0$ is sufficient by the [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md), which gives $M^2-M+(\det M)I=0$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [11](../../11.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
