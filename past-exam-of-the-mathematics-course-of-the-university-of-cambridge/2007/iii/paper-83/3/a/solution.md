<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\nu=\mu/\rho$ and average the horizontal [Navier-Stokes equation](../../../../../../navier-stokes-equation.md), with zero-mean fluctuations and [incompressible flow](../../../../../../incompressible-flow.md). The mean flow is stationary, has no vertical [velocity](../../../../../../velocity.md) and has no horizontal [pressure](../../../../../../pressure.md) gradient. The mean advection of $U(z)$ is therefore zero. Incompressibility rewrites the averaged nonlinear fluctuation term as a divergence:

$$
\overline{u'_j\partial_j u'}=\partial_j\overline{u'_j u'}.
$$

These correlations transport mean momentum and produce [Reynolds stress](../../../../../../reynolds-stress.md). Horizontal statistical homogeneity makes the horizontal derivatives of the averaged correlations vanish. It does not require the instantaneous turbulent derivatives themselves to vanish. Only the vertical divergence remains, giving

$$
\boxed{0=\nu U_{zz}-\frac{d}{dz}\overline{u'w'}.}
$$

Multiplying by [density](../../../../../../density.md) and integrating once gives [constant-stress Reynolds-averaged wall flow](../../../../../../constant-stress-reynolds-averaged-wall-flow.md):

$$
\boxed{\tau_d=\mu U_z-\rho\overline{u'w'},\qquad\frac{d\tau_d}{dz}=0.}
$$

Here $\tau_d$ is physical [shear stress](../../../../../../shear-stress.md). Positive mean shear commonly has $\overline{u'w'}<0$, representing downward transport of positive horizontal momentum. The Reynolds term then contributes positively to the total stress.

The printed target formula has an extra vertical derivative in the Reynolds contribution. That term has dimensions of stress per length, while $\mu U_z$ has dimensions of stress, so the formula as printed is inconsistent. The derivative belongs in the stress-divergence equation above; the boxed integrated stress is the corrected result. Part b also uses a kinematic rather than physical stress, so the [density](../../../../../../density.md) factor must be tracked explicitly.

Define the [friction velocity](../../../../../../shear-velocity.md) $u_*=\sqrt{\tau_d/\rho}$ for positive wall shear. In the near-wall region [turbulence](../../../../../../turbulence-split.md) is suppressed and molecular viscosity carries the stress. With no slip, $U\simeq u_*^2z/\nu$. The viscous wall coordinate $z^+=zu_*/\nu$ becomes order one at the characteristic [viscous sublayer](../../../../../../viscous-sublayer.md) length

$$
\boxed{\delta\sim\frac{\nu}{u_*}.}
$$

The numerical extent of viscosity dominance depends on the crossover convention and wall condition; the scaling is the required viscous length.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
