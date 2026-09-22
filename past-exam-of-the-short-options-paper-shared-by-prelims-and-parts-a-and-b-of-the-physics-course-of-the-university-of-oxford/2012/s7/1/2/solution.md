<h1 id="s7/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) in cylindrical coordinates are

$$
\boxed{\ddot R=R\dot\phi^2-\frac{C\dot z}{R},\qquad
\frac d{dt}(R^2\dot\phi)=0,\qquad
\ddot z=\frac{C\dot R}{R}.}
$$

The last two follow because $\phi$ and $z$ are [cyclic coordinates](../../../../../cyclic-coordinate.md). They give the [conserved quantities](../../../../../conserved-quantity.md)

$$
\boxed{\ell=R^2\dot\phi,\qquad k=\dot z-C\log R.}
$$

Since the [Lagrangian](../../../../../lagrangian.md) is autonomous, its energy function is conserved as well:

$$
\boxed{\mathcal E=\dot R\frac{\partial L}{\partial\dot R}
+\dot\phi\frac{\partial L}{\partial\dot\phi}
+\dot z\frac{\partial L}{\partial\dot z}-L
=\frac12(\dot R^2+R^2\dot\phi^2+\dot z^2).}
$$

The velocity-linear term cancels from this energy, but it still changes the equations of motion. A dimensionless logarithm means $\log(R/R_0)$ for some fixed reference length; replacing the printed $\log R$ by that expression changes the [Lagrangian](../../../../../lagrangian.md) only by a total time derivative and shifts the numerical value of $k$, not the trajectory.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [S7](../../../s7.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
