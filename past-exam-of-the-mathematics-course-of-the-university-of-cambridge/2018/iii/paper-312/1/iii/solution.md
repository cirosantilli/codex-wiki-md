<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $\langle\varphi_G(\mathbf k)\varphi_G(\mathbf k')\rangle=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf k')P_\varphi(k)$. For nonzero external momenta, the quadratic term in [local-type primordial non-Gaussianity](../../../../../../local-type-primordial-non-gaussianity.md) is

$$
f_{\rm NL}\int\frac{d^3q}{(2\pi)^3}\varphi_G(\mathbf q)\varphi_G(\mathbf k-\mathbf q).
$$

Insert it in one of the three external fields. [Wick theorem](../../../../../../wick-s-theorem.md) supplies two connected [Wick contractions](../../../../../../wick-contraction.md) at each insertion, whereas the mean subtraction removes the disconnected zero-mode contribution. Thus the leading [primordial bispectrum](../../../../../../primordial-bispectrum.md) is

$$
B_\varphi(k_1,k_2,k_3)=2f_{\rm NL}\bigl[P_\varphi(k_1)P_\varphi(k_2)+P_\varphi(k_2)P_\varphi(k_3)+P_\varphi(k_3)P_\varphi(k_1)\bigr].
$$

Linear propagation by the [cosmological Poisson equation](../../../../../../cosmological-poisson-equation.md) gives $P_m(k)=\alpha(k)^2P_\varphi(k)$ and multiplies the [primordial bispectrum](../../../../../../primordial-bispectrum.md) by $\alpha_1\alpha_2\alpha_3$. Defining the matter three-point function by its momentum-conserving [Dirac delta function](../../../../../../dirac-delta-function.md) times $B_m$, the [primordial contribution to the matter bispectrum](../../../../../../primordial-contribution-to-the-matter-bispectrum.md) is

$$
\boxed{B_m^{\rm prim}=2f_{\rm NL}\left[\frac{\alpha_3}{\alpha_1\alpha_2}P_m(k_1)P_m(k_2)+\frac{\alpha_1}{\alpha_2\alpha_3}P_m(k_2)P_m(k_3)+\frac{\alpha_2}{\alpha_3\alpha_1}P_m(k_3)P_m(k_1)\right]}.
$$

The nonlinear gravitational contribution from [standard perturbation theory in cosmology](../../../../../../standard-perturbation-theory-in-cosmology.md) is excluded here.

In a [squeezed bispectrum configuration](../../../../../../squeezed-bispectrum-configuration.md), $k_1=k_L\ll k_2\simeq k_3=k_S$, so

$$
B_m^{\rm prim}\simeq4f_{\rm NL}\frac{P_m(k_L)P_m(k_S)}{\alpha(k_L)}
+2f_{\rm NL}\frac{\alpha(k_L)}{\alpha(k_S)^2}P_m(k_S)^2.
$$

For a nearly scale-invariant potential, $P_\varphi(k_L)\gg P_\varphi(k_S)$, so the second term is subleading and

$$
\boxed{B_m^{\rm prim}(k_L,k_S,k_S)\simeq\frac{4f_{\rm NL}}{\alpha(k_L)}P_m(k_L)P_m(k_S)}.
$$

Relative to the product of matter [power spectra](../../../../../../power-spectrum.md), the squeezed response is enhanced by $k_L^{-2}$. Its sign is the sign of $f_{\rm NL}$. This is the three-point counterpart of the conditional [short-scale variance modulation by local non-Gaussianity](../../../../../../short-scale-variance-modulation-by-local-non-gaussianity.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
