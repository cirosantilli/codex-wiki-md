<h1 id="3/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Let $\mathcal E=\langle|\mathbf u|^2\rangle/2$ be the turbulent [kinetic energy](../../../../../../kinetic-energy.md) per unit mass. In addition to $L>0$ and high [Reynolds number](../../../../../../reynolds-number.md), use the usual self-preserving large-eddy decay assumption: the normalized large-scale correlation has a fixed shape, so

$$
L=C_L\mathcal E\ell^3,\qquad \ell=\left(\frac{L}{C_L\mathcal E}\right)^{1/3},
$$

where $C_L>0$ is constant. For freely decaying high-Reynolds-number [turbulence](../../../../../../turbulence-split.md), the cascade [viscous dissipation](../../../../../../viscous-dissipation.md) law is $\epsilon=C_\epsilon\mathcal E^{3/2}/\ell$. The kinetic-energy balance therefore gives

$$
\frac{d\mathcal E}{dt}=-C_\epsilon C_L^{1/3}L^{-1/3}\mathcal E^{11/6}.
$$

Put $A=C_\epsilon C_L^{1/3}L^{-1/3}$. Integrating,

$$
\boxed{\mathcal E(t)=\left[\mathcal E(t_0)^{-5/6}+\frac56A(t-t_0)\right]^{-6/5}},
\qquad \boxed{\mathcal E\propto(t-t_*)^{-6/5},\quad \ell\propto(t-t_*)^{2/5}}.
$$

The constant $t_*$ is a virtual time origin. This is the [Saffman decay law](../../../../../../saffman-decay-law.md). The energy decreases while the [integral scale of turbulence](../../../../../../integral-scale-of-turbulence.md) grows so that the conserved large-volume [momentum](../../../../../../momentum.md) [variance](../../../../../../variance-split.md) remains constant.

The exponent does not follow from the invariant alone: it also uses unforced decay, one evolving large-eddy length and an asymptotically constant cascade [viscous dissipation](../../../../../../viscous-dissipation.md) coefficient. A changing normalized spectral shape or a confining boundary can invalidate that closure. Moreover $\mathrm{Re}\sim\mathcal E^{1/2}\ell/\nu\propto(t-t_*)^{-1/5}$, so at fixed [kinematic viscosity](../../../../../../kinematic-viscosity.md) the high-Reynolds-number decay regime eventually ends; the $-6/5$ law is not a claim about the ultimate viscous limit.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
