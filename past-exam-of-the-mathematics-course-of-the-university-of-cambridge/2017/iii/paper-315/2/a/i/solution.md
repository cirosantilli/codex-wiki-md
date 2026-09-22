<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the collisionless [exosphere](../../../../../../../exosphere.md), an atom escapes if its outward trajectory has positive total mechanical [energy](../../../../../../../energy.md). Neglect tides and stellar forces and use [Newtonian gravity](../../../../../../../gravitational-acceleration.md) at exobase [radius](../../../../../../../radius.md) $r_e$:

$$
\frac12mv^2>\frac{GM_pm}{r_e},\qquad
v>v_{\rm esc}=\sqrt{\frac{2GM_p}{r_e}}.
$$

With thermal speed $v_{\rm th}=\sqrt{2k_BT_e/m}$, the [Jeans escape parameter](../../../../../../../jeans-escape-parameter.md) is

$$
\lambda_e=\frac{v_{\rm esc}^2}{v_{\rm th}^2}
=\frac{GM_pm}{k_BT_er_e}.
$$

A thermal distribution always has an escaping tail; [Jeans escape](../../../../../../../jeans-escape.md) is exponentially suppressed for $\lambda_e\gg1$, with [Jeans escape flux](../../../../../../../jeans-escape-flux.md) proportional to $(1+\lambda_e)e^{-\lambda_e}$. Efficient escape requires $\lambda_e$ of order a few or smaller, with an order-unity energetic estimate $k_BT_e\sim GM_pm/r_e$.

Assume a [Neptune](../../../../../../../neptune.md)-like [mass](../../../../../../../mass.md) and [radius](../../../../../../../radius.md), $r_e\simeq R_p$, and atomic [hydrogen](../../../../../../../hydrogen.md). Using the supplied rounded constants gives

$$
g\simeq17.5\,\mathrm{m\,s^{-2}},\qquad
v_{\rm esc}\simeq2.65\times10^4\,\mathrm{m\,s^{-1}},\qquad
\frac{GM_pm_H}{k_BR_p}\simeq3.5\times10^4\,\mathrm K.
$$

Hence

$$
\boxed{T_e\sim10^4\text{--}4\times10^4\,\mathrm K
\text{ for a few-to-unity Jeans parameter at }r_e\simeq R_p.}
$$

Using the mean kinetic energy $3k_BT/2$ instead gives an order-unity coefficient and $T\simeq2.3\times10^4\,\mathrm K$. An expanded [exobase](../../../../../../../exobase.md) has weaker binding and lowers the estimate by $R_p/r_e$. A comet-like tail can also be shaped by [radiation pressure](../../../../../../../radiation-pressure.md) and stellar-wind interactions; it does not by itself measure $T_e$ or prove that a hydrostatic Jeans model is valid. At $\lambda_e\sim1$, $H/r_e\sim1$ and [hydrostatic equilibrium](../../../../../../../hydrostatic-equilibrium.md) fails as a global description: substantial mass loss must usually be treated as [hydrodynamic atmospheric escape](../../../../../../../hydrodynamic-escape.md).

The [exobase](../../../../../../../exobase.md) is defined by [mean free path](../../../../../../../mean-free-path.md) $\ell\sim H$, not by a universal [pressure](../../../../../../../pressure.md). For a neutral hydrostatic gas with [collision cross-section](../../../../../../../collision-cross-section.md) $\sigma_c$,

$$
\ell\sim\frac1{n_e\sigma_c},\quad H\simeq\frac{k_BT_e}{m_Hg},\quad
\boxed{P_e=n_ek_BT_e\sim\frac{m_Hg}{\sigma_c}.}
$$

For example, explicitly assuming $\sigma_c\sim10^{-19}\text{--}10^{-20}\,\mathrm{m^2}$ gives $P_e\sim2\times10^{-7}\text{--}2\times10^{-6}\,\mathrm{Pa}$, or $2\times10^{-12}\text{--}2\times10^{-11}\,\mathrm{bar}$. These are representative extremely dilute neutral-exobase pressures, with orders of magnitude varying with composition, cross-sections and expansion. The supplied constants contain no collision information, so they cannot uniquely determine an exobase [pressure](../../../../../../../pressure.md); ionization or a non-hydrostatic density profile changes this estimate.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 315](../../../../paper-315-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
