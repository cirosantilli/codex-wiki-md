<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\rho$ for cylindrical radius in this question, not the rod's [mass density](../../../../density.md). A charged relativistic particle in a time-independent [magnetic field](../../../../magnetic-field-split.md) has the [charged-particle electromagnetic Lagrangian](../../../../charged-particle-electromagnetic-lagrangian.md)

$$
L=-mc^2\sqrt{1-\mathbf v^2/c^2}+q\mathbf A\cdot\mathbf v,
$$

with zero electrostatic potential. The cylindrical speed is $\mathbf v^2=\dot\rho^2+\rho^2\dot\theta^2+\dot z^2$. Inside a uniform axial field, choose the symmetric [magnetic vector potential](../../../../magnetic-vector-potential.md) $A_\theta=B\rho/2$, $A_\rho=A_z=0$. Its cylindrical curl gives $B_z=\rho^{-1}\partial_\rho(\rho A_\theta)=B$. Hence

$$
\boxed{L=-mc^2\sqrt{1-\frac{\dot z^2+\dot\rho^2+\rho^2\dot\theta^2}{c^2}}+\frac{qB\rho^2\dot\theta}{2}}.
$$

In a field-free region far from either end one can use $A_\theta=0$, recovering the requested outside expression. The question's $V=-qB\rho^2\dot\theta/2$ is a velocity-dependent generalized potential, not electrostatic potential [energy](../../../../energy-split.md).

There is an important end-field qualification. A finite axial field that jumps to zero with no radial component would violate [Gauss's law for magnetism](../../../../gauss-s-law-for-magnetism.md). The consistent near-axis idealisation is the [solenoid fringe field from an axisymmetric vector potential](../../../../solenoid-fringe-field-from-an-axisymmetric-vector-potential.md), $A_\theta=\rho B(z)/2$, giving $B_\rho=-\rho B'(z)/2$ and $B_z=B(z)$. The piecewise [Lagrangian](../../../../lagrangian.md) is its hard-edge limit and retains fringe impulses through the jump in $A_\theta$. Those impulses are essential to the focusing calculation.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
