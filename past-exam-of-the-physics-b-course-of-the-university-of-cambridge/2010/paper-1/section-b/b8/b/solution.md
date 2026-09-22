<h1 id="section-b/b8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A freely rotating [rigid body](../../../../../../rigid-body-dynamics-split.md) with no external [torque](../../../../../../torque.md) conserves its inertial [angular momentum](../../../../../../angular-momentum.md) and [kinetic energy](../../../../../../kinetic-energy.md). In body-fixed [principal axes](../../../../../../principal-axis.md), the Euler equations include

$$
I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3=0
$$

and cyclic permutations. The body can still change its orientation relative to its fixed angular-momentum vector; zero [torque](../../../../../../torque.md) does not require every [principal axis](../../../../../../principal-axis.md) to remain fixed.

For a [symmetric top](../../../../../../symmetric-top.md), $I_1=I_2=I_\perp$, $I_3=I_\parallel$. The axial rate $\omega_3$ is constant, and $\omega_1+i\omega_2$ rotates in body coordinates with signed [frequency](../../../../../../frequency.md) $(I_\parallel-I_\perp)\omega_3/I_\perp$. In space,

$$
\mathbf L=I_\perp\boldsymbol\omega+(I_\parallel-I_\perp)\omega_3\hat{\mathbf e}_3,
\qquad
\dot{\hat{\mathbf e}}_3=\frac{\mathbf L}{I_\perp}\times\hat{\mathbf e}_3.
$$

Thus the [symmetry](../../../../../../symmetry-physics.md) axis precesses about fixed $\mathbf L$ at rate $L/I_\perp$ and constant inclination. This [body-frame and space-frame frequencies of free symmetric-top precession](../../../../../../body-frame-and-space-frame-frequencies-of-free-symmetric-top-precession.md) distinction avoids confusing two different frame-dependent rates. A sphere has no dynamically distinguished [symmetry](../../../../../../symmetry-physics.md) axis even though a chosen body marker rotates.

For a general body, rotations about the largest and smallest principal inertias are stable to small perturbations, while rotation about the intermediate inertia is unstable. With $I_1<I_2<I_3$ and rotation $\omega_2=\Omega$, linearization gives $\ddot\omega_1=\Omega^2(I_3-I_2)(I_2-I_1)\omega_1/(I_1I_3)$, showing exponential growth. This is torque-free motion, distinct from the gravity-driven [precession](../../../../../../precession.md) of a supported [gyroscope](../../../../../../gyroscope.md).

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2010](../../../../split.md)
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
