<h1 id="section-b/b8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For positions measured from the chosen origin, the [inertia tensor](../../../../../../inertia-tensor.md) is

$$
\boxed{I_{ij}=\int\rho(\mathbf r)(r^2\delta_{ij}-x_ix_j)\,d^3r.}
$$

It relates [angular momentum](../../../../../../angular-momentum.md) and [rotational kinetic energy](../../../../../../rotational-kinetic-energy.md) to [angular velocity](../../../../../../angular-velocity.md):

$$
\mathbf L=\mathbf I\boldsymbol\omega,\qquad T_{\rm rot}=\tfrac12\boldsymbol\omega\cdot\mathbf I\boldsymbol\omega.
$$

The real symmetric tensor has orthogonal principal axes, in which $\mathbf I=\operatorname{diag}(I_1,I_2,I_3)$. Its [eigenvalues](../../../../../../eigenvalue.md) are nonnegative moments of inertia. Rotation about a [principal axis](../../../../../../principal-axis.md) has $\mathbf L\parallel\boldsymbol\omega$; a general rotation does not. The moment about a unit axis $\mathbf n$ is $I_{\mathbf n}=\mathbf n\cdot\mathbf I\mathbf n$.

Changing from the centre of mass to a parallel origin displaced by $\mathbf a$ gives the [tensor parallel-axis theorem](../../../../../../tensor-parallel-axis-theorem.md),

$$
\boxed{\mathbf I_O=\mathbf I_{\rm CM}+M(a^2\mathbf 1-\mathbf a\mathbf a^{\mathsf T}).}
$$

For example, a uniform solid sphere has $\mathbf I=(2MR^2/5)\mathbf1$, while a thin rod along $x$ has principal moments $0,Ml^2/12,Ml^2/12$ in the ideal zero-radius limit. The tensor is needed to describe off-axis rotation and torque-free [precession](../../../../../../precession.md); a single scalar inertia only suffices after an axis is specified.[Sections 3.1–3.3: inertia tensor, principal axes and the parallel-axis theorem](../../../../../../classical-dynamics-by-david-tong.md)

## ↑ Ancestors (15)

1. [C](../c.md)
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
