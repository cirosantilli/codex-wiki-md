<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The state update [matrix](../../../../matrix.md) is

$$
A=\begin{pmatrix}1/2&1/2\\1&0\end{pmatrix}.
$$

Its [eigenvalues](../../../../eigenvalue.md) are $1$ and $-1/2$, with [eigenvectors](../../../../eigenvector.md) $(1,1)^T$ and $(1,-2)^T$. The initial column $(G_1,G_0)^T=(1,0)^T$ decomposes as $\frac23(1,1)^T+\frac13(1,-2)^T$. Applying $A^i$ and reading the second component gives

$$
\boxed{G_i=\frac23\left[1-\left(-\frac12\right)^i\right]\ \longrightarrow\ \frac23.}
$$

The alternating term decays because its [eigenvalue](../../../../eigenvalue.md) has modulus below one. The [convergence of an adjacent-term averaging recurrence](../../../../convergence-of-an-adjacent-term-averaging-recurrence.md) gives the same result by a first-order recurrence for successive differences.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
