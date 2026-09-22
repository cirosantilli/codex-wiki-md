<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Interpret the requested abundance as [comoving number density](../../../../../../comoving-number-density.md) and use this question's mean density, rather than importing the different cosmology of Question 2. The mass-to-radius relation for a [spherical top-hat window function](../../../../../../spherical-top-hat-window-function.md) gives

$$
R=\left(\frac{3M}{4\pi\bar\rho_0}\right)^{1/3}=0.2568\,\mathrm{Mpc}\qquad (M=10^{10}M_\odot).
$$

The normalization radius $7h^{-1}\,\mathrm{Mpc}$ is $10\,\mathrm{Mpc}$, not $4.9\,\mathrm{Mpc}$. Using $m=-3/4$,

$$
\sigma(M,3)=0.25\left(\frac{0.2568}{10}\right)^{-3/4}\simeq3.897,\qquad \sigma(M,z)\simeq\frac{4(3.897)}{1+z}.
$$

These are linearly extrapolated rms amplitudes, even when the numerical value at late times exceeds one. The high-redshift matter-dominated approximation is appropriate to the crossing sought below.

For $s=1/4$, the [Press-Schechter halo mass function](../../../../../../press-schechter-halo-mass-function.md) yields

$$
M\frac{dN}{dM}=\sqrt{\frac2\pi}\frac{\bar\rho_0}{4M}\nu e^{-\nu^2/2}=2.8125\,\nu e^{-\nu^2/2}\,\mathrm{Mpc^{-3}},\qquad \nu=\frac{1.68647(1+z)}{15.5893}.
$$

Equating this to $10^{-4}\,\mathrm{Mpc^{-3}}$ gives $\nu e^{-\nu^2/2}=3.5555\times10^{-5}$. On the rare-object branch, solving $\nu^2/2-\ln\nu=\ln(2.8125\times10^4)$ gives $\nu\simeq4.8634$. Hence

$$
\boxed{1+z\simeq44.96,\qquad z\simeq44.}
$$

This is the first crossing as the Universe evolves from very early times. It retains the supplied scale-free extrapolation across a substantial range of scales; it is not a precision prediction using a full matter spectrum.

The abundance factor $\nu e^{-\nu^2/2}$ peaks at $\nu=1$. Therefore the same target has a second mathematical root, $\nu\simeq3.56\times10^{-5}$, corresponding to $z\simeq-0.99967$ if matter-dominated growth is extrapolated indefinitely. This extremely remote future branch is not the formation epoch and would not be physically justified by that growth approximation in a universe with late vacuum domination. This illustrates the [two abundance crossings of the Press-Schechter mass function](../../../../../../two-abundance-crossings-of-the-press-schechter-mass-function.md).

There is also an input-normalization qualification. If the characteristic cutoff is defined exactly by $\nu^2/2=(M/M_*)^{1/2}$, the variance normalization here gives $M_*(3)=10^{10}[\sqrt2(3.897)/1.68647]^4\simeq1.14\times10^{12}M_\odot$, rather than the earlier approximate quoted cutoff. **The numerical estimate uses the explicit rms normalization in this part and the mass-scaling exponent from the preceding part; both cutoff normalizations cannot be imposed as exact simultaneously.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
