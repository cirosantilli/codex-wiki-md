<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Work at one radius and write $\mathcal R=k/(\mu_m m_p)$. Use the [surface density](../../../../../../surface-density-of-a-disk.md) to fix the [mass density](../../../../../../density.md) normalization and introduce the height scale

$$
h^6=\frac{3\alpha\kappa\Sigma^2\mathcal R^4}{16\sigma\Omega^5}.
$$

Choose the dimensionless variables

$$
z=h\zeta,\qquad \rho=\frac\Sigma h D,\qquad p=\Sigma\Omega^2hP,\qquad T=\frac{\Omega^2h^2}{\mathcal R}\Theta,\qquad F=\alpha\Sigma\Omega^3h^2Q.
$$

The [pressure](../../../../../../pressure.md) and [temperature](../../../../../../temperature.md) scales make the hydrostatic and [ideal gas](../../../../../../ideal-gas.md) equations parameter-free. The [flux](../../../../../../flux.md) scale fixes the heating coefficient at $9/4$, and the choice of $h$ makes the diffusion coefficient unity. Direct substitution gives the universal [ordinary differential equations](../../../../../../ordinary-differential-equation.md)

$$
\boxed{\frac{dP}{d\zeta}=-D\zeta,\qquad \frac{dQ}{d\zeta}=\frac94P,\qquad \frac{d\Theta}{d\zeta}=-\frac{DQ}{\Theta^3},\qquad P=D\Theta.}
$$

For example, the dimensionless coefficient in the [temperature](../../../../../../temperature.md) equation is $3\alpha\kappa\Sigma^2\mathcal R^4/(16\sigma\Omega^5h^6)=1$.

Let the upper free surface be at $\zeta=\zeta_s$, so its physical semithickness is $H=h\zeta_s$. Midplane [symmetry](../../../../../../symmetry-physics.md) and the [radiative-zero disk surface](../../../../../../radiative-zero-disk-surface.md) conditions give

$$
\boxed{Q(0)=0,\qquad P(\zeta_s)=\Theta(\zeta_s)=0,\qquad 2\int_0^{\zeta_s}D\,d\zeta=1.}
$$

The last condition is precisely $\Sigma=\int_{-H}^H\rho\,dz$. The unknown surface position and the two positive midplane values $P(0),\Theta(0)$ are determined as part of the normalized [boundary value problem](../../../../../../boundary-value-problem.md). [Symmetry](../../../../../../symmetry-physics.md) makes $P,D,\Theta$ even and $Q$ odd; $P'(0)=\Theta'(0)=0$ already follow from the equations and are not additional independent [boundary conditions](../../../../../../boundary-condition.md).

The zero conditions do not mean zero surface [flux](../../../../../../flux.md). Integrating the heating equation gives $Q(\zeta_s)=(9/4)\int_0^{\zeta_s}P\,d\zeta>0$. Near a regular surface with finite outgoing [flux](../../../../../../flux.md), dividing the hydrostatic equation by the [temperature](../../../../../../temperature.md) equation yields $dP/d\Theta\simeq\zeta_s\Theta^3/Q_s$. Thus $P\propto\Theta^4$, $D\propto\Theta^3$ and $\Theta\propto\zeta_s-\zeta$, so [mass density](../../../../../../density.md) also vanishes. The apparent singular quotient in the diffusion equation has a finite regular limit. All [boundary conditions](../../../../../../boundary-condition.md) and equations are independent of the physical parameters: this is [homologous vertical structure of a constant-opacity alpha disk](../../../../../../homologous-vertical-structure-of-a-constant-opacity-alpha-disk.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
