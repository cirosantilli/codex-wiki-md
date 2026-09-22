<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a statistically homogeneous [comoving curvature perturbation](../../../../../../comoving-curvature-perturbation.md), define the connected [primordial bispectrum](../../../../../../primordial-bispectrum.md) by

$$
\boxed{\langle\zeta(\boldsymbol k_1)\zeta(\boldsymbol k_2)\zeta(\boldsymbol k_3)\rangle_c
=(2\pi)^3\delta^{(3)}(\boldsymbol k_1+\boldsymbol k_2+\boldsymbol k_3)B(k_1,k_2,k_3).}
$$

[Statistical isotropy](../../../../../../statistical-isotropy.md) makes $B$ depend only on the three magnitudes, which must form a triangle. A [Gaussian random field](../../../../../../gaussian-random-field.md) has zero connected bispectrum. Canonical attractor [single-field slow-roll inflation](../../../../../../single-field-slow-roll-inflation.md) with the usual vacuum produces only slow-roll-sized [primordial non-Gaussianity](../../../../../../primordial-non-gaussianity.md). A measurable signal can arise from additional light fields and nonlinear conversion of [isocurvature perturbations](../../../../../../cosmological-entropy-perturbation.md), or from enhanced interactions such as a small sound speed, departures from an attractor, or suitable features/excited initial states. The resulting model must still reproduce the observed nearly scale-invariant [power spectrum](../../../../../../power-spectrum.md) and remain under perturbative control, with acceptable backreaction and late-time conversion to the observed perturbations. Large non-Gaussianity is therefore possible but is not automatic in a viable model.

Put $c=3f_{\mathrm{NL}}/5$ and use the consistent [Fourier transform](../../../../../../fourier-transform.md) convention with $\zeta_G(\boldsymbol x)$, rather than the repeated momentum argument printed in the integrand. The quadratic part has transform

$$
\zeta(\boldsymbol k)=\zeta_G(\boldsymbol k)+c\int\frac{d^3p}{(2\pi)^3}
\zeta_G(\boldsymbol p)\zeta_G(\boldsymbol k-\boldsymbol p)
-c\langle\zeta_G^2\rangle(2\pi)^3\delta^{(3)}(\boldsymbol k).
$$

The subtraction sets the mean to zero and removes the internal contraction of a single quadratic factor. At first order in $f_{\mathrm{NL}}$, choose one of the three external factors to be quadratic. For example, the two connected [Wick contractions](../../../../../../wick-contraction.md) at the third leg pair its two fields with the first two legs, giving

$$
2c(2\pi)^3\delta^{(3)}(\boldsymbol k_1+\boldsymbol k_2+\boldsymbol k_3)P(k_1)P(k_2).
$$

Summing the three placements proves

$$
\boxed{B^{\mathrm{loc}}=\frac65f_{\mathrm{NL}}\left[P(k_1)P(k_2)+P(k_2)P(k_3)+P(k_3)P(k_1)\right]+O(f_{\mathrm{NL}}^3).}
$$

This is the leading local [primordial bispectrum](../../../../../../primordial-bispectrum.md). The factor $6/5$ is the quadratic coefficient $3/5$ multiplied by the two cross-pairings. Terms of order $f_{\mathrm{NL}}^2$ have an odd Gaussian moment and vanish.

The literal quadratic local model also has a connected cubic-in-$f_{\mathrm{NL}}$ contribution, from one quadratic factor at every leg:

$$
B_{\mathrm{loop}}=8c^3\int\frac{d^3p}{(2\pi)^3}
P(p)P(|\boldsymbol k_1-\boldsymbol p|)P(|\boldsymbol k_2+\boldsymbol p|).
$$

This is the [loop correction to the local primordial bispectrum](../../../../../../loop-correction-to-the-local-primordial-bispectrum.md); regulators may be needed for idealized spectra. Thus the PDF's displayed formula is the tree/leading-order result, not an exact identity for arbitrary $f_{\mathrm{NL}}$. The weak-non-Gaussian expansion assumes these loop terms are small. The local shape is enhanced in the [squeezed bispectrum configuration](../../../../../../squeezed-bispectrum-configuration.md) when a long-wavelength perturbation modulates small-scale power.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
