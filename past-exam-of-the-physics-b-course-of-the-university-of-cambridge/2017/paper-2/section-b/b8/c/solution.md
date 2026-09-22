<h1 id="section-b/b8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take axes fixed in a [rigid body](../../../../../../rigid-body-dynamics-split.md), chosen along its [principal axes](../../../../../../principal-axis.md), with moments of inertia $I_1,I_2,I_3$. The [angular momentum](../../../../../../angular-momentum.md) components are $H_i=I_i\omega_i$. Newton's rotational equation is $\boldsymbol\tau=(d\mathbf H/dt)_{\rm inertial}$, while the rotating-frame transport rule gives

$$
\left(\frac{d\mathbf H}{dt}\right)_{\rm inertial}
=\left(\frac{d\mathbf H}{dt}\right)_{\rm body}+\boldsymbol\omega\times\mathbf H.
$$

Thus [Euler's equations](../../../../../../euler-s-equations-rigid-body-dynamics.md) are

$$
\boxed{\begin{aligned}
I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3&=\tau_1,\\
I_2\dot\omega_2+(I_1-I_3)\omega_3\omega_1&=\tau_2,\\
I_3\dot\omega_3+(I_2-I_1)\omega_1\omega_2&=\tau_3.
\end{aligned}}
$$

The nonlinear cross terms arise because the [principal axes](../../../../../../principal-axis.md) rotate. Even with no external [torque](../../../../../../torque.md), the body-frame components of [angular momentum](../../../../../../angular-momentum.md) can vary while the [angular momentum](../../../../../../angular-momentum.md) [vector](../../../../../../vector.md) stays fixed in inertial space.

With zero [torque](../../../../../../torque.md), the equations conserve

$$
E=\tfrac12\sum_i I_i\omega_i^2,\qquad
H^2=\sum_iI_i^2\omega_i^2.
$$

Uniform [rotation](../../../../../../rotation-mathematics.md) about any [principal axis](../../../../../../principal-axis.md) is a torque-free solution. If $I_1<I_2<I_3$, [linearization](../../../../../../linearization.md) about the intermediate-axis solution $\omega_2=\Omega$ gives

$$
\delta\ddot\omega_1=\Omega^2\frac{(I_2-I_1)(I_3-I_2)}{I_1I_3}\delta\omega_1.
$$

The positive coefficient gives exponential growth: intermediate-axis [rotation](../../../../../../rotation-mathematics.md) is unstable, whereas [rotation](../../../../../../rotation-mathematics.md) about the largest or smallest moment is linearly stable. For a symmetric body, [Euler's equations](../../../../../../euler-s-equations-rigid-body-dynamics.md) also describe the [precession](../../../../../../precession.md) of the transverse [angular velocity](../../../../../../angular-velocity.md) around its [symmetry](../../../../../../symmetry-physics.md) axis. [Torques](../../../../../../torque.md) from gravity or an applied couple enter through the right-hand sides rather than being absorbed into the inertial cross terms.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
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
