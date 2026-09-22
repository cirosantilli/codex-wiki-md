<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the constant [mass density](../../../../../../density.md) be $\rho>0$ and put $\mathbf v_a=\mathbf B/\sqrt{\mu_0\rho}$, the [Alfvén velocity](../../../../../../alfven-velocity.md). Since both the [velocity](../../../../../../velocity.md) and the [magnetic field](../../../../../../magnetic-field.md) have zero [divergence](../../../../../../divergence.md), the [magnetic tension](../../../../../../magnetic-tension.md) and [magnetic pressure](../../../../../../magnetic-pressure.md) decomposition of the [Lorentz force](../../../../../../lorentz-force.md) gives

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla\psi+(\mathbf v_a\cdot\nabla)\mathbf v_a,\qquad
\partial_t\mathbf v_a+(\mathbf u\cdot\nabla)\mathbf v_a=(\mathbf v_a\cdot\nabla)\mathbf u,
\qquad
\boxed{\psi=\frac p\rho+\Phi+\frac{|\mathbf v_a|^2}{2}.}
$$

The [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) $\Phi$ remains in $\psi$; uniform [mass density](../../../../../../density.md) does not justify dropping a prescribed [gravitational acceleration](../../../../../../gravitational-acceleration.md). Adding and subtracting the two equations proves the [Elsässer variable](../../../../../../elsasser-variable.md) equations

$$
\boxed{\partial_t\mathbf z^\pm+(\mathbf z^\mp\cdot\nabla)\mathbf z^\pm=-\nabla\psi,\qquad \nabla\cdot\mathbf z^\pm=0.}
$$

Here $\mathbf z^\pm=\mathbf u\pm\mathbf v_a$; each [Elsässer variable](../../../../../../elsasser-variable.md) is transported by the other.

Define $I_\pm=\int_V|\mathbf z^\pm|^2\,dV$. Taking the [dot product](../../../../../../dot-product.md) with $2\mathbf z^\pm$ gives the [Elsässer energy invariant](../../../../../../elsasser-energy-invariant.md) balance

$$
\partial_t|\mathbf z^\pm|^2+\nabla\cdot\left(|\mathbf z^\pm|^2\mathbf z^\mp+2\psi\mathbf z^\pm\right)=0.
$$

The [divergence theorem](../../../../../../divergence-theorem.md) proves $dI_\pm/dt=0$ whenever the net boundary flux vanishes. In particular, $\mathbf u\cdot\mathbf n=\mathbf B\cdot\mathbf n=0$ makes $\mathbf z^\pm\cdot\mathbf n=0$, so both fluxes vanish pointwise. [Periodic boundary conditions](../../../../../../periodic-boundary-conditions.md) or decay at infinity are also sufficient. These [boundary conditions](../../../../../../boundary-condition.md) matter: fixed volume alone gives no conservation.

The [kinetic energy](../../../../../../kinetic-energy.md) plus [magnetic energy](../../../../../../magnetic-energy.md) is

$$
E=\frac{\rho}{2}\int_V\left(u^2+v_a^2\right)dV.
$$

Expanding $|\mathbf u\pm\mathbf v_a|^2$ and using the [cross-helicity](../../../../../../cross-helicity.md) definition yields

$$
\boxed{E=\frac{\rho}{4}(I_++I_-),\qquad H_c=\frac{\sqrt{\mu_0\rho}}{4}(I_+-I_-),\qquad I_\pm=\frac{2E}{\rho}\pm\frac{2H_c}{\sqrt{\mu_0\rho}}.}
$$

Both [energy](../../../../../../energy.md) and [cross-helicity](../../../../../../cross-helicity.md) therefore follow from the two [Elsässer energy invariants](../../../../../../elsasser-energy-invariant.md). The quantity $E$ here is exactly the requested [kinetic energy](../../../../../../kinetic-energy.md) plus [magnetic energy](../../../../../../magnetic-energy.md), without an additional gravitational term.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
