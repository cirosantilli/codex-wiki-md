<h1 id="16c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the steady, fully developed ansatz $\mathbf u=w(r)\mathbf e_z$, both $\partial_t\mathbf u$ and $(\mathbf u\cdot\nabla)\mathbf u$ vanish. The axial [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) reduces to

$$
0=-\frac{\partial p}{\partial z}
+\mu\frac1r\frac d{dr}\left(r\frac{dw}{dr}\right).
$$

Two integrations give

$$
w(r)=\frac1{4\mu}\frac{\partial p}{\partial z}r^2
+C_1\log r+C_2.
$$

Regularity at the axis forces $C_1=0$, and the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) $w(R)=0$ gives the [Hagen-Poiseuille flow](../../../../../../hagen-poiseuille-equation.md)

$$
\boxed{
w(r)=-\frac1{4\mu}\frac{\partial p}{\partial z}
(R^2-r^2)}.
$$

For flow in the positive $z$ direction, $\partial p/\partial z<0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16C](../../16c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
