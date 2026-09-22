# Frequency and wavelength spectral radiance conversion

↑ **Parent:** [Spectral radiance](spectral-radiance.md)

In [vacuum](vacuum.md), $\nu=c/\lambda$, where $c$ is the [speed of light](speed-of-light.md). Increasing [wavelength](wavelength.md) decreases [frequency](frequency.md), so the ordinary signed [differentials](differential-of-a-smooth-map.md) satisfy $d\nu=-c\lambda^{-2}d\lambda$. A spectral slice's positive contribution to [radiance](radiance.md) must be unchanged. The [change of variables formula](change-of-variables-formula.md) therefore gives the absolute [Jacobian determinant](jacobian-determinant.md)

$$
L_\nu(\nu)=L_\lambda(c/\nu)\left|\frac{d\lambda}{d\nu}\right|
=L_\lambda(c/\nu)\frac{c}{\nu^2},
\qquad
L_\lambda(\lambda)=L_\nu(c/\lambda)\frac{c}{\lambda^2}.
$$

These formulas use $L_\lambda$ per metre and $L_\nu$ per hertz. The factor $c/\nu^2$ has units $\mathrm{m\,s}=\mathrm{m\,Hz^{-1}}$, which converts the former density into the latter. If $\ell_{\rm nm}$ denotes the numerical density per nanometre in $\mathrm{W\,m^{-2}\,sr^{-1}\,nm^{-1}}$, its per-metre value is $10^9\ell_{\rm nm}$. Conversely, the per-nanometre value is $10^{-9}$ times the per-metre value. Likewise, a density per terahertz is $10^{12}$ times its per-hertz value because $1\,\mathrm{THz}=10^{12}\,\mathrm{Hz}$.

For a concrete stipulated spectrum, let $L_\lambda=C=10^9\,\mathrm{W\,m^{-2}\,sr^{-1}\,m^{-1}}$ between $\lambda_1=500\,\mathrm{nm}$ and $\lambda_2=600\,\mathrm{nm}$, and zero outside. This is exactly $1\,\mathrm{W\,m^{-2}\,sr^{-1}\,nm^{-1}}$ throughout the band. Using the exact [International System of Units](international-system-of-units.md) value $c=299792458\,\mathrm{m\,s^{-1}}$, the corresponding [frequency](frequency.md) bounds are

$$
\nu_1=\frac{c}{\lambda_2}=499.654096666\ldots\,\mathrm{THz},
\qquad
\nu_2=\frac{c}{\lambda_1}=599.584916\,\mathrm{THz}.
$$

The transformed [spectral radiance](spectral-radiance.md) is $L_\nu=Cc/\nu^2$ on this interval. At $\nu_1$ it is approximately $1.200830743\times10^{-12}\,\mathrm{W\,m^{-2}\,sr^{-1}\,Hz^{-1}}$, and at $\nu_2$ it is $8.339102380\times10^{-13}$ in the same units. These are respectively $1.200830743$ and $0.833910238$ per terahertz. Thus a flat [wavelength](wavelength.md) density becomes a decreasing [frequency](frequency.md) density; relabelling the horizontal axis alone would miss both the shape and the units. [NIST, Meet the Constants: exact speed of light](https://www.nist.gov/si-redefinition/meet-constants).

The equality of band [radiances](radiance.md) has a short exact proof:

$$
\int_{\lambda_1}^{\lambda_2}C\,d\lambda
=C(\lambda_2-\lambda_1)
=100\,\mathrm{W\,m^{-2}\,sr^{-1}},
$$



$$
\int_{\nu_1}^{\nu_2}\frac{Cc}{\nu^2}\,d\nu
=Cc\left(\frac1{\nu_1}-\frac1{\nu_2}\right)
=C(\lambda_2-\lambda_1).
$$

The reversed bounds and the [Jacobian determinant](jacobian-determinant.md) preserve the same spectral measure. Each half-band, $500$–$550\,\mathrm{nm}$ and $550$–$600\,\mathrm{nm}$, carries $50\,\mathrm{W\,m^{-2}\,sr^{-1}}$, although the corresponding [frequency](frequency.md) widths are about $54.508$ and $45.423\,\mathrm{THz}$.

<a id="image-a-flat-wavelength-spectrum-becomes-curved-in-frequency-with-equal-band-radiances"></a>
![](spectral-radiance-variable-change.png)

**[Figure 4](#image-a-flat-wavelength-spectrum-becomes-curved-in-frequency-with-equal-band-radiances). A flat wavelength spectrum becomes curved in frequency, with equal band radiances**. Matching colours identify the same two spectral half-bands. The shaded areas are $50\,\mathrm{W\,m^{-2}\,sr^{-1}}$ each in either coordinate. The right-hand density is plotted per terahertz; the longer-wavelength half-band occupies the lower-frequency, narrower interval. Both total shaded areas are exactly $100\,\mathrm{W\,m^{-2}\,sr^{-1}}$.

A spectrum's peak is consequently a statement about a particular density and coordinate. The [frequency and wavelength peaks of Planck's law](frequency-and-wavelength-peaks-of-planck-s-law.md) differ for precisely this reason. Integrated [radiance](radiance.md) over a specified physical band supplies a comparison that survives the [change of variables](change-of-variables-formula.md).

## ↑ Ancestors (7)

1. [Spectral radiance](spectral-radiance.md)
2. [Radiance](radiance.md)
3. [Radiometry](radiometry-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Spectral radiant flux](spectral-radiant-flux.md)
- [Wien's displacement law](wien-s-displacement-law.md)
