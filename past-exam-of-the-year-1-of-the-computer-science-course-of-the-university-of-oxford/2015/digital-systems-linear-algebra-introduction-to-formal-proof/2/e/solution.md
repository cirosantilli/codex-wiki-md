<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Apply the same [elementary row operations](../../../../../elementary-row-operation.md) to the [augmented matrix](../../../../../augmented-matrix.md):

$$
\left(\begin{array}{rrrr|r}1&2&-1&4&2\\1&2&4&1&7\\-1&-2&6&-7&3\end{array}\right)\sim\left(\begin{array}{rrrr|r}1&2&-1&4&2\\0&0&5&-3&5\\0&0&0&0&0\end{array}\right).
$$

The last row establishes consistency; equivalently the third original row is the second minus twice the first, and the right-hand entries obey $3=7-2\cdot2$. With $x_2=s$ and $x_4=5t$, the second equation gives $x_3=1+3t$ and the first gives $x_1=3-2s-17t$. All real solutions are therefore

$$
\boxed{x=\begin{pmatrix}3\\0\\1\\0\end{pmatrix}+s\begin{pmatrix}-2\\1\\0\\0\end{pmatrix}+t\begin{pmatrix}-17\\0\\3\\5\end{pmatrix},\qquad s,t\in\mathbb R.}
$$

This [affine solution space](../../../../../affine-solution-space.md) is one particular solution plus the [null space](../../../../../kernel-of-a-linear-map-split.md). The two [free variables](../../../../../free-variable.md) show that there are no additional restrictions.

## ↑ Ancestors (12)

1. [E](../e.md)
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
