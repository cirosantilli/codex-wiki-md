<h1 id="s19/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D(d)=\begin{pmatrix}1&d\\0&1\end{pmatrix}$ be the drift [beam transfer matrix](../../../../../beam-transfer-matrix.md). Start immediately before the first lens and end immediately before its counterpart in the next [FODO cell](../../../../../fodo-cell.md). Matrices act on column vectors from right to left. With $A=1/f_1$ and $B=1/f_2$, where both focal lengths are signed in the chosen plane,

$$
\boxed{M=DQ(f_2)DQ(f_1)=
\begin{pmatrix}
1-2dA-dB+d^2AB&2d-d^2B\\
-A-B+dAB&1-dB
\end{pmatrix}.}
$$

The two drifts account for both gaps. Direct multiplication gives $\det M=1$ and

$$
\frac12\operatorname{tr}M=1-d(A+B)+\frac{d^2AB}{2}.
$$

For the equal-strength focusing-defocusing case, $f_1=f>0$ and $f_2=-f$:

$$
M=\begin{pmatrix}1-d/f-d^2/f^2&2d+d^2/f\\-d/f^2&1+d/f\end{pmatrix},
\qquad \operatorname{tr}M=2-\frac{d^2}{f^2}.
$$

Choosing a different start within the cell gives a conjugate matrix, with the same trace and eigenvalues. If $f_2$ is specified as a positive magnitude of a defocusing lens, its signed value in these formulas is $-f_2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [S19](../../../s19.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
