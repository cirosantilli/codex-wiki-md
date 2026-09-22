<h1 id="section-b/b8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose body-fixed [principal axes](../../../../../../principal-axis.md) through a fixed point or the centre of [mass](../../../../../../mass.md), with principal moments $I_1,I_2,I_3$. [Angular momentum](../../../../../../angular-momentum.md) has components $L_i=I_i\omega_i$. The inertial [derivative](../../../../../../derivative.md) is the body [derivative](../../../../../../derivative.md) plus $\boldsymbol\omega\times\mathbf L$, so [Euler's equations](../../../../../../euler-s-equations-rigid-body-dynamics.md) read

$$
\boxed{I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3=\tau_1,\quad
I_2\dot\omega_2+(I_1-I_3)\omega_3\omega_1=\tau_2,\quad
I_3\dot\omega_3+(I_2-I_1)\omega_1\omega_2=\tau_3.}
$$

They avoid differentiating the rotating [inertia tensor](../../../../../../inertia-tensor.md) in laboratory coordinates. [Torques](../../../../../../torque.md) must refer to the chosen point, and the displayed fixed moments require a [rigid body](../../../../../../rigid-body-dynamics-split.md).

For zero [torque](../../../../../../torque.md), laboratory [angular momentum](../../../../../../angular-momentum.md) is constant, while its components can change in the body frame. Both $L^2$ and rotational [kinetic energy](../../../../../../kinetic-energy.md) $T=\tfrac12\sum I_i\omega_i^2$ are conserved. The intersections of their constant-value surfaces constrain the motion. For distinct $I_1<I_2<I_3$, steady rotation about either extreme [principal axis](../../../../../../principal-axis.md) is stable against small perturbations, whereas rotation about the intermediate axis is unstable. For example perturbing rotation $\Omega$ about axis 2 gives

$$
\ddot{\delta\omega_1}=
\Omega^2\frac{(I_2-I_3)(I_1-I_2)}{I_1I_3}\,\delta\omega_1,
$$

whose coefficient is positive. A symmetric body has additional simplifications and can precess. **Conservation of laboratory [angular momentum](../../../../../../angular-momentum.md) does not imply constant body-frame [angular velocity](../../../../../../angular-velocity.md).**

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2012](../../../../split.md)
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
