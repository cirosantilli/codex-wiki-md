# Finite-end correction for periodic rod heating

↑ **Parent:** [Ångström periodic heating method](angstrom-periodic-heating-method.md)

A finite rod generally contains both exponential branches. With prescribed oscillating [temperature](temperature-split.md) at $x=0$ and an insulated far end, $\widehat\theta'(L)=0$, the exact solution is

$$
\widehat\theta(x)=\Theta_0\frac{\cosh[\gamma(L-x)]}{\cosh(\gamma L)}
=\Theta_0e^{-\gamma x}\frac{1+e^{-2\gamma(L-x)}}{1+e^{-2\gamma L}}.
$$

The correction near a sensor is controlled by $e^{-2a(L-x)}$. The important separation is between the farther sensor and the end, not merely between the heater and the end. For a far end clamped at the mean [temperature](temperature-split.md), $\widehat\theta(L)=0$, replace both [hyperbolic cosines](hyperbolic-cosine.md) by [hyperbolic sines](hyperbolic-sine.md); other end [boundary conditions](boundary-condition.md) require their corresponding solution.

In the lossy [Ångström method worked example](angstrom-method-worked-example.md), an insulated rod of [length](length.md) $L=0.080\,\mathrm m$ gives $D=0.354866$ and $\Delta\phi=0.615651\,\mathrm{rad}$. Incorrectly applying the semi-infinite formula returns $1.29418\times10^{-4}\,\mathrm{m^2\,s^{-1}}$, about $29.4\%$ high. At $L=0.300\,\mathrm m$, it returns $9.99877\times10^{-5}\,\mathrm{m^2\,s^{-1}}$, about $0.0123\%$ low. Side loss remains real in both cases; the error arises because the measured spatial response no longer has one exponential [complex wavenumber](complex-wavenumber.md).

Choose the period and sensor spacing so that the lag and attenuation are resolvable while the downstream signal remains larger than sensor noise. Keep transverse equilibration fast compared with the period; compare the transverse [thermal diffusion time](thermal-diffusion-time.md) with $P$ and check that surface exchange does not create large transverse [temperature gradients](temperature-gradient.md). A short period reduces far-end influence but can expose sensor response times; a long period increases penetration and finite-end bias. Calibrate both sensors together, exchange their positions to check channel bias, compare successive cycles, and repeat at several spacings and periods. In a valid single-exponential region, [linear regression](linear-regression-split.md) of $\log A$ against $x$ and unwrapped lag against $x$ should give consistent slopes. These are proposed diagnostic controls. If they fail, fit the finite-rod or coupled-sensor model rather than interpreting every delay as intrinsic [thermal diffusivity](thermal-diffusivity.md).

## ↑ Ancestors (9)

1. [Ångström periodic heating method](angstrom-periodic-heating-method.md)
2. [Thermal diffusivity](thermal-diffusivity.md)
3. [Thermal conduction](thermal-conduction.md)
4. [Heat](heat-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
