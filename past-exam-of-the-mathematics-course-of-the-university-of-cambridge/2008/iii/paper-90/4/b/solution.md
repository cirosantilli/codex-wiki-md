<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep the half-section convention of part (a). Define the [mass density](../../../../../../density.md)-weighted [mass flux](../../../../../../mass-flux.md), [buoyancy flux](../../../../../../buoyancy-flux.md) and [momentum flux](../../../../../../momentum-flux.md) by

$$
\boxed{Q=\rho bw,\qquad F=(\rho_0-\rho)gbw,\qquad M=\rho bw^2.}
$$

The full-section fluxes are $2Q,2F,2M$. These factors must be changed consistently if full fluxes are used; mixing a full-width flux with a half-width [entrainment](../../../../../../fluid-entrainment.md) source would introduce a spurious factor two.

For positive $Q,M$, $w=M/Q$, $\rho b=Q^2/M$, and $(\rho_0-\rho)gb=FQ/M$. The mass equation in part (a), the momentum equation, and the [buoyancy](../../../../../../buoyancy.md) equation therefore become

$$
\boxed{
\begin{aligned}
\partial_t(Q^2/M)+Q_z&=\rho_0\alpha M/Q,\\
Q_t+M_z&=FQ/M,\\
\partial_t(FQ/M)+F_z&=-\frac{\rho_0}{\rho}N^2Q.
\end{aligned}}
$$

These are direct algebraic rewritings with the [mass density](../../../../../../density.md) factors retained. In particular, $FQ/M$ is the [buoyancy](../../../../../../buoyancy.md) inventory per unit height as well as the integrated [buoyancy](../../../../../../buoyancy.md) force. If desired, $\rho$ can be reconstructed from $F/(gQ)=\rho_0/\rho-1$.

At leading [Boussinesq](../../../../../../boussinesq-approximation.md) order use a constant reference [mass density](../../../../../../density.md) $R$ in the inertial fluxes, $Q=Rbw$, $M=Rbw^2$, and write $g'=g(\rho_0-\rho)/R$ so $F=Rg'bw$. Set $\rho_0/\rho=1$ in the [stratification](../../../../../../density-stratification.md) source and use $N^2\simeq-g\rho_0'/R$. The [unsteady top-hat line-plume balances](../../../../../../unsteady-top-hat-line-plume-balances.md) are then

$$
\boxed{\partial_t(Q^2/M)+Q_z=R\alpha M/Q,\qquad
Q_t+M_z=FQ/M,\qquad
\partial_t(FQ/M)+F_z=-N^2Q.}
$$

Equivalently the kinematic fluxes $q=Q/R=bw$, $m=M/R=bw^2$ and $f=F/R=g'bw$ obey the same equations with $R$ removed from the first source. This explicit distinction between [mass density](../../../../../../density.md)-weighted and kinematic fluxes fixes the normalization for the power-law solution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
