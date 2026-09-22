<h1 id="12b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The vector identity from Question 3 gives

$$
\begin{aligned}
\nabla\cdot(E\times B)
&=B\cdot(\nabla\times E)-E\cdot(\nabla\times B)\\
&=-B\cdot\frac{\partial B}{\partial t}
-E\cdot J-E\cdot\frac{\partial E}{\partial t}\\
&=-E\cdot J
-\frac{\partial}{\partial t}
\frac{|E|^2+|B|^2}{2}.
\end{aligned}
$$

Integrating over $V$ and applying the [divergence theorem](../../../../../../divergence-theorem.md) proves the [Poynting theorem](../../../../../../poynting-theorem.md)

$$
\boxed{
\int_SP\cdot dS
=-\int_VE\cdot J\,dV
-\frac{\partial}{\partial t}
\int_V\frac{|E|^2+|B|^2}{2}\,dV}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12B](../../12b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
