<h1 id="6b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For drift $A_i(x)$ and constant diffusion matrix $b_{ij}$, the [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) is

$$
\frac{\partial P}{\partial t}
=-\frac{\partial}{\partial x_i}(A_iP)
+\frac12\frac{\partial^2}{\partial x_i\partial x_j}(b_{ij}P).
$$

Here

$$
A_1=-x_1+x_2,
\qquad
A_2=-2x_1-x_2,
\qquad
b=I,
$$

so

$$
\boxed{
\frac{\partial P}{\partial t}
=\frac{\partial}{\partial x_1}\bigl[(x_1-x_2)P\bigr]
+\frac{\partial}{\partial x_2}\bigl[(2x_1+x_2)P\bigr]
+\frac12\left(
\frac{\partial^2P}{\partial x_1^2}
+\frac{\partial^2P}{\partial x_2^2}\right)}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6B](../../6b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
