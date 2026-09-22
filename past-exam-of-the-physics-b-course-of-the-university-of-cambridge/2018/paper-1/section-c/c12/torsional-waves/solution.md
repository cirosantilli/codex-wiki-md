<h1 id="section-c/c12/torsional-waves/solution">Solution</h1>

↑ **Parent:** [Torsional waves](../torsional-waves.md)

**The torque difference.** Let $\phi(x,t)$ now be the local angular displacement, and take $G$ and the section constant. The local twist per unit length is $\partial_x\phi$, so the transmitted torque is $C(x,t)=GJ_p\partial_x\phi$. Across a short slice,

$$
\Delta C=C(x+\Delta x)-C(x)
=GJ_p\frac{\partial^2\phi}{\partial x^2}\Delta x+O(\Delta x^2).
$$

Thus

$$
\boxed{\Delta C=\frac{\pi a^4G}{2}
\frac{\partial^2\phi}{\partial x^2}\Delta x}
$$

to first order in slice length.

**The slice's angular acceleration.** The slice's axial [moment of inertia](../../../../../../moment-of-inertia.md) is $\Delta I=\rho J_p\Delta x$. Its net torque is the difference of the end torques, so

$$
\rho J_p\Delta x\,\partial_t^2\phi
=GJ_p\Delta x\,\partial_x^2\phi.
$$

Canceling the common geometry gives the [torsional waves in a solid circular rod](../../../../../../torsional-waves-in-a-solid-circular-rod.md),

$$
\boxed{\frac{\partial^2\phi}{\partial t^2}
=\frac G\rho\frac{\partial^2\phi}{\partial x^2},\qquad
c_t=\sqrt{\frac G\rho}.}
$$

For the given steel, $c_t\simeq3.16\times10^3\ \mathrm{m\,s^{-1}}$. The radius cancels because both torsional stiffness and slice inertia contain the same $J_p$. This ideal one-dimensional wave model neglects dissipation and additional elastic modes.

## ↑ Ancestors (15)

1. [Torsional waves](../torsional-waves.md)
2. [C12](../../c12.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
