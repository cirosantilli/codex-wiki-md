<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First consider $k\tau_{\rm eq}<1$. Such a mode remains outside the horizon through [matter-radiation equality](../../../../../../matter-radiation-equality.md), grows as $\tau^2$ on both sides, and keeps the same matter-era growth after entry. Squaring this growth preserves the shape of the [HPZ spectrum](../../../../../../harrison-peebles-zeldovich-spectrum.md):

$$
P(k,\tau)\sim\mathcal C\tau^4 k,\qquad k\tau_{\rm eq}<1,
$$

up to a scale-independent matching coefficient.

For $k\tau_{\rm eq}\gg1$, entry occurs in [radiation domination](../../../../../../radiation-domination.md) at $\tau_H\sim k^{-1}$, with $P_H\sim\mathcal C k^{-3}$. The density amplitude then grows only logarithmically until equality. Thus

$$
\delta_{\rm eq}\sim\delta_H\ln(k\tau_{\rm eq}),\qquad
P_{\rm eq}\sim\mathcal C k^{-3}\ln^2(k\tau_{\rm eq}).
$$

During [matter domination](../../../../../../matter-domination.md), the [matter-era linear growth factor](../../../../../../matter-era-linear-growth-factor.md) of the density is $(\tau/\tau_{\rm eq})^2$, so its square multiplies the [matter power spectrum](../../../../../../matter-power-spectrum.md):

$$
\boxed{P(k,\tau)\sim\mathcal C
\left(\frac{\tau}{\tau_{\rm eq}}\right)^4
k^{-3}\ln^2(k\tau_{\rm eq}),\qquad k\tau_{\rm eq}\gg1.}
$$

The turnover at $k\sim\tau_{\rm eq}^{-1}$ records whether a mode entered during [radiation domination](../../../../../../radiation-domination.md). Earlier-entering small-scale modes miss the rapid $\tau^2$ growth and receive only the logarithmic [Mészáros effect](../../../../../../meszaros-effect.md). This is the origin of the [logarithmic small-scale matter transfer](../../../../../../logarithmic-small-scale-matter-transfer.md). The formula is a large-$k$ asymptote: the additive constant in the logarithmic solution and smooth equality matching must be retained near $k\tau_{\rm eq}=1$, where the spectrum does not vanish.

Multiplying by $k^3$ gives the small-scale mass-fluctuation [variance](../../../../../../variance-split.md)

$$
\boxed{\left\langle\left(\frac{\delta M}{M}\right)_k^2\right\rangle
\sim\mathcal C\left(\frac{\tau}{\tau_{\rm eq}}\right)^4
\ln^2(k\tau_{\rm eq}).}
$$

This gives the requested estimate for modes entering before equality, with the logarithm replaced by a smooth order-one factor in the transition region. On comoving scale $L\sim k^{-1}$, unit variance today requires

$$
\boxed{\mathcal C\sim
\frac{(\tau_{\rm eq}/\tau_0)^4}{\ln^2(\tau_{\rm eq}/L)}.}
$$

For a numerical illustration faithful to this question's flat, matter-plus-radiation background, take $h=0.7$ and $\Omega_r=4.2\times10^{-5}h^{-2}$, hence $\Omega_C=1-\Omega_r\simeq1$ rather than the $0.3$ appropriate to a vacuum-dominated model. Part 1(b), now with $\Omega_m=\Omega_C$, gives $\tau_{\rm eq}\simeq33\,\mathrm{Mpc}$. In this two-component model the same integral is valid all the way to today, giving

$$
\tau_0=\frac{2}{H_0\Omega_C}
\left(\sqrt{\Omega_r+\Omega_C}-\sqrt{\Omega_r}\right)
\simeq8.5\times10^3\,\mathrm{Mpc}.
$$

With $L=3\,\mathrm{Mpc}$, $\tau_0/\tau_{\rm eq}\simeq258$ and $\ln(\tau_{\rm eq}/L)\simeq2.39$. Therefore $\mathcal C\sim[258^4(2.39)^2]^{-1}\simeq4\times10^{-11}$, corresponding to a horizon-entry root-mean-square fluctuation of roughly $6\times10^{-6}$. **A very small primordial amplitude, of order $10^{-10}$ in this schematic normalization, can reach unit small-scale variance by today.** Factors from the Fourier convention, smoothing window and equality matching preclude a precise normalization here. The calculation marks the onset of nonlinear structure formation, where extrapolating the linear solution ceases to be valid. For a universe with late vacuum domination, one must replace the matter-only growth law by its actual growth factor before making a numerical inference.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
