<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define the [characteristic polynomial](../../../../../characteristic-polynomial.md) using $p(\lambda)=\det(\lambda I-P)$, where $I$ is the [identity matrix](../../../../../identity-matrix.md). Expanding the [determinant](../../../../../determinant.md) along the first row gives

$$
\begin{aligned}
p(\lambda)&=(\lambda-0.6)\bigl((\lambda-0.8)(\lambda-0.7)-0.02\bigr)\\
&\quad+0.1\bigl(-0.1(\lambda-0.7)-0.06\bigr)-0.1\bigl(0.01+0.3(\lambda-0.8)\bigr)\\
&=\lambda^3-2.1\lambda^2+1.4\lambda-0.3\\
&=(\lambda-1)(\lambda-0.6)(\lambda-0.5).
\end{aligned}
$$

Thus the [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is

$$
\boxed{p(\lambda)=\lambda^3-\frac{21}{10}\lambda^2+\frac75\lambda-\frac3{10}=0.}
$$

The convention $\det(P-\lambda I)$ changes the sign of this cubic [polynomial](../../../../../polynomial-split.md) but gives the same [roots](../../../../../root-of-a-root-system.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
