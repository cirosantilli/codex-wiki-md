<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Update the unknowns in row order, immediately using newly computed components. The component equations are

$$
\begin{aligned}
x_1^{(n)}&=-1+x_2^{(n-1)}-x_3^{(n-1)},\\
x_2^{(n)}&=\tfrac12(2-x_1^{(n)}-x_3^{(n-1)})=\tfrac32-\tfrac12x_2^{(n-1)},\\
x_3^{(n)}&=\tfrac12(-2-x_1^{(n)}+x_2^{(n)})=\tfrac14-\tfrac34x_2^{(n-1)}+\tfrac12x_3^{(n-1)}.
\end{aligned}
$$

Thus **$G=\begin{pmatrix}0&1&-1\\0&-1/2&0\\0&-3/4&1/2\end{pmatrix}$** and **$c=(-1,3/2,1/4)^T$**. Using only old values in all three row equations would instead describe the [Jacobi method](../../../../../../jacobi-method.md), not the [Gauss-Seidel method](../../../../../../gauss-seidel-method.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
