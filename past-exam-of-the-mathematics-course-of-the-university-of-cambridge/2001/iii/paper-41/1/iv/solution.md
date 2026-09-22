<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the luminosity convention in the supplied flux relation: $P_\nu=L_\nu/(4\pi)$, where $L_\nu$ is the total [spectral luminosity](../../../../../../spectral-luminosity.md). For a general spectrum $P_\nu\propto\nu^\alpha$, the [cosmological spectral flux-density relation](../../../../../../cosmological-spectral-flux-density-relation.md) gives

$$
S_{\nu_0}=\frac{(1+z)P_{(1+z)\nu_0}}{d_L^2}
=\frac{P_{\nu_0}(1+z)^{\alpha-1}}{r_e^2}.
$$

In a spatially flat universe, a shell subtending the [solid angle](../../../../../../solid-angle.md) $d\Omega$ contains $dN=n_0r_e^2dr_e\,d\Omega$ sources, because $n_0$ is their [comoving number density](../../../../../../comoving-number-density.md). The [cosmological spectral background](../../../../../../cosmological-spectral-background.md) intensity per unit [solid angle](../../../../../../solid-angle.md) is consequently

$$
I_{\nu_0}(z_{\max})
=n_0P_{\nu_0}\int_0^{r_e(z_{\max})}(1+z)^{\alpha-1}dr_e
=\frac{cn_0P_{\nu_0}}{H_0}
\int_0^{z_{\max}}(1+z)^{\alpha-5/2}\,dz.
$$

This is the [cosmological background intensity from comoving emissivity](../../../../../../cosmological-background-intensity-from-comoving-emissivity.md) specialized to identical, nonevolving sources in an [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md). For $\alpha=1$ the integrand reduces to $(1+z)^{-3/2}$, or directly $dI_{\nu_0}=n_0P_{\nu_0}dr_e$. The finite [comoving particle horizon](../../../../../../comoving-particle-horizon.md) therefore gives

$$
I_{\nu_0}(z_{\max})=
\frac{2cn_0P_{\nu_0}}{H_0}[1-(1+z_{\max})^{-1/2}],
\qquad
\boxed{I_{\nu_0}(\infty)=\frac{2cn_0P_{\nu_0}}{H_0}.}
$$

For $\alpha=2$, instead,

$$
\boxed{I_{\nu_0}(z_{\max})=
\frac{2cn_0P_{\nu_0}}{H_0}[\sqrt{1+z_{\max}}-1]\longrightarrow\infty.}
$$

The emitted [frequency](../../../../../../frequency.md) grows with [redshift](../../../../../../redshift.md), and the rising [spectral luminosity](../../../../../../spectral-luminosity.md) now defeats the redshift dimming. The [Einstein-de Sitter spectral-background convergence criterion](../../../../../../einstein-de-sitter-spectral-background-convergence-criterion.md) is $\alpha<3/2$; equality produces a logarithmic divergence. This divergence describes the unbounded power-law, eternal-population model. A finite formation epoch, a high-frequency spectral break or absorption changes that model and can make its background finite.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
