<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $u^\lambda u_\lambda=-c^2$ and a constant [Minkowski metric](../../../../minkowski-metric.md). Vary the velocity-dependent square root **before** imposing the proper-time normalization. Equivalently, vary a reparametrization-invariant [worldline](../../../../world-line.md) action first and then choose [proper time](../../../../proper-time.md). Its canonical covector momentum is

$$
\frac{\partial\mathcal L}{\partial u^a}
=mc\frac{u_a}{\sqrt{-u^2}}+qA_a
\ \longrightarrow\ m u_a+qA_a.
$$

The coordinate derivative at fixed velocity is $\partial\mathcal L/\partial x^a=q u^\lambda\partial_aA_\lambda$. The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) and the [chain rule](../../../../chain-rule.md) from [a](../a.md) therefore give

$$
m\dot u_a+q u^\lambda\partial_\lambda A_a
=q u^\lambda\partial_a A_\lambda.
$$

Define the antisymmetric field tensor by

$$
\boxed{F_{ab}=\partial_aA_b-\partial_bA_a,\qquad
F^{ab}=\partial^aA^b-\partial^bA^a.}
$$

The particle equation becomes

$$
\boxed{m\frac{du_a}{d\tau}=qF_{a\lambda}u^\lambda.}
$$

Antisymmetry ensures $u^aF_{a\lambda}u^\lambda=0$, so the force is orthogonal to the [four-velocity](../../../../four-velocity.md) and preserves $u^2=-c^2$. The [worldline variation before proper-time normalization](../../../../worldline-variation-before-proper-time-normalization.md) is essential: substituting $\sqrt{-u^2}=c$ into the [Lagrangian](../../../../lagrangian.md) **before taking its velocity derivative** would turn the kinetic term into a constant and incorrectly remove the inertial momentum. The normalization is a property of the proper-time solution, not permission to discard the variational dependence.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
