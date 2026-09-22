<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $\beta=p_{\rm rad}/p_{\rm gas}$ is the [radiation-to-gas pressure ratio](../../../../../../radiation-to-gas-pressure-ratio.md), not [plasma beta](../../../../../../plasma-beta.md). Write the [opacity](../../../../../../opacity.md) as $\kappa_{\rm op}$ to distinguish it from the [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md). The [radiation pressure](../../../../../../radiation-pressure.md) is $p_{\rm rad}=4\sigma T^4/(3c)$, so [radiative diffusion](../../../../../../radiative-diffusion.md) can be written as

$$
F_z=-\frac{c}{\kappa_{\rm op}\rho}\frac{dp_{\rm rad}}{dz}.
$$

Since $\beta$ is independent of height, $p_{\rm rad}=\beta p/(1+\beta)$. Substitution of [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md), $p'=-\rho\Omega^2z$, gives

$$
F_z=\frac\beta{1+\beta}\frac{c\Omega^2}{\kappa_{\rm op}}z.
$$

Differentiating and using the viscous heating equation, together with $r\Omega'=-q\Omega$, yields

$$
\rho\nu q^2\Omega^2=\frac\beta{1+\beta}\frac{c\Omega^2}{\kappa_{\rm op}},\qquad
\boxed{\rho\nu=\frac\beta{1+\beta}\frac{c}{q^2\kappa_{\rm op}}}.
$$

Thus the effective [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\rho\nu$ is independent of height. If the surfaces are at $z=\pm H$, the vertically integrated [kinematic viscosity](../../../../../../kinematic-viscosity.md) satisfies

$$
\bar\nu\Sigma=\int_{-H}^H\rho\nu\,dz
=2H\frac\beta{1+\beta}\frac{c}{q^2\kappa_{\rm op}}.
$$

Use the previous result and the specified [Eddington accretion rate](../../../../../../eddington-accretion-rate.md) convention,

$$
\dot M_E=\frac{L_E}{\eta c^2}
=\frac{4\pi GM}{\eta\kappa_{\rm op}c},\qquad \eta=\frac1{16},
$$

to obtain the full thickness

$$
\boxed{2H=\frac{64}{3}\frac{1+\beta}{\beta}\,q^2f\,
\frac{\dot M}{\dot M_E}\frac{GM}{c^2}}.
$$

The [constant-pressure-ratio vertical disk model](../../../../../../constant-pressure-ratio-vertical-disk-model.md) therefore has thickness proportional to the inward [accretion rate](../../../../../../accretion-rate.md). This is a full surface-to-surface thickness, rather than a density [disk scale height](../../../../../../disk-scale-height.md). Its use as a [thin disk](../../../../../../thin-disk.md) requires $2H\ll r$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
