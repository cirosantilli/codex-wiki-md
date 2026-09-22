<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate both algebraic [constraints](../../../../../constraint-mechanics.md) at fixed $y$ or fixed $x$:

$$
z_x=\frac{2x}z,\quad z_y=\frac yz,\qquad u_x=\frac xu,\quad u_y=-\frac yu.
$$

The [multivariable chain rule](../../../../../multivariable-chain-rule.md) for $\phi(x,y)=\psi(z,u)$ therefore gives

$$
\left(\frac{\partial\phi}{\partial x}\right)_y=\frac{2x}z\left(\frac{\partial\psi}{\partial z}\right)_u+\frac xu\left(\frac{\partial\psi}{\partial u}\right)_z,\qquad\left(\frac{\partial\phi}{\partial y}\right)_x=\frac yz\left(\frac{\partial\psi}{\partial z}\right)_u-\frac yu\left(\frac{\partial\psi}{\partial u}\right)_z.
$$

Divide the first identity by $x$ and the second by $y$, and add. The $\psi_u$ terms cancel, leaving

$$
\boxed{\frac1x\left(\frac{\partial\phi}{\partial x}\right)_y+\frac1y\left(\frac{\partial\phi}{\partial y}\right)_x=\frac3z\left(\frac{\partial\psi}{\partial z}\right)_u.}
$$

The [Jacobian determinant](../../../../../jacobian-determinant.md) of $(x,y)\mapsto(z,u)$ is $-3xy/(zu)$, so the calculation is valid on real branches with $xyzu\ne0$. This explicitly supplies the local independence assumption underlying the change of coordinates.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
