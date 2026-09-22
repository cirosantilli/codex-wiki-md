<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md) makes the inward [entrainment velocity](../../../../../../entrainment-velocity.md) proportional to the local plume speed:

$$
\boxed{u_e=\alpha |w|,}
$$

where $\alpha>0$ is the dimensionless [entrainment coefficient](../../../../../../entrainment-coefficient.md). For an upward plume $w>0$, this is $u_e=\alpha w$. The hypothesis represents turbulent ingestion of ambient fluid; it is a closure rather than a consequence of [mass conservation](../../../../../../mass-conservation.md).

Let $A=b^2$, suppressing the common factor $\pi$ from cross-sectional integrals. In the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), use a constant reference [density](../../../../../../density.md) $\rho_r$ in the leading-order [mass conservation](../../../../../../mass-conservation.md) equation. Dividing that equation by $\rho_r$ gives [volume conservation](../../../../../../volume-conservation.md):

$$
\boxed{A_t+(Aw)_z=2b u_e.}
$$

The factor two is the ratio of the perimeter $2\pi b$ to the suppressed area factor $\pi$. [Density](../../../../../../density.md) differences are retained in [buoyancy](../../../../../../buoyancy.md), even though they are neglected in the leading inertial and volume terms.

To derive the density-deficit balance, first leave the small [density](../../../../../../density.md) differences explicit in the supplied mass equation. Because the ambient [density](../../../../../../density.md) $\rho_0(z)$ is time independent, the [product rule](../../../../../../product-rule.md) gives

$$
\begin{aligned}
\partial_t[(\rho_0-\rho)gA]+\partial_z[(\rho_0-\rho)gAw]
&=g\rho_0[A_t+(Aw)_z]+g\rho_{0z}Aw\\
&\quad-g[(\rho A)_t+(\rho Aw)_z]\\
&=g\rho_0(2bu_e)+g\rho_{0z}Aw-g(2\rho_0bu_e)\\
&=g\rho_{0z}Aw.
\end{aligned}
$$

Thus the ambient mass entrained through the perimeter cancels exactly against its contribution to the volume budget, yielding the required [buoyancy](../../../../../../buoyancy.md) balance. It is understood to the accuracy of the underlying [Boussinesq approximation](../../../../../../boussinesq-approximation.md); the volume equation is not an additional exact constraint on a fully variable-density fluid.

For later use define [reduced gravity](../../../../../../reduced-gravity-split.md) $g'=g(\rho_0-\rho)/\rho_r$ and the squared [buoyancy frequency](../../../../../../buoyancy-frequency.md) $N^2=-g\rho_{0z}/\rho_r$. With $B=Ag'$ and $Q=Aw$, the balance is

$$
\boxed{B_t+(Awg')_z=-N^2Q.}
$$

A stably stratified ambient has $N^2>0$, so upward motion consumes the plume's positive [density](../../../../../../density.md) deficit; an unstable ambient reverses this sign.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
