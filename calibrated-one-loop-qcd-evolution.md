# Calibrated one-loop QCD evolution

↑ **Parent:** [Asymptotic freedom](asymptotic-freedom.md)

A useful original example fixes five active [quark flavors](quark-flavor.md) and chooses $Q_0=20\,\mathrm{GeV}$ and $\alpha_0=\alpha_s(Q_0)=0.16$. These are illustrative inputs, not a measured determination. Integrating $d(1/\alpha_s)/d\ln Q=\beta_0/(2\pi)$ with $\beta_0=23/3$ gives

$$
\alpha_s^{-1}(Q)=6.25+\frac{23}{6\pi}\ln\frac{Q}{20\,\mathrm{GeV}},\qquad
\Lambda=Q_0\exp\!\left(-\frac{2\pi}{\beta_0\alpha_0}\right)\simeq0.1193\,\mathrm{GeV}.
$$

Consequently $\alpha_s(10\,\mathrm{GeV})\simeq0.1850$, $\alpha_s(40\,\mathrm{GeV})\simeq0.1409$, and $\alpha_s(100\,\mathrm{GeV})\simeq0.1217$. Substituting $Q=Q_0$ returns the input, while differentiating returns the stated [beta function](beta-function-physics.md). Rescaling all dimensional inputs by the same factor leaves the [QCD coupling](strong-coupling-constant.md) unchanged: only [ratios](ratio.md) enter. The [reciprocal](multiplicative-inverse.md) [QCD coupling](strong-coupling-constant.md) is a straight line against $\ln(Q/Q_0)$, so the calibration sets the intercept and $n_f$ sets the slope.

Changing the physical probe [energy](energy-split.md) and changing an auxiliary [renormalization scale](renormalization-scale.md) are different operations. To isolate the latter, hold a hypothetical hard scale $Q_h=20\,\mathrm{GeV}$ fixed and define $a(\mu)=\alpha_s(\mu)/\pi$, $b=\beta_0/4$, and the toy approximations

$$
R_1(\mu)=1+a(\mu),\qquad
R_2(\mu)=1+a(\mu)+b\,a(\mu)^2\ln\frac{\mu^2}{Q_h^2}.
$$

Using the one-[loop order](loop-order.md) equation $da/d\ln\mu^2=-ba^2$ gives

$$
\frac{dR_1}{d\ln\mu^2}=-ba^2,\qquad
\frac{dR_2}{d\ln\mu^2}=-2b^2a^3\ln\frac{\mu^2}{Q_h^2}.
$$

The explicit [logarithm](logarithm.md) cancels the order-$a^2$ scale drift. At $\mu=10,20,40\,\mathrm{GeV}$, respectively, $R_1\simeq1.0589,1.0509,1.0449$, whereas $R_2\simeq1.0497,1.0509,1.0502$. These are values of an invented [dimensionless](dimensionless-quantity.md) observable chosen to expose the cancellation; they are not a [cross section](cross-section-physics.md) prediction. Smaller residual scale variation does not bound the unknown constant at the next [loop order](loop-order.md).

<a id="image-calibrating-a-running-coupling-and-cancelling-leading-auxiliary-scale-dependence"></a>
![](qcd-calibrated-inverse-coupling.png)

**[Figure 4](#image-calibrating-a-running-coupling-and-cancelling-leading-auxiliary-scale-dependence). Calibrating a running coupling and cancelling leading auxiliary-scale dependence**. Left: the original five-[quark flavor](quark-flavor.md) calibration written as an inverse [QCD coupling](strong-coupling-constant.md). Right: varying the [renormalization scale](renormalization-scale.md) at fixed $Q_h$ in the original toy $R_1,R_2$. The reduced variation illustrates cancellation between running and an explicit [logarithm](logarithm.md); it is not an experimental uncertainty band.

## ↑ Ancestors (10)

1. [Asymptotic freedom](asymptotic-freedom.md)
2. [Beta function (physics)](beta-function-physics.md)
3. [Running coupling](running-coupling.md)
4. [Renormalization scale](renormalization-scale.md)
5. [Renormalization](renormalization.md)
6. [Perturbative quantum field theory](perturbative-quantum-field-theory-split.md)
7. [Quantum field theory](quantum-field-theory-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)
