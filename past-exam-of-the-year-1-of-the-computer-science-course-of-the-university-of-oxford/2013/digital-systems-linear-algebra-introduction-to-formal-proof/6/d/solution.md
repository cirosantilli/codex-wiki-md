<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [characteristic polynomial](../../../../../characteristic-polynomial.md) convention $p(\lambda)=\det(\lambda I-P)$, with $I$ the [identity matrix](../../../../../identity-matrix.md). Put $u=\lambda-1/2$. Then

$$
\begin{aligned}
p(\lambda)&=\det\begin{pmatrix}u&-1/2&-1/2\\-1/4&u&0\\-1/4&0&u\end{pmatrix}\\
&=u^3-\frac18u-\frac18u=u\left(u^2-\frac14\right)\\
&=\lambda(\lambda-1/2)(\lambda-1).
\end{aligned}
$$

The required [characteristic polynomial](../../../../../characteristic-polynomial.md) equation for this [matrix](../../../../../matrix.md) is therefore

$$
\boxed{p(\lambda)=\lambda^3-\frac32\lambda^2+\frac12\lambda=0.}
$$

Using $\det(P-\lambda I)$ instead negates the cubic [polynomial](../../../../../polynomial-split.md) and leaves the [eigenvalues](../../../../../eigenvalue.md) unchanged.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
