<h1 id="section-b/b8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A torque-free [rigid body](../../../../../../rigid-body-dynamics-split.md) has constant [angular momentum](../../../../../../angular-momentum.md) $\mathbf L$ in inertial space. Its [angular velocity](../../../../../../angular-velocity.md) need not be parallel to $\mathbf L$, because $\mathbf L=\mathbf I\boldsymbol\omega$. In body principal axes, [Euler equations for a torque-free rigid body](../../../../../../euler-equations-for-a-torque-free-rigid-body.md) are

$$
I_1\dot\omega_1=(I_2-I_3)\omega_2\omega_3,\quad I_2\dot\omega_2=(I_3-I_1)\omega_3\omega_1,\quad I_3\dot\omega_3=(I_1-I_2)\omega_1\omega_2.
$$

For a [symmetric top](../../../../../../symmetric-top.md) $I_1=I_2=I_\perp$, $I_3=I_\parallel$, the component $\omega_3$ is constant and

$$
\boxed{\omega_1+i\omega_2=C e^{i\Omega_b t},\qquad\Omega_b=\frac{I_\parallel-I_\perp}{I_\perp}\omega_3.}
$$

This is the signed rotation frequency of the transverse angular-velocity components in the body frame. In space the symmetry axis instead obeys

$$
\dot{\mathbf e}_3=\frac{\mathbf L}{I_\perp}\times\mathbf e_3,\qquad\boxed{\Omega_{\rm space}=L/I_\perp.}
$$

Its angle to $\mathbf L$ is constant, with $\cos\theta=I_\parallel\omega_3/L$. The [body-frame and space-frame frequencies of free symmetric-top precession](../../../../../../body-frame-and-space-frame-frequencies-of-free-symmetric-top-precession.md) describe different frames. A spherical body has $\boldsymbol\omega\parallel\mathbf L$ and no corresponding wobble. For a triaxial body, rotations about the largest and smallest principal-inertia axes are stable, whereas rotation about the intermediate axis is unstable.[Sections 3.4.2–3.4.3: free symmetric top and stability of the asymmetric top](../../../../../../classical-dynamics-by-david-tong.md)

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2015](../../../../split.md)
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
