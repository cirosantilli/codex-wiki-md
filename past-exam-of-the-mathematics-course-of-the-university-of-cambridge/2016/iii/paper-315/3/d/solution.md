<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The stellar luminosity is $L_\star=4\pi R_\star^2\sigma_{\rm SB}T_\star^4$. At separation $a$, the planet intercepts a disk of area $\pi R_p^2$. For [Bond albedo](../../../../../../bond-albedo.md) $A_B$ and uniform emission over its full surface, energy balance gives

$$
(1-A_B)\frac{L_\star}{4\pi a^2}\pi R_p^2=4\pi R_p^2\sigma_{\rm SB}T_e^4,
\qquad
\boxed{T_e=T_\star\left(\frac{R_\star}{2a}\right)^{1/2}(1-A_B)^{1/4}.}
$$

This [planetary equilibrium temperature](../../../../../../planetary-equilibrium-temperature.md) neglects intrinsic heat. Dayside-only or nonuniform emission changes the redistribution factor.

For the [single-layer greenhouse model](../../../../../../single-layer-greenhouse-model.md), assume a black infrared surface, an atmosphere transparent to incoming stellar radiation, and infrared absorptivity/emissivity $\alpha$. Let $T_s$ be surface temperature and $T_a$ layer temperature. Kirchhoff's law makes the layer's emission in each direction $\alpha\sigma_{\rm SB}T_a^4$. Its balance is

$$
\alpha\sigma_{\rm SB}T_s^4=2\alpha\sigma_{\rm SB}T_a^4,
$$

so $T_a^4=T_s^4/2$ for $\alpha>0$. Surface balance includes the downward layer emission:

$$
\sigma_{\rm SB}T_e^4+\alpha\sigma_{\rm SB}T_a^4=\sigma_{\rm SB}T_s^4.
$$

Therefore

$$
\boxed{T_s=T_e(1-\alpha/2)^{-1/4}.}
$$

The no-atmosphere limit is $T_s=T_e$, and a completely IR-absorbing single layer gives **$T_s=2^{1/4}T_e$**. The outgoing flux $(1-\alpha)\sigma T_s^4+\alpha\sigma T_a^4$ remains $\sigma T_e^4$. The layer delays escape by absorption and re-emission; it does not permanently retain a fraction $\alpha$ of every emitted photon, which would incorrectly predict a divergent temperature at $\alpha=1$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
