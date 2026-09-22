<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The leading disturbance in [sphere](../../../../../sphere.md) [Stokes flow](../../../../../stokes-flow-split.md) has size $u\sim Ua/r$. Consequently viscous [diffusion](../../../../../diffusion.md) has size $\nu u/r^2$, background [advection](../../../../../advection.md) has size $Uu/r$, and their ratio is $Ur/\nu$. Even if the [sphere](../../../../../sphere.md) [Reynolds number](../../../../../reynolds-number.md) $Ua/\nu$ is small, this ratio becomes order one at $r\sim\nu/U$. Thus **the Stokes approximation is nonuniform at distances of order $\nu/U$**. At that outer distance the disturbance itself is small relative to $U$, so self-convection is smaller than background [advection](../../../../../advection.md) and the [Oseen approximation](../../../../../oseen-approximation.md) is appropriate:

$$
\boxed{\rho\mathbf U\cdot\nabla\mathbf u=-\nabla p+\mu\nabla^2\mathbf u,\qquad\nabla\cdot\mathbf u=0.}
$$

Write $\mathbf u=\nabla\phi+\nu\nabla\chi-\mathbf U\chi$. It is sufficient outside the origin to impose $\Delta\phi=0$ and $(\nu\Delta-\mathbf U\cdot\nabla)\chi=0$: these give zero [divergence](../../../../../divergence.md), and substitution into [momentum](../../../../../momentum.md) gives $p=-\rho\mathbf U\cdot\nabla\phi$. With $\chi=h e^{\mathbf U\cdot\mathbf x/(2\nu)}$, differentiation yields

$$
(\nu\Delta-\mathbf U\cdot\nabla)\chi=\nu e^{\mathbf U\cdot\mathbf x/(2\nu)}\left(\Delta h-\frac{U^2}{4\nu^2}h\right),\qquad U=|\mathbf U|.
$$

A decaying radial choice is $h=C e^{-Ur/(2\nu)}/r$. Therefore

$$
\chi=\frac C r\exp\left(\frac{\mathbf U\cdot\mathbf x-Ur}{2\nu}\right).
$$

The exponent is nonpositive, so this scalar decays at infinity, including as $1/r$ directly downstream. In the overlap $a\ll r\ll\nu/U$,

$$
\chi=\frac C r+\frac C{2\nu}\frac{\mathbf U\cdot\mathbf x}{r}-\frac{CU}{2\nu}+\cdots.
$$

Choosing $\phi=-\nu C/r$ cancels the first term's [gradient](../../../../../gradient.md) in $\nabla\phi+\nu\nabla\chi$. The remaining leading [velocity](../../../../../velocity.md) is

$$
\mathbf u\sim\frac C2\nabla\left(\frac{\mathbf U\cdot\mathbf x}{r}\right)-\frac C r\mathbf U=-\frac C{2r}\left[\mathbf U+\mathbf n(\mathbf U\cdot\mathbf n)\right].
$$

Matching fixes $C=3a/2$. Thus the [potential-source and wake decomposition of sphere Oseen flow](../../../../../potential-source-and-wake-decomposition-of-sphere-oseen-flow.md) is

$$
\boxed{\phi=-\frac{3a\nu}{2r},\qquad\chi=\frac{3a}{2r}e^{(\mathbf U\cdot\mathbf x-Ur)/(2\nu)},\qquad\mathbf u=\nabla\phi+\nu\nabla\chi-\mathbf U\chi.}
$$

Its [pressure](../../../../../pressure.md) is $p=-3\mu a(\mathbf U\cdot\mathbf x)/(2r^3)$, the sign appropriate to a fixed [sphere](../../../../../sphere.md) in an incident flow. The [velocity](../../../../../velocity.md) decays in every direction and matches the requested leading inner disturbance; the [sphere](../../../../../sphere.md)'s potential-dipole term enters a higher matching order.

The scalar potential is a [point source](../../../../../point-source.md): $\nabla\phi=(3a\nu/2)\mathbf x/r^3$, so [integration](../../../../../integral.md) over a centred [sphere](../../../../../sphere.md) gives

$$
\boxed{Q_{\rm source}=\int\nabla\phi\cdot\mathbf n\,dS=6\pi\nu a,\qquad\dot M_{\rm source}=\rho Q_{\rm source}=6\pi\mu a.}
$$

To see the [fluid wake](../../../../../wake-physics.md), take $z$ downstream along $\mathbf U$ and transverse radius $R_\perp$. For $z\gg\nu/U$, $r-z\simeq R_\perp^2/(2z)$, giving

$$
\chi\simeq\frac{3a}{2z}\exp\left(-\frac{UR_\perp^2}{4\nu z}\right),\qquad u_z\simeq-U\chi.
$$

The [fluid wake](../../../../../wake-physics.md) is concentrated within $R_\perp=O(\sqrt{\nu z/U})$. Its integrated mass deficit is $\rho U\int\chi\,dA\simeq6\pi\mu a$, balancing the outward potential-source [mass flux](../../../../../mass-flux.md). The corresponding [momentum](../../../../../momentum.md) deficit is

$$
\boxed{\rho U^2\int\chi\,dA\simeq6\pi\mu aU,}
$$

which equals the leading [sphere](../../../../../sphere.md) drag. The [Gaussian integral](../../../../../gaussian-integral.md) used here is $\int_0^\infty e^{-UR_\perp^2/(4\nu z)}2\pi R_\perp dR_\perp=4\pi\nu z/U$.

The PDF labels $6\pi\mu aU$ as the mass-source strength, but this has dimensions of [force](../../../../../force.md). **The actual mass-source strength is $6\pi\mu a$; $6\pi\mu aU$ is the [momentum](../../../../../momentum.md) deficit or drag.** The decomposition above supplies both quantities and identifies the printed normalization error.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
