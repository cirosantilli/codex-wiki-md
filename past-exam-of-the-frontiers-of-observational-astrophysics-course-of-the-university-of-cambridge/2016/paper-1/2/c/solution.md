<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [electron](../../../../../electron.md) accelerated in an [ion](../../../../../ion.md)'s Coulomb field emits [bremsstrahlung](../../../../../bremsstrahlung.md). Both [electron](../../../../../electron.md) states are unbound, giving free-free radiation rather than a discrete bound-state line. Averaging over a Maxwellian [electron](../../../../../electron.md) distribution gives an optically thin spectral emissivity with dependence

$$
j_\nu=C_{\rm ff}Z^2n_en_iT^{-1/2}e^{-h\nu/(k_BT)}\bar g_{\rm ff}(\nu,T).
$$

Here $C_{\rm ff}$ depends on the emissivity convention, and the [Gaunt factor](../../../../../gaunt-factor.md) supplies the quantum correction. No numerical emissivity normalization is needed for these diagnostics. For a mixture, sum $Z_i^2n_i$ over [ion](../../../../../ion.md) species. The bolometric emissivity is proportional to $n_e\sum Z_i^2n_i\,T^{1/2}$ with a frequency-averaged [Gaunt factor](../../../../../gaunt-factor.md). Thermal [electron](../../../../../electron.md) speeds control the spectrum while the encounter rate supplies its density-squared dependence.

[temperature](../../../../../temperature-split.md) can be measured from the high-energy exponential cutoff at [photon](../../../../../photon.md) energy of order $k_BT$, provided the spectrum spans that turnover and foreground absorption and nonthermal contamination are modelled. At radio [frequencies](../../../../../frequency.md) $h\nu\ll k_BT$, the exponential is nearly one, so the optically thin continuum is a poor thermometer by slope alone. Kirchhoff's law, $\alpha_\nu=j_\nu/B_\nu$, and the [Rayleigh-Jeans law](../../../../../rayleigh-jeans-law.md) give $\alpha_\nu\propto n_en_iT^{-3/2}\nu^{-2}\bar g_{\rm ff}$ for an isothermal thermal [plasma](../../../../../plasma-physics.md). The transfer solution is

$$
I_\nu=B_\nu(T)(1-e^{-\tau_\nu}),\qquad T_b\simeq T(1-e^{-\tau_\nu})
$$

in the radio limit. A resolved optically thick region therefore measures its [electron](../../../../../electron.md) [temperature](../../../../../temperature-split.md) through [brightness temperature](../../../../../brightness-temperature.md), if it fills the beam. The turnover between thick and thin emission constrains the line-of-sight [emission measure](../../../../../emission-measure.md) $\mathrm{EM}=\int n_e^2dl$ for a hydrogen-dominated fully ionized [plasma](../../../../../plasma-physics.md). In the thin regime $T_b\simeq T\tau_\nu$, rather than $T_b=T$. The slowly varying [Gaunt factor](../../../../../gaunt-factor.md) gives a nearly flat optically thin radio flux-density spectrum, in contrast to the $\nu^2$ thick limit at fixed projected area.[chapter 4, §4.3, especially equations (4.57)–(4.58): emission measure, absorption and optically thick/thin diagnostics](../../../../../essential-radio-astronomy-by-james-j-condon-and-scott-m-ransom.md)

To obtain [density](../../../../../density.md), one also needs geometry. An angular extent and independent distance give a transverse size; an assumed shape provides a depth or volume. For approximately uniform emitting gas with [astrophysical volume filling factor](../../../../../astrophysical-volume-filling-factor.md) $f_V$, $L_{\rm ff}\propto n_e^2 f_VVT^{1/2}$, so $n_e\propto[L_{\rm ff}/(f_VVT^{1/2})]^{1/2}$. Alternatively a measured column [emission measure](../../../../../emission-measure.md) and assumed path length give an rms [density](../../../../../density.md). Clumping raises the mean squared [density](../../../../../density.md) relative to the square of the mean: the inferred value is not automatically the mean gas [density](../../../../../density.md). **Free-free brightness alone does not uniquely determine [temperature](../../../../../temperature-split.md), [density](../../../../../density.md) and physical size.** Resolved imaging, a distance, optical-depth information or an independent column-density diagnostic is needed to remove those degeneracies. Cluster SZ data are complementary because their leading signal depends on $\int n_eT_e\,dl$, whereas free-free emission depends on [density](../../../../../density.md) squared. Metal lines, unresolved [temperature](../../../../../temperature-split.md) structure, foreground absorption, synchrotron emission and [background subtraction](../../../../../background-subtraction.md) must be controlled before attributing the continuum to a single thermal component.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../../../split.md)
6. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../../../../frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
