<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take inward [fluid entrainment](../../../../../../fluid-entrainment.md) speed to be positive. The non-Boussinesq form of the [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md) is

$$
\boxed{v_e=\alpha w\sqrt{\rho/\rho_0},}
$$

where $\alpha$ is the [entrainment coefficient](../../../../../../entrainment-coefficient.md). Define physical, cross-section-integrated fluxes for the [top-hat plume model](../../../../../../top-hat-plume-model.md) by

$$
\boxed{Q=\pi b^2\rho w,\qquad M=\pi b^2\rho w^2,\qquad
F=\pi b^2w g(\rho_0-\rho).}
$$

Thus $Q$ is [mass flux](../../../../../../mass-flux.md), $M$ is [momentum flux](../../../../../../momentum-flux.md), and $F$ is a density-weighted [buoyancy flux](../../../../../../buoyancy-flux.md). The kinematic buoyancy flux in the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) is $F/\rho_0$. These definitions keep the factor $\pi$; conventions suppressing it simply rescale all three fluxes consistently.

For a homogeneous ambient, the sectional volume, mass and momentum balances are

$$
\partial_t(\pi b^2)+\partial_z(\pi b^2w)=2\pi b v_e,
$$



$$
\partial_t(\pi b^2\rho)+\partial_zQ=2\pi b\rho_0v_e,\qquad
\partial_tQ+\partial_zM=\pi b^2g(\rho_0-\rho).
$$

The momentum source is the net upward [buoyancy](../../../../../../buoyancy.md) force; entrained ambient fluid initially supplies no vertical momentum. Subtracting the mass balance from $\rho_0$ times the volume balance gives conservation of the density deficit:

$$
\partial_t[\pi b^2g(\rho_0-\rho)]+\partial_zF=0.
$$

Now $w=M/Q$, $\pi b^2\rho=Q^2/M$, and $\pi b^2g(\rho_0-\rho)=QF/M$. Substitution produces the [non-Boussinesq top-hat plume equations](../../../../../../non-boussinesq-top-hat-plume-equations.md)

$$
\boxed{\partial_t\left(\frac{Q^2}{M}\right)+\partial_zQ=2\alpha\sqrt{\pi\rho_0M},\qquad
\partial_tQ+\partial_zM=\frac{QF}{M},\qquad
\partial_t\left(\frac{QF}{M}\right)+\partial_zF=0.}
$$

For reconstructing the fields without a [Boussinesq approximation](../../../../../../boussinesq-approximation.md),

$$
\rho=\frac{\rho_0gQ}{gQ+F},\qquad b^2=\frac{Q^2}{\pi\rho M},\qquad
\frac{g(\rho_0-\rho)}\rho=\frac FQ.
$$

The last expression uses the plume density in the acceleration denominator; it agrees with the ambient-density definition of [reduced gravity](../../../../../../reduced-gravity-split.md) to Boussinesq order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
