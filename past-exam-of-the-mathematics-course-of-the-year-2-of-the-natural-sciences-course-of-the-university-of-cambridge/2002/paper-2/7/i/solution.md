<h1 id="7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the equilibrium coordinates specified in the paper; their distances from the origin are one and their mutual separation is $\sqrt3$. Let $u_i=(x_i,y_i)$ be the small displacements. Each initially unstretched [spring](../../../../../spring.md) has, to first order, extension equal to the relative displacement projected along its original bond. Choose the three oriented extensions

$$
e_{12}=x_2-x_1,\qquad e_{13}=\tfrac12(x_3-x_1)+\tfrac{\sqrt3}{2}(y_3-y_1),\qquad e_{23}=-\tfrac12(x_3-x_2)+\tfrac{\sqrt3}{2}(y_3-y_2).
$$

The [kinetic energy](../../../../../kinetic-energy.md) is exact in these displacement coordinates, while the [potential energy](../../../../../potential-energy.md) needed for [small oscillations](../../../../../small-oscillation.md) is its quadratic part:

$$
\boxed{T=\frac m2\sum_{i=1}^3(\dot x_i^2+\dot y_i^2),\qquad V=\frac k2(e_{12}^2+e_{13}^2+e_{23}^2).}
$$

The factor $\sqrt3$ in the equilibrium bond length cancels when forming the unit bond directions. Applying the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md), or differentiating $V$ for the force on each mass, gives

$$
\boxed{\begin{aligned}
m\ddot x_1&=k(e_{12}+\tfrac12e_{13}),&m\ddot y_1&=\tfrac{\sqrt3 k}{2}e_{13},\\
m\ddot x_2&=-k(e_{12}+\tfrac12e_{23}),&m\ddot y_2&=\tfrac{\sqrt3 k}{2}e_{23},\\
m\ddot x_3&=-\tfrac k2(e_{13}-e_{23}),&m\ddot y_3&=-\tfrac{\sqrt3 k}{2}(e_{13}+e_{23}).
\end{aligned}}
$$

The total force vanishes componentwise, as expected for three masses coupled only by internal [spring](../../../../../spring.md) forces.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
