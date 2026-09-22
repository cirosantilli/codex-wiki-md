<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The requested order is $A=P^{-1}DP$. To obtain this order directly, put the transposes of the two [eigenvectors](../../../../../eigenvector.md) in the rows of $P$, using the fact that $A$ is symmetric:

$$
\boxed{P=\begin{pmatrix}\varphi&1\\\psi&1\end{pmatrix},\qquad D=\begin{pmatrix}\varphi&0\\0&\psi\end{pmatrix}.}
$$

Then $\det P=\varphi-\psi=\sqrt5\ne0$, so $P$ is an [invertible matrix](../../../../../invertible-matrix.md), with

$$
P^{-1}=\frac1{\sqrt5}\begin{pmatrix}1&-1\\-\psi&\varphi\end{pmatrix}.
$$

Multiplication gives $PA=\bigl(\begin{smallmatrix}\varphi+1&\varphi\\\psi+1&\psi\end{smallmatrix}\bigr)=DP$, since $\varphi^2=\varphi+1$ and $\psi^2=\psi+1$. Multiplying by $P^{-1}$ proves the required [diagonalization](../../../../../diagonalization-of-a-matrix.md). Putting the [eigenvectors](../../../../../eigenvector.md) in columns would instead give the equally standard order $A=QDQ^{-1}$, so the convention must be checked rather than copied mechanically.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
