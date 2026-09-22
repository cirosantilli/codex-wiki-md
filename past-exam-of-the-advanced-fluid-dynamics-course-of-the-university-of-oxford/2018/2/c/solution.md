<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $S_a$ be the sphere surface, $\mathbf n_s$ point from the sphere into the fluid, and write

$$
\mathbf w=\mathbf u_S-\mathbf u_\infty,\qquad
\boldsymbol\tau=\boldsymbol\sigma_S-\boldsymbol\sigma_\infty.
$$

Because the prescribed exterior [body forces](../../../../body-force.md) are unchanged, they cancel on subtraction: the disturbance is a homogeneous [Stokes flow](../../../../stokes-flow-split.md) in the exterior domain. On the sphere the [no-slip boundary condition](../../../../no-slip-boundary-condition.md) is

$$
\mathbf w=\mathbf V+\boldsymbol\omega_s\times\mathbf x-\mathbf u_\infty,
$$

allowing an arbitrary sphere rotation $\boldsymbol\omega_s$.

Use as auxiliary flow the translating-sphere solution of part [b](../b.md), with arbitrary test [velocity](../../../../velocity.md) $\mathbf U$. Its surface [velocity](../../../../velocity.md) is $\mathbf U$ and its surface [traction](../../../../traction.md) is $-3\mu\mathbf U/(2a)$. Applying the [Lorentz reciprocal theorem](../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) on the exterior domain gives, after cancelling the common inner-normal minus sign,

$$
\int_{S_a}\mathbf w\cdot\boldsymbol\sigma^*\mathbf n_s\,dS
=\int_{S_a}\mathbf U\cdot\boldsymbol\tau\mathbf n_s\,dS.
$$

The outer surface terms vanish for decaying disturbances: velocities are at most $O(r^{-1})$, stresses $O(r^{-2})$, and the integrated cross-work is $O(r^{-1})$.

There are no [body forces](../../../../body-force.md) inside the sphere in the original ambient problem. Thus the smooth ambient [stress tensor](../../../../cauchy-stress-tensor.md) has zero divergence there, and

$$
\int_{S_a}\boldsymbol\sigma_\infty\mathbf n_s\,dS
=\int_{r<a}\nabla\cdot\boldsymbol\sigma_\infty\,dV=0.
$$

Also $\int_{S_a}\mathbf x\,dS=0$, so the rotation term drops out of the left side. Consequently the reciprocal identity reduces to

$$
-\frac{3\mu}{2a}\mathbf U\cdot
\left[4\pi a^2\mathbf V-\int_{S_a}\mathbf u_\infty\,dS\right]
=\mathbf U\cdot\mathbf F_H.
$$

Since $\mathbf U$ is arbitrary, the result before imposing mechanical balance is

$$
\boxed{\mathbf F_H=-6\pi\mu a\left[\mathbf V-
\frac1{4\pi a^2}\int_{S_a}\mathbf u_\infty\,dS\right].}
$$

For a freely suspended sphere with negligible inertia and no applied external [force](../../../../force-split.md), $\mathbf F_H=0$. Its [sphere velocity as a surface average of ambient Stokes flow](../../../../sphere-velocity-as-a-surface-average-of-ambient-stokes-flow.md) is therefore

$$
\boxed{\mathbf V=\frac1{4\pi a^2}\int_{|\mathbf x|=a}\mathbf u_\infty(\mathbf x)\,dS.}
$$

The implicit force-free condition is essential. More generally, an external [force](../../../../force-split.md) $\mathbf F_{\rm ext}$ gives $\mathbf V=\langle\mathbf u_\infty\rangle_{S_a}+\mathbf F_{\rm ext}/(6\pi\mu a)$. For example, an externally pulled sphere in the zero ambient flow has nonzero [velocity](../../../../velocity.md), contrary to an unrestricted surface-average-only claim. No torque-free assumption is needed for this translational identity, because the auxiliary surface traction is constant.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
