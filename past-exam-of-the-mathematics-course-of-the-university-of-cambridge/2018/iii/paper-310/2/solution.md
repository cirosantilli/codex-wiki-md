<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Interpret $P(k)$ in the variance integral as the unsmoothed [cosmological density power spectrum](../../../../../matter-power-spectrum.md) of $\delta$. A linear smoothing window gives $P_R(k)=P(k)|\widetilde W(kR)|^2$ for the smoothed field; the PDF's description of $P(k)$ as already belonging to $\delta_R$ would otherwise count the window twice.

For a [scale-free matter power spectrum](../../../../../scale-free-matter-power-spectrum.md) $P(k)=Ak^{n_{\mathrm{eff}}}$, substitute $q=kR$ to obtain

$$
\sigma_R^2=\frac{A}{2\pi^2}R^{-(n_{\mathrm{eff}}+3)}
\int_0^\infty q^{n_{\mathrm{eff}}+2}|\widetilde W(q)|^2\,dq.
$$

Whenever the dimensionless integral is finite and nonzero, this proves the [scale-free smoothed density variance](../../../../../scale-free-smoothed-density-variance.md)

$$
\boxed{\sigma_R\propto R^{-(n_{\mathrm{eff}}+3)/2}.}
$$

The printed condition $n_{\mathrm{eff}}<3$ is insufficient by itself. For a normalized window with $\widetilde W(0)=1$, infrared convergence requires $n_{\mathrm{eff}}>-3$. Ultraviolet convergence depends on the filter: a [spherical top-hat window function](../../../../../spherical-top-hat-window-function.md) requires $n_{\mathrm{eff}}<1$, a Gaussian filter suppresses every ultraviolet power, and a [sharp-k smoothing filter](../../../../../sharp-k-smoothing-filter.md) has finite Fourier support. In particular, the monotone relation $R\to\infty\Rightarrow S=\sigma_R^2\to0$ requires $n_{\mathrm{eff}}>-3$ in the scale-free model.

At a single variance $S_*$, the [Gaussian random field](../../../../../gaussian-random-field.md) has $\delta_{S_*}\sim N(0,S_*)$. Thus its endpoint tail is

$$
\boxed{\mathbb P(\delta_{S_*}\geq\delta_c)=\int_{\delta_c}^{\infty}\frac{e^{-z^2/(2S_*)}}{\sqrt{2\pi S_*}}\,dz
=\frac12\operatorname{erfc}\!\left(\frac{\delta_c}{\sqrt{2S_*}}\right).}
$$

Here $\operatorname{erfc}$ is the complementary [error function](../../../../../error-function.md).

For the crossing probability, the key assumption is independent, symmetric increments as the smoothing scale changes. A [sharp-k smoothing filter](../../../../../sharp-k-smoothing-filter.md), $\widetilde W(kR)=\mathbf1_{k<1/R}$, supplies this property: decreasing $R$ adds independent Fourier shells of the underlying Gaussian field. Parameterizing their accumulated variance by $S$ gives a [Brownian motion](../../../../../brownian-motion-split.md) with covariance $\min(S,S')$. An arbitrary real-space window gives correlated increments and does not justify this argument.

Reflect a trajectory after its first hit of $\delta_c$. The [Strong Markov property](../../../../../strong-markov-property.md) and symmetric future increments preserve its probability, and reflection maps an endpoint below the barrier to one above it. Every endpoint above the barrier has already crossed; the reflected paths give an equally probable set that crossed but ended below. The [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) therefore yields the [excursion-set description of halo formation](../../../../../excursion-set-description-of-halo-formation.md):

$$
\boxed{\mathcal P(S_*)=\mathbb P\!\left(\sup_{0\leq S\leq S_*}\delta_S\geq\delta_c\right)
=\operatorname{erfc}\!\left(\frac{\delta_c}{\sqrt{2S_*}}\right).}
$$

Its derivative is the [Brownian first-passage time](../../../../../brownian-first-passage-time.md) density

$$
f(S)=\frac{\delta_c}{\sqrt{2\pi}S^{3/2}}e^{-\delta_c^2/(2S)}.
$$

The factor of two resolves trajectories that crossed a larger-scale barrier but finish below it on the chosen smaller scale.

Define the [halo peak height](../../../../../halo-peak-height.md) $\nu=\delta_c/\sigma_R$. The cumulative probability $\mathcal P(>M)$ is a dimensionless mass fraction. With $V_M=M/\bar\rho$, its conversion to halo number density gives

$$
\frac{d\bar n_h}{dM}=-\frac{\bar\rho}{M}\frac{d\mathcal P}{dM},\qquad
\frac{d\mathcal P}{dM}=\sqrt{\frac2\pi}\,\frac{\nu}{\sigma_R}e^{-\nu^2/2}\frac{d\sigma_R}{dM}.
$$

Consequently the [Press-Schechter halo mass function](../../../../../press-schechter-halo-mass-function.md) is

$$
\boxed{\frac{d\bar n_h}{dM}=-\sqrt{\frac2\pi}\frac{\bar\rho}{M\sigma_R}\frac{d\sigma_R}{dM}\,\nu e^{-\nu^2/2},\qquad\nu=\frac{\delta_c}{\sigma_R}.}
$$

It is positive when $\sigma_R$ decreases with mass. A chosen mass-radius convention $M\propto R^3$ gives $d\log\sigma_R/d\log M=-(n_{\mathrm{eff}}+3)/6$. For a sharp Fourier filter that mass assignment needs a convention, since its real-space kernel is not a localized top-hat volume.

For [warm dark matter](../../../../../warm-dark-matter.md), the cutoff introduces a new length and invalidates the pure power-law variance scaling near that length. With the same sharp-k filter and $n_{\mathrm{eff}}>-3$, the variance is exactly

$$
\boxed{S(R)=\frac{A}{2\pi^2(n_{\mathrm{eff}}+3)}
\min(R^{-1},k_{\mathrm{WDM}})^{n_{\mathrm{eff}}+3},\qquad
S_{\max}=\frac{A k_{\mathrm{WDM}}^{n_{\mathrm{eff}}+3}}{2\pi^2(n_{\mathrm{eff}}+3)}.}
$$

The Brownian walk runs only up to $S_{\max}$ and then stops. The cutoff does not destroy independence of the Fourier shells that are still present. Thus the first-crossing density and derivative mass-function formula remain valid on the invertible part of $S(M)$, using the actual cutoff variance. For $R<k_{\mathrm{WDM}}^{-1}$, $d\sigma_R/dM=0$ and this idealized sharp-filter model has no new crossings or new low-mass haloes. Its total collapsed fraction is

$$
\boxed{\mathcal P_{\mathrm{collapsed}}=\operatorname{erfc}\!\left(\frac{\delta_c}{\sqrt{2S_{\max}}}\right)<1.}
$$

This is [halo first crossing with a finite variance cutoff](../../../../../halo-first-crossing-with-a-finite-variance-cutoff.md): some trajectories never cross, so one must not force the collapsed fraction to one. The uncut power-law abundance cannot be extrapolated to small masses. For other windows, a variance plateau still occurs but the Markov/reflection derivation is not exact; the same mass function is then a modelling approximation, rather than a result established by this calculation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 310](../../paper-310-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
