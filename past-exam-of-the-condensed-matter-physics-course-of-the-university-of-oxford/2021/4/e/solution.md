<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the stipulated noninteracting [impurity band](../../../../impurity-band.md) approximation, with one donated [electron](../../../../electron.md) per donor and two available [spin](../../../../spin.md) states per donor orbital. The [energy band](../../../../energy-band.md) is half filled. Approximating its spin-summed [density of states](../../../../density-of-states.md) per volume near the [Fermi energy](../../../../fermi-energy.md) by $D_v(E_F)\simeq2n/W$ gives the zero-[temperature](../../../../temperature-split.md) [Pauli paramagnetism](../../../../pauli-paramagnetism.md)

$$
\chi_{\rm imp}=\mu_0\left(\frac{|g|\mu_B}{2}\right)^2D_v(E_F)
\simeq\frac{\mu_0g^2\mu_B^2n}{2W}.
$$

With $\alpha=1$,

$$
\boxed{\chi_{\rm imp}(n)\sim\frac{\mu_0g^2\mu_B^2}{2E_b}\,n\exp\left(\frac1{a_bn^{1/3}}\right)>0.}
$$

A factor of order one depends on the [density of states](../../../../density-of-states.md) shape; using the [conduction band](../../../../conduction-band.md) $g$-factor rather than silently setting $g=2$ matters here.

To locate the comparison with the magnitude of the undoped [Larmor-Langevin susceptibility](../../../../larmor-langevin-susceptibility.md), put $x=n^{-1/3}/a_b>1$. Numerically,

$$
\chi_{\rm imp}\simeq P\frac{e^x}{x^3},\qquad
P=\frac{\mu_0g^2\mu_B^2}{2E_ba_b^3}=1.179\times10^{-8}.
$$

For the stated atomic-scale estimate $R=a_0$ in part (b), equality with $|\chi_0|=2.599\times10^{-5}$ requires

$$
x-3\ln x=\ln\frac{|\chi_0|}{P},\qquad x\simeq16.02.
$$

Thus the dilute-branch crossover is

$$
\boxed{n_*\simeq2.3\times10^{20}\,\mathrm{m^{-3}}
=2.3\times10^{14}\,\mathrm{cm^{-3}},}
$$

well below $a_b^{-3}=9.45\times10^{23}\,\mathrm{m^{-3}}$. Within this model the positive [spin](../../../../spin.md) response exceeds the negative background magnitude for **lower** [dopant densities](../../../../dopant-density.md) on this dilute branch: the exponential narrowing of $W$ wins over the loss of donors. Indeed $d\ln(e^x/x^3)/dx=1-3/x>0$ for $x>3$. This is not a claim of [ferromagnetism](../../../../ferromagnetism.md).

The degenerate [Pauli paramagnetism](../../../../pauli-paramagnetism.md) calculation requires $k_BT\ll W$, with an unimportant order-one filling factor. At the estimated crossing,

$$
W=E_be^{-16.02}\simeq6.04\times10^{-10}\,\mathrm{eV},\qquad
\boxed{T\ll W/k_B\simeq7.0\times10^{-6}\,\mathrm K.}
$$

The weak-field condition also requires $|g|\mu_BB\ll W$. For a different assumed atomic $R$, use $|\chi_0|=2.599\times10^{-5}(R/a_0)^2$ in the displayed equation for $x$. An order-of-magnitude background $|\chi_0|\sim10^{-5}$ gives the same density order and a crossover scale of order $10^{-5}\,\mathrm K$. At higher [temperature](../../../../temperature-split.md) than this extremely narrow [bandwidth](../../../../bandwidth-signal-processing.md) permits, the $n/W$ enhancement cannot be used; the independent-donor [Curie law](../../../../curie-s-law.md) is the appropriate thermal scale if interactions remain negligible. At very small [dopant density](../../../../dopant-density.md), disorder, localization and [Coulomb interactions](../../../../coulomb-interaction.md) can also invalidate the assumed noninteracting [impurity band](../../../../impurity-band.md). The formal divergence as $n\to0$ is therefore a limit of the stated zero-[temperature](../../../../temperature-split.md) band model, not a prediction for isolated donors at a fixed nonzero [temperature](../../../../temperature-split.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
