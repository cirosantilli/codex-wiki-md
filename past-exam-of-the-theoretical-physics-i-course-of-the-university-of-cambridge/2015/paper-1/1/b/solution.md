<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The derivatives needed in the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) are

$$
\frac{\partial L}{\partial\dot\theta}
=ml^2\dot\theta+ml(\dot a_x\cos\theta+\dot a_y\sin\theta),
$$



$$
\frac{\partial L}{\partial\theta}
=ml\dot\theta(-\dot a_x\sin\theta+\dot a_y\cos\theta)-mgl\sin\theta.
$$

The terms proportional to $\dot a_i\dot\theta$ cancel after differentiation, leaving

$$
\boxed{l\ddot\theta+\ddot a_x\cos\theta+(g+\ddot a_y)\sin\theta=0.}
$$

With $\mathbf l=l(\sin\theta,-\cos\theta,0)$ and $\mathbf g=-g\hat{\mathbf y}$,

$$
[\mathbf l\times(\mathbf g-\ddot{\mathbf a})]_z
=-l\left[\ddot a_x\cos\theta+(g+\ddot a_y)\sin\theta\right]
=l^2\ddot\theta.
$$

Hence the vector equation is **$l^2\ddot\theta\hat{\mathbf z}=\mathbf l\times(\mathbf g-\ddot{\mathbf a})$**. In the translating support frame, $-m\ddot{\mathbf a}$ is the [inertial force](../../../../../fictitious-force.md). The rod's [tension](../../../../../tension.md) passes through the hinge and contributes no [torque](../../../../../torque.md) about it. The same [torque](../../../../../torque.md) equation therefore has an immediate mechanical interpretation.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
