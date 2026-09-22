<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [matrix multiplication](../../../../../matrix-multiplication.md) to evolve the [probability vector](../../../../../probability-vector.md) by $x_{n+1}=Px_n$. With $x_0=(0.4,0.4,0.2)^{\mathsf T}$,

$$
x_1=\begin{pmatrix}0.24+0.04+0.02\\0.04+0.32+0.04\\0.12+0.04+0.14\end{pmatrix}=\begin{pmatrix}0.30\\0.40\\0.30\end{pmatrix},\qquad x_2=\begin{pmatrix}0.18+0.04+0.03\\0.03+0.32+0.06\\0.09+0.04+0.21\end{pmatrix}=\begin{pmatrix}0.25\\0.41\\0.34\end{pmatrix}.
$$

Hence, in Central, Headington, Botley order,

$$
\boxed{\text{day 1: }(30\%,40\%,30\%),\qquad\text{day 2: }(25\%,41\%,34\%).}
$$

Both [probability vectors](../../../../../probability-vector.md) have nonnegative entries summing to one.

## ↑ Ancestors (12)

1. [C](../c.md)
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
