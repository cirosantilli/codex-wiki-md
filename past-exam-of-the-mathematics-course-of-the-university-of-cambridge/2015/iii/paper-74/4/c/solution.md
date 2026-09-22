<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply [volume conservation](../../../../../../volume-conservation.md), [mass conservation](../../../../../../mass-conservation.md) and vertical [momentum flux](../../../../../../momentum-flux.md) balance to a slice of the [triangular-profile line plume](../../../../../../triangular-profile-line-plume.md). Ambient ingestion contributes $2e$ of [volume](../../../../../../volume.md) and $2\rho_0e$ of [mass](../../../../../../mass.md) per unit height and source length. The ambient is quiescent, so it supplies no leading vertical [momentum](../../../../../../momentum.md). The integrated driving force is the stored [buoyancy](../../../../../../buoyancy.md) $\mathcal B$. Using the quantities from part (a), the [non-Boussinesq triangular-profile line-plume balances](../../../../../../non-boussinesq-triangular-profile-line-plume-balances.md) are

$$
\boxed{\begin{aligned}
\partial_t(2b)+\partial_z(bW)&=2e,\\
\partial_t[b(\rho+\rho_0)]+\partial_z\left[\frac{bW}{3}(\rho_0+2\rho)\right]&=2\rho_0e,\\
\partial_t\left[\frac{bW}{3}(\rho_0+2\rho)\right]+\partial_z\left[\frac{bW^2}{6}(\rho_0+3\rho)\right]&=gb(\rho_0-\rho).
\end{aligned}}
$$

Together with [Batchelor entrainment](../../../../../../batchelor-entrainment-hypothesis.md), these are three equations for $W,\rho,b$. They neglect viscous boundary stresses and streamwise pressure-force corrections within the integral-plume approximation.

Multiplying [volume](../../../../../../volume.md) conservation by $g\rho_0$ and subtracting $g$ times [mass conservation](../../../../../../mass-conservation.md) cancels the ambient sources exactly, giving

$$
\boxed{\partial_t[gb(\rho_0-\rho)]+\partial_z\left[\frac23gbW(\rho_0-\rho)\right]=0.}
$$

This is [buoyancy](../../../../../../buoyancy.md) conservation in the homogeneous ambient; it is a consequence of the first two balances, not an additional independent equation.

Now take the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) in inertia and entrainment, retaining the small density deficit in [buoyancy](../../../../../../buoyancy.md). Then $Q=\rho_0bW$, $M=(2/3)\rho_0bW^2$ and $F=(2/3)gbW(\rho_0-\rho)$. Consequently

$$
W=\frac32\frac MQ,\qquad 2\rho_0b=\frac43\frac{Q^2}{M},\qquad \mathcal B=\frac{FQ}{M}.
$$

The [mass](../../../../../../mass.md) source is $2\alpha\rho_0W=3\alpha\rho_0M/Q$. Substitution into the [mass conservation](../../../../../../mass-conservation.md), [momentum](../../../../../../momentum.md) and [buoyancy](../../../../../../buoyancy.md) balances gives the [unsteady Boussinesq triangular-profile line-plume balances](../../../../../../unsteady-boussinesq-triangular-profile-line-plume-balances.md)

$$
\boxed{\begin{aligned}
\frac43\partial_t\left(\frac{Q^2}{M}\right)+\partial_zQ&=3\alpha\rho_0\frac MQ,\\
\partial_tQ+\partial_zM&=\frac{FQ}{M},\\
\partial_t\left(\frac{FQ}{M}\right)+\partial_zF&=0.
\end{aligned}}
$$

These use density-weighted [mass](../../../../../../mass.md) and [momentum](../../../../../../momentum.md) fluxes. Removing $\rho_0$ from some flux definitions while retaining it in the source would mix incompatible conventions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
