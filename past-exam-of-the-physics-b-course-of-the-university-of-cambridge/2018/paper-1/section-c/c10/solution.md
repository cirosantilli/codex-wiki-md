<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

**Inertia and principal directions.** About the centre of mass, the [inertia tensor](../../../../../inertia-tensor.md) is

$$
I_{ij}=\int(r^2\delta_{ij}-r_ir_j)\,dm.
$$

It relates [angular momentum](../../../../../angular-momentum.md) and [angular velocity](../../../../../angular-velocity.md) by $\mathbf J=\mathsf I\boldsymbol\omega$ and gives rotational [kinetic energy](../../../../../kinetic-energy.md) $T=\boldsymbol\omega\cdot\mathsf I\boldsymbol\omega/2$. The [principal axes](../../../../../principal-axis.md) are orthogonal [eigenvector](../../../../../eigenvector.md) directions of this real symmetric [tensor](../../../../../tensor.md); in that basis it is diagonal, with entries the [principal moments of inertia](../../../../../principal-moment-of-inertia.md) $I_1,I_2,I_3$.

**Derivatives in a rotating frame.** Write $\mathbf J=\sum_iJ_i\mathbf e_i$ in a body-fixed orthonormal basis. Each basis vector rotates according to $(d\mathbf e_i/dt)_0=\boldsymbol\omega\times\mathbf e_i$. Differentiating the components and basis separately proves the [rotating-frame derivative formula](../../../../../rotating-frame-derivative-formula.md),

$$
\boxed{\left.\frac{d\mathbf J}{dt}\right|_0
=\left.\frac{d\mathbf J}{dt}\right|_{\rm body}
+\boldsymbol\omega\times\mathbf J.}
$$

The body derivative differentiates the scalar components in that basis. A fixed pivot can replace the centre of mass when the corresponding angular-momentum balance is valid.

**Euler equations.** The inertial angular-momentum equation is $d\mathbf J/dt=\mathbf G$. Since the principal moments are constant in the body frame, substitute $J_i=I_i\omega_i$:

$$
\boxed{\begin{aligned}
G_1&=I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3,\\
G_2&=I_2\dot\omega_2+(I_1-I_3)\omega_3\omega_1,\\
G_3&=I_3\dot\omega_3+(I_2-I_1)\omega_1\omega_2.
\end{aligned}}
$$

These are [Euler's equations](../../../../../euler-s-equations-rigid-body-dynamics.md) in the [principal body frame](../../../../../principal-body-frame.md).

**Linear perturbation of free rotation.** After the impulse, $\mathbf G=0$. Let $\omega_3=\Omega$ to leading order and $\omega_1,\omega_2$ be small. The third Euler equation changes $\omega_3$ only at quadratic order, so the linear transverse equations are

$$
I_1\dot\omega_1=(I_2-I_3)\Omega\omega_2,\qquad
I_2\dot\omega_2=(I_3-I_1)\Omega\omega_1.
$$

For $\omega_1=ae^{pt}$ and $\omega_2=be^{pt}$, eliminate $a,b$ from

$$
I_1pa=(I_2-I_3)\Omega b,\qquad
I_2pb=(I_3-I_1)\Omega a.
$$

This gives

$$
\boxed{p^2=\Omega^2\frac{(I_2-I_3)(I_3-I_1)}{I_1I_2}.}
$$

Its units are inverse square seconds. Positive $p^2$ gives a growing real exponential; negative $p^2$ gives bounded oscillatory perturbations.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
