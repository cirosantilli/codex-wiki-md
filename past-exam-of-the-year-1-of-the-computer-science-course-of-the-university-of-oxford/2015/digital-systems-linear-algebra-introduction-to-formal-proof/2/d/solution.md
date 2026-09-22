<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [reduced row echelon form](../../../../../reduced-row-echelon-form.md) gives

$$
x_1=-2x_2-\frac{17}{5}x_4,\qquad x_3=\frac35x_4.
$$

Taking the [free variables](../../../../../free-variable.md) as $x_2=s$ and $x_4=5t$, the [null space](../../../../../kernel-of-a-linear-map-split.md) is

$$
\ker A=\left\{s\begin{pmatrix}-2\\1\\0\\0\end{pmatrix}+t\begin{pmatrix}-17\\0\\3\\5\end{pmatrix}:s,t\in\mathbb R\right\}.
$$

The two displayed [vectors](../../../../../vector.md) are [linearly independent](../../../../../linear-independence.md), as their second and fourth coordinates show, and each satisfies $Ax=0$. Thus

$$
\boxed{\text{a null-space basis is }\{(-2,1,0,0)^{\mathsf T},(-17,0,3,5)^{\mathsf T}\},\quad\dim\ker A=2.}
$$

This also agrees with the [rank-nullity theorem](../../../../../rank-nullity-theorem.md): $4-2=2$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
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
