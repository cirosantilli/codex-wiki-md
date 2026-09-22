# Evanescent penetration depth

↑ **Parent:** [Evanescent field in total internal reflection](evanescent-field-in-total-internal-reflection.md)

Define the amplitude [evanescent penetration depth](evanescent-penetration-depth.md) as the distance at which the [electric field](electric-field-split.md) [wave amplitude](wave-amplitude.md) falls to $1/e$ of its surface value:

$$
\delta=\frac1\kappa=\frac{\lambda_0}{2\pi\sqrt{n_1^2\sin^2\theta-n_2^2}},\qquad
\frac{|\mathbf E(z)|}{|\mathbf E(0)|}=e^{-z/\delta}.
$$

The squared-field envelope decays twice as fast:

$$
\frac{|\mathbf E(z)|^2}{|\mathbf E(0)|^2}=e^{-2z/\delta},\qquad d_{1/e}=\frac\delta2.
$$

The same normalized [exponential decay](exponential-decay.md) describes the tangential average [Poynting vector](poynting-vector.md) for the [TE polarization](transverse-electric-polarization.md) above. An intensity penetration depth convention often means $d_{1/e}$; it must not be confused with amplitude depth $\delta$ or interpreted as outgoing normal [light intensity](light-intensity.md).

For the stipulated $n_1=1.5$, $n_2=1$, $\lambda_0=633\,\mathrm{nm}$ and $\theta=50^\circ$,

$$
\begin{aligned}
k_0&\approx0.00992604314\,\mathrm{nm}^{-1},&
\kappa&\approx0.00561812463\,\mathrm{nm}^{-1},\\
\delta&\approx177.99534\,\mathrm{nm},&
d_{1/e}&\approx88.99767\,\mathrm{nm}.
\end{aligned}
$$

At $z=200\,\mathrm{nm}$ the normalized [wave amplitude](wave-amplitude.md) is approximately $0.325099$, and its squared envelope is approximately $0.105689$. At $z=\delta$, these become $e^{-1}$ and $e^{-2}$, respectively. The quantity inside the [square root](square-root.md) is dimensionless, so $\kappa$ has inverse-length units and both depths have length units.

<a id="image-constructed-evanescent-field-model-at-633-nm-amplitude-and-squared-field-decay-at-50-degrees-and-their-penetration-depths-as-incidence-increases-above-the-critical-angle"></a>
![](evanescent-field-decay-and-penetration-depth.png)

**[Figure 9](#image-constructed-evanescent-field-model-at-633-nm-amplitude-and-squared-field-decay-at-50-degrees-and-their-penetration-depths-as-incidence-increases-above-the-critical-angle). Constructed evanescent-field model at 633 nm: amplitude and squared-field decay at 50 degrees, and their penetration depths as incidence increases above the critical angle**.

The sharp angular dependence has a simple explanation. For $\theta=\theta_c+\varepsilon$ with $\varepsilon>0$ small and measured in [radians](radian.md), a first-order [Taylor expansion](taylor-expansion.md) gives

$$
\delta\sim\frac{\lambda_0}{2\pi\sqrt{2n_1^2\sin\theta_c\cos\theta_c}}\,\varepsilon^{-1/2}.
$$

Thus $\delta\to\infty$ as $\theta\downarrow\theta_c$: exponential confinement disappears continuously. With fixed [refractive indices](refractive-index.md), $\delta$ decreases as the [angle of incidence](angle-of-incidence.md) increases and approaches $\lambda_0/(2\pi\sqrt{n_1^2-n_2^2})\approx90.1091\,\mathrm{nm}$ as $\theta\to90^\circ$. This is a [limit](limit-of-a-function.md) of the normalized depth; exactly grazing incidence supplies zero incident normal [power](power.md). Real beam widths, angular spreads and [optical dispersion](dispersion-optics.md) matter when applying these ideal [plane electromagnetic wave](plane-electromagnetic-wave.md) predictions near the threshold.

## ↑ Ancestors (12)

1. [Evanescent field in total internal reflection](evanescent-field-in-total-internal-reflection.md)
2. [Total internal reflection](total-internal-reflection.md)
3. [Snell law for electromagnetic waves](snell-law-for-electromagnetic-waves.md)
4. [Phase matching at a planar wave interface](phase-matching-at-a-planar-wave-interface.md)
5. [Dielectric-interface boundary conditions](dielectric-interface-boundary-conditions.md)
6. [Interface conditions for electromagnetic fields](interface-conditions-for-electromagnetic-fields.md)
7. [Plane electromagnetic wave](plane-electromagnetic-wave.md)
8. [Electromagnetic wave](electromagnetic-wave-split.md)
9. [Electromagnetism](electromagnetism-split.md)
10. [Branches of physics](branches-of-physics.md)
11. [Physics](physics-split.md)
12. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Evanescent penetration depth](evanescent-penetration-depth.md)
- [Frustrated total internal reflection](frustrated-total-internal-reflection.md)
