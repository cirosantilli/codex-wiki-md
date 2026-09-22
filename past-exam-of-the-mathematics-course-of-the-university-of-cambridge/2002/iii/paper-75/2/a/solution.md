<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use physical momentum $p_{\mathrm{phys}}$ and conserved-background [comoving momentum](../../../../../../comoving-momentum.md) $q=a p_{\mathrm{phys}}$. At fixed $q$, the homogeneous collisionless [phase-space distribution function](../../../../../../phase-space-distribution-function.md) is $f_0(q)$, with no spatial or angular dependence and no explicit background time derivative. The printed relation $p_i=aqn_i$ cannot have this meaning: freely propagating physical momentum redshifts as $a^{-1}$, so it should read $p_i=q n_i/a$. Keeping the printed relation literally would give $q=p_{\mathrm{phys}}/a$ and a nonzero zeroth-order redshift, inconsistent with the target equation. The standard definition is positively confirmed by [the phase-space convention in Ma and Bertschinger's perturbation treatment](https://arxiv.org/html/astro-ph/9506072).

With this conserved $q$, the orders of the factors are:

- $\partial_t f=\partial_t f_1$ is first order; the zeroth-order collisionless equation has already made $\partial_t f_0=0$.
- $\partial_{x^i}f$ is first order, while $dx^i/dt$ has a zeroth-order free-streaming velocity and first-order corrections. Their product contributes at first order only through that background velocity.
- $\partial_qf=f_0'(q)+\partial_qf_1$ begins at zeroth order; $dq/dt$ begins at first order. Its leading product is $f_0'\dot q_1$.
- $\partial_{n^i}f=\partial_{n^i}f_1$ begins at first order, and $dn^i/dt$ begins at first order because background trajectories keep their direction. Their product is second order and drops out.

Thus the linear [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) is

$$
\boxed{\partial_t f_1+v_0^i\partial_{x^i}f_1+\dot q_1 f_0'(q)=0.}
$$

For photons $v_0^i=n^i/a$. For a particle of mass $m$, $v_0^i=q n^i/[a\sqrt{q^2+a^2m^2}]$. The order counting does not assume that the first-order angular deflection itself vanishes; only its multiplication by an already perturbed angular distribution makes it higher order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
