# Common-ion effect

↑ **Parent:** [Solubility product](solubility-product.md)

The [common-ion effect](common-ion-effect.md) is the change in a [chemical equilibrium](chemical-equilibrium.md) caused by adding an [ion](ion.md) already participating in it. In the fixed-[activity coefficient](activity-coefficient.md) AB model, adding the common B [anion](anion.md) lowers the [molar solubility](molar-solubility.md). The shared [ion](ion.md) participates regardless of which [salt](salt-chemistry.md) supplied it.[Chemistry 2e by Paul Flowers and others; §15.1, Common Ion Effect: adding an ion also produced by dissolution shifts the solubility equilibrium](chemistry-2e-by-paul-flowers-and-others/15-1-precipitation-and-dissolution.md)

The preceding [solubility product and material balance](solubility-product-and-material-balance.md) give a short proof without a qualitative slogan. Taking a [derivative](derivative.md) of $s_*^2+c_0s_*=K_{\mathrm{sp},c}$ at fixed $K_{\mathrm{sp},c}$ gives

$$
(2s_*+c_0)\frac{ds_*}{dc_0}+s_*=0,\qquad
\frac{ds_*}{dc_0}=-\frac{s_*}{2s_*+c_0}<0.
$$

Thus the [molar solubility](molar-solubility.md) decreases continuously as $c_0$ increases. At $c_0=0$, the [derivative](derivative.md) is $-1/2$; for a very large common-ion background, the rationalized expression approaches $K_{\mathrm{sp},c}/c_0$. The [solubility product](solubility-product.md) is fixed within this model even while the [molar solubility](molar-solubility.md) changes.

Neglecting $s_*$ beside $c_0$ replaces $s_*(c_0+s_*)=K_{\mathrm{sp},c}$ by $c_0s_{\mathrm{app}}=K_{\mathrm{sp},c}$. This approximation always overestimates the exact [molar solubility](molar-solubility.md), since it neglects the B [anions](anion.md) supplied by AB itself. For $c_0>0$, its [relative error](relative-error.md) has an exact simple form:

$$
s_{\mathrm{app}}=\frac{K_{\mathrm{sp},c}}{c_0}
=s_*+\frac{s_*^2}{c_0},\qquad
\frac{s_{\mathrm{app}}-s_*}{s_*}=\frac{s_*}{c_0}.
$$

At $c_0=0.030\,\mathrm M$, $s_{\mathrm{app}}=0.003333333\,\mathrm M$, approximately $10.1\%$ too high. At $c_0=0.100\,\mathrm M$, $s_*=0.000990195\,\mathrm M$ and $s_{\mathrm{app}}=0.001000000\,\mathrm M$, approximately $0.990\%$ too high. A small [solubility product](solubility-product.md) by itself does not justify the approximation: the common-ion background must be large compared with the resulting [molar solubility](molar-solubility.md).

<a id="image-common-ion-suppression-and-the-error-from-neglecting-the-solid-s-own-b-anions"></a>
![](common-ion-solubility-exact-and-approximate.png)

**[Figure 3](#image-common-ion-suppression-and-the-error-from-neglecting-the-solid-s-own-b-anions). Common-ion suppression and the error from neglecting the solid's own B anions**. Original curves for the same stipulated AB model, with exact [molar solubility](molar-solubility.md) and $K_{\mathrm{sp},c}/c_0$ approximation. The exact curve reaches $0.010\,\mathrm M$ at $c_0=0$; the approximation diverges there. The lower panel shows its exact [relative error](relative-error.md), with markers at $0.030$ and $0.100\,\mathrm M$. No curve represents experimental measurements of a named substance.

For a desired fractional [relative error](relative-error.md) at most $\varepsilon>0$, substituting $s_*/c_0\leq\varepsilon$ into the exact balance gives the equivalent criterion

$$
c_0\geq\sqrt{\frac{K_{\mathrm{sp},c}}{\varepsilon(1+\varepsilon)}}.
$$

For this model, a $5\%$ tolerance requires $c_0\geq0.0436436\,\mathrm M$. This bound concerns only the algebraic approximation. In a real [chemical solution](solution-chemistry.md), changes in [ionic strength](ionic-strength.md) and [activity coefficients](activity-coefficient.md), or competing [chemical reactions](chemical-reaction-split.md), can invalidate a constant $K_{\mathrm{sp},c}$ even when this bound is met.

## ↑ Ancestors (5)

1. [Solubility product](solubility-product.md)
2. [Precipitation (chemistry)](precipitation-chemistry.md)
3. [Chemical reaction](chemical-reaction-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Common-ion effect](common-ion-effect.md)
