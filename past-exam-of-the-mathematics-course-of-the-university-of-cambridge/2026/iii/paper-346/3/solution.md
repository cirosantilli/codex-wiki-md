<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $x=r/r_s$. The enclosed mass of the [Navarro--Frenk--White profile](../../../../../navarro-frenk-white-profile.md) is

$$
M(r)=4\pi\int_0^r\rho(r')r'^2\,dr'
=4\pi\rho_sr_s^3\int_0^x\frac{y}{(1+y)^2}\,dy.
$$

Since $y/(1+y)^2=(1+y)^{-1}-(1+y)^{-2}$,

$$
\boxed{M(r)=4\pi\rho_sr_s^3
\left[\log(1+x)-\frac{x}{1+x}\right]}.
$$

The circular-orbit condition $v_c^2/r=GM(r)/r^2$ then gives the [galaxy rotation curve](../../../../../galaxy-rotation-curve.md)

$$
\boxed{v_c^2(r)=4\pi G\rho_sr_s^2
\frac{\log(1+x)-x/(1+x)}{x}}.
$$

For $x\ll1$,

$$
\log(1+x)-\frac{x}{1+x}=\frac{x^2}{2}+O(x^3),
$$

and therefore

$$
v_c^2\sim2\pi G\rho_sr_sr,
\qquad
\boxed{v_c\propto r^{1/2}}.
$$

For $x\gg1$,

$$
\log(1+x)-\frac{x}{1+x}=\log x-1+O(x^{-1}),
$$

so

$$
\boxed{v_c^2\sim4\pi G\rho_sr_s^2\frac{\log x-1}{x}},
\qquad
v_c\sim\left(\frac{\log r}{r}\right)^{1/2}.
$$

The NFW curve thus rises from the center, peaks, and eventually declines slowly. Typical spiral-galaxy rotation curves remain approximately flat over the observed outer disk, although an NFW halo combined with baryons can approximate such a plateau over a finite interval.

At the maximum, $x_m=2.16$, so the [scale radius of a Navarro--Frenk--White profile](../../../../../scale-radius-of-a-navarro-frenk-white-profile.md) is

$$
\boxed{r_s=\frac{20}{2.16}\,\mathrm{kpc}=9.26\,\mathrm{kpc}}.
$$

Writing $f(x)=\log(1+x)-x/(1+x)$, the [characteristic density of a Navarro--Frenk--White profile](../../../../../characteristic-density-of-a-navarro-frenk-white-profile.md) is

$$
\boxed{\rho_s=
\frac{v_{\max}^2x_m}{4\pi Gr_s^2f(x_m)}}.
$$

With $G=4.3009\times10^{-6}\,\mathrm{kpc}(\mathrm{km\,s^{-1}})^2M_\odot^{-1}$ and $f(2.16)=0.4670$, this is

$$
\boxed{\rho_s\simeq4.83\times10^7M_\odot\,\mathrm{kpc}^{-3}
=0.0483M_\odot\,\mathrm{pc}^{-3}}.
$$

An NFW cusp has $\rho\propto r^{-1}$ and hence $v_c\propto r^{1/2}$. Many dwarf and low-surface-brightness galaxies instead favor a nearly constant-density core, for which $M(r)\propto r^3$ and $v_c\propto r$; after matching the outer speed, this gives the more slowly rising observed inner curve. This is the [cusp--core problem](../../../../../cusp-core-problem.md). Repeated burst-driven gas outflows can fluctuate the central potential and transfer orbital energy to dark matter, while self-interacting dark matter provides another possible core-forming mechanism. Beam smearing and noncircular motions are observational systematics but do not explain every case.

For an [exponential galactic disk](../../../../../exponential-galactic-disk.md),

$$
M_{\rm disk}=2\pi\int_0^\infty \Sigma_0e^{-R/R_d}R\,dR
=2\pi\Sigma_0R_d^2\int_0^\infty ue^{-u}\,du,
$$

so

$$
\boxed{M_{\rm disk}=2\pi\Sigma_0R_d^2}.
$$

Since $7\,\mathrm{kpc}\simeq2.3R_d$ is near the disk maximum, assigning the full $220\,\mathrm{km\,s^{-1}}$ there gives

$$
M_{\rm disk}\simeq\frac{R_d}{G}
\left(\frac{220\,\mathrm{km\,s^{-1}}}{0.88}\right)^2
\simeq\boxed{4.36\times10^{10}M_\odot}.
$$

If the disk mass is increased while the observed total curve is fixed, the halo contribution must decrease in the inner galaxy. An NFW fit therefore needs a lower characteristic density, a larger scale radius and lower concentration, or a correlated combination of these changes.

A [maximum disk](../../../../../maximum-disk.md) model raises the stellar mass-to-light ratio as far as the rotation curve permits, conventionally making the disk contribute about $85\%$ of the speed near $2.2R_d$. High stellar surface densities, population-synthesis mass-to-light ratios, microlensing optical depths, and fast bars that have suffered little dynamical-friction braking can support a large disk contribution. Directly measured vertical stellar dispersions often favor submaximal disks, especially in low-surface-brightness galaxies, while stability and cosmological halo constraints may also disfavor an excessively massive disk.

The [disk--halo degeneracy](../../../../../disk-halo-degeneracy.md) follows from

$$
v_{\rm obs}^2=v_{\rm gas}^2+v_{\rm disk}^2+v_{\rm bulge}^2+v_{\rm halo}^2.
$$

Over a finite radial range, raising the stellar mass-to-light ratio and lowering or broadening the halo can leave the same sum. The degeneracy can be reduced by measuring the disk surface density dynamically from vertical velocity dispersion and scale height, or by constraining the stellar mass-to-light ratio with resolved populations, colors, and a specified initial mass function. Strong or weak gravitational lensing, gas-layer flaring, stellar streams, and rotation data far beyond the optical disk provide further independent halo constraints.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
