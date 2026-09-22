<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Measure each [generalized coordinate](../../../../../generalized-coordinate.md) $\theta_i$ from an unstressed configuration. The diagram has one [torsional spring](../../../../../torsion-spring.md) joining the frame to object 1, one joining objects 1 and 2, and one joining objects 2 and 3. The [rotational kinetic energy](../../../../../rotational-kinetic-energy.md) and [elastic potential energy](../../../../../elastic-energy.md) are

$$
T=\frac12\sum_{i=1}^3I_i\dot\theta_i^2,\qquad
U=\frac12k_1\theta_1^2+\frac12k_2(\theta_2-\theta_1)^2+\frac12k_3(\theta_3-\theta_2)^2.
$$

Each spring contribution follows by integrating its restoring [torque](../../../../../torque.md): $\int_0^{\Delta\theta}k_j s\,ds=k_j(\Delta\theta)^2/2$. Thus

$$
\boxed{L=T-U.}
$$

The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) give

$$
\boxed{\begin{aligned}
I_1\ddot\theta_1+(k_1+k_2)\theta_1-k_2\theta_2&=0,\\
I_2\ddot\theta_2-k_2\theta_1+(k_2+k_3)\theta_2-k_3\theta_3&=0,\\
I_3\ddot\theta_3-k_3\theta_2+k_3\theta_3&=0.
\end{aligned}}
$$

These hold for either interpretation of the square's [moment of inertia](../../../../../moment-of-inertia.md); the geometry-based value from (a) is used first below.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
