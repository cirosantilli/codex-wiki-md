<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The prescribed photon budget requires a collapsed mass fraction $f_{\rm coll}=3/3000=10^{-3}$, assuming baryons trace the collapsed mass fraction and using the supplied effective photon yield. No extra photon-escape or recombination correction should be counted on top of this stipulated budget.

For spectral slope $n=-2$, $q=1/6$. The mass-scale measurement gives

$$
\sigma(M_{\min},3)=0.5\left(\frac{64M_{\min}}{M_{\min}}\right)^{1/6}=1.
$$

Both relevant epochs are matter-dominated, so the [linear growth factor](../../../../../../linear-growth-factor.md) ratio is $D(z)/D(3)=4/(1+z)$, independent of any present-day normalization convention. Thus $\sigma(M_{\min},z)=4/(1+z)$. The [Press-Schechter formalism](../../../../../../press-schechter-formalism.md) gives

$$
\operatorname{erfc}\left[\frac{\delta_{\rm sc}(1+z)}{4\sqrt2}\right]=10^{-3}.
$$

Using the supplied inverse value,

$$
\boxed{1+z_{\rm reion}=\frac{4\sqrt2\,(2.33)}{1.686}\simeq7.82,\qquad z_{\rm reion}\simeq6.8.}
$$

This is the [photon-budget reionization threshold](../../../../../../photon-budget-reionization-threshold.md) in the specified toy model, not a measurement of the full astrophysical reionization history.

To estimate the characteristic mass, use the non-dissipative [spherical-collapse model](../../../../../../spherical-collapse-model.md) result $\Delta_{\rm vir}=18\pi^2$. At this high redshift the background matter density is practically the [critical density](../../../../../../critical-density.md). Circular [virial velocity](../../../../../../virial-velocity-of-a-spherical-overdensity-halo.md) then obeys

$$
v_{\rm vir}^2=\frac{GM}{r_{\rm vir}},\qquad
M=\frac{4\pi}{3}r_{\rm vir}^3\Delta_{\rm vir}\frac{3H^2}{8\pi G},
\qquad v_{\rm vir}=3\pi H r_{\rm vir}.
$$

Consequently

$$
M_{\min}=\frac{v_{\rm vir}^3}{3\pi GH(z)},\qquad
H(z)\simeq72\sqrt{0.25}(1+z)^{3/2}\,\mathrm{km\,s^{-1}\,Mpc^{-1}}.
$$

For $v_{\rm vir}=9\,\mathrm{km\,s^{-1}}$, this gives $H\simeq7.87\times10^2\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$ and **$M_{\min}\simeq2.3\times10^7M_\odot$**, with physical virial radius about $1.21\,\mathrm{kpc}$.

At the threshold mass the [halo peak height](../../../../../../halo-peak-height.md) is $\nu=\sqrt2(2.33)\simeq3.30$, so

$$
n(M_{\min},z)M_{\min}=\frac{\bar\rho_{m,0}}{M_{\min}}F,\qquad
F=\sqrt{\frac2\pi}\frac16\nu e^{-\nu^2/2}\simeq1.92\times10^{-3}.
$$

The present mean matter density is $\bar\rho_{m,0}=2.775\times10^{11}\Omega_{\rm mat}h^2M_\odot\,\mathrm{Mpc}^{-3}\simeq3.60\times10^{10}M_\odot\,\mathrm{Mpc}^{-3}$. Hence the differential abundance per logarithmic mass interval is about $3.0\,\mathrm{Mpc}^{-3}$ and

$$
\boxed{\bar l=\bigl[n(M_{\min},z)M_{\min}\bigr]^{-1/3}
=\left(\frac{M_{\min}}{\bar\rho_{m,0}F}\right)^{1/3}\simeq0.69\,\mathrm{Mpc}\ \text{comoving}.}
$$

Rounded inputs and the supplied approximate factor justify quoting about $0.7\,\mathrm{Mpc}$. The corresponding physical separation is about $0.088\,\mathrm{Mpc}$ at this epoch. The requested [halo spacing from a differential mass function](../../../../../../halo-spacing-from-a-differential-mass-function.md) uses a logarithmic mass bin of order unity; it is not obtained by identifying $f_{\rm coll}\bar\rho/M$ with that differential abundance. A cumulative number density above the threshold requires a separate mass integral.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
