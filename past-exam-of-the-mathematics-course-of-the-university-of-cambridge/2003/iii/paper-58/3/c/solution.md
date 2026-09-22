<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Neglecting the rapidly oscillating radiation source on subhorizon scales, [stress-energy conservation](../../../../../../stress-energy-conservation.md) and the trace of the [Einstein field equations](../../../../../../einstein-field-equations.md) give

$$
\delta_m''+\mathcal H\delta_m'-4\pi Ga^2\rho_m\delta_m=0.
$$

Equivalently in [cosmic time](../../../../../../cosmic-time.md), $\delta_{m,tt}+2H\delta_{m,t}-4\pi G\rho_m\delta_m=0$. Radiation still contributes to the background expansion, even when its perturbation source is averaged away.

Put $\eta=a/a_{\rm eq}$ and let $\rho_{\rm eq}$ be the density of either component at [matter-radiation equality](../../../../../../matter-radiation-equality.md). Then $\rho_m=\rho_{\rm eq}\eta^{-3}$ and $\rho_r=\rho_{\rm eq}\eta^{-4}$. With $C=(8\pi G/3)\rho_{\rm eq}a_{\rm eq}^2$, the [Friedmann equation](../../../../../../friedmann-equations.md) gives

$$
\mathcal H^2=C\frac{1+\eta}{\eta^2},\quad
(\eta')^2=C(1+\eta),\quad \eta''=\frac C2,\quad
4\pi Ga^2\rho_m=\frac{3C}{2\eta}.
$$

Apply the [chain rule](../../../../../../chain-rule.md) to the density equation:

$$
C(1+\eta)\delta_{\eta\eta}+C\left(\frac12+\frac{1+\eta}{\eta}\right)\delta_\eta-\frac{3C}{2\eta}\delta=0.
$$

Thus the [Mészáros equation](../../../../../../meszaros-equation.md) is

$$
\boxed{2\eta(1+\eta)\delta_{\eta\eta}+(2+3\eta)\delta_\eta-3\delta=0.}
$$

Substituting $D_+=1+3\eta/2$ gives $(2+3\eta)(3/2)-3(1+3\eta/2)=0$, so

$$
\boxed{\delta_m=A(\mathbf x)(1+3\eta/2)}
$$

is indeed a solution. It is approximately constant during [radiation domination](../../../../../../radiation-domination.md) and grows as $a$ during [matter domination](../../../../../../matter-domination.md). The second independent solution is

$$
D_-=(1+3\eta/2)\log\frac{\sqrt{1+\eta}+1}{\sqrt{1+\eta}-1}-3\sqrt{1+\eta},
$$

which behaves as $\log(4/\eta)-3$ at small $\eta$. Thus smoothing radiation does not eliminate every logarithmic solution; matching through actual horizon entry fixes the combination excited.

Modes with $k\ll k_{\rm eq}$ enter after equality and retain the $P(k)\propto k$ shape. Modes with $k\gg k_{\rm eq}$ enter during radiation domination: their horizon-entry spectrum is $P_H\propto k^{-3}$ and they gain little growth until equality. The late [matter power spectrum](../../../../../../matter-power-spectrum.md) therefore turns over near $k_{\rm eq}$ and has **a large-scale $k$ branch and a small-scale $k^{-3}$ branch**, with the more accurate radiation-era matching giving

$$
P(k)\propto k^{-3}\log^2(k/k_{\rm eq})\quad(k\gg k_{\rm eq}).
$$

Equivalently the [cold-dark-matter transfer function](../../../../../../cold-dark-matter-transfer-function.md) falls approximately as $(k_{\rm eq}/k)^2$, up to the logarithm. The turnover is the consequence of the [Mészáros effect](../../../../../../meszaros-effect.md); it is not a change of the primordial scale-invariance condition.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
