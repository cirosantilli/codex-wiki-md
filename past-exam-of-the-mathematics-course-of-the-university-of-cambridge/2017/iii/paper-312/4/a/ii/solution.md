<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $K=k_1+k_2+k_3>0$ and $C=\epsilon+1-c_s^2$. The [inflationary scalar Fourier mode](../../../../../../../inflationary-scalar-fourier-mode.md) has real late-time value $A_k=H/\sqrt{4\epsilon M_{\rm Pl}^2c_sk^3}$ and $u_k'^*(\tau)=A_kc_s^2k^2\tau e^{ikc_s\tau}$. Thus the time integrand, before the factor $-2i$, is

$$
\frac{M_{\rm Pl}^2\epsilon C}{H^2c_s^2\tau}\prod_{r=1}^3u_{k_r}(0)u_{k_r}'{}^*(\tau)=\frac{H^4c_sC}{64\epsilon^2M_{\rm Pl}^4k_1k_2k_3}\tau^2e^{ic_sK\tau}.
$$

The [Bunch-Davies vacuum](../../../../../../../bunch-davies-vacuum.md) prescription supplies damping in the past. Equivalently, use a positive regulator $d$ and then take the limit:

$$
\int_{-\infty}^0\tau^2e^{(d+ic_sK)\tau}\,d\tau=\frac2{(d+ic_sK)^3}\longrightarrow\frac{2i}{c_s^3K^3}\qquad(d\downarrow0).
$$

The real part of $-2i$ times this integral is $4/(c_s^3K^3)$. Including the six [Wick contractions](../../../../../../../wick-contraction.md) yields the [cubic time-derivative curvature bispectrum](../../../../../../../cubic-time-derivative-curvature-bispectrum.md)

$$
\boxed{B(k_1,k_2,k_3)=\frac{3H^4(\epsilon+1-c_s^2)}{8\epsilon^2M_{\rm Pl}^4c_s^2k_1k_2k_3(k_1+k_2+k_3)^3}.}
$$

The resulting [primordial bispectrum](../../../../../../../primordial-bispectrum.md) is a [homogeneous function](../../../../../../../homogeneous-function.md) of degree $-6$ in the wavenumbers, as expected for scale-independent background parameters.

The printed limit $c_s\ll0$ is not a physical sound-speed limit for these modes. The normalization and positive-frequency choice assume $c_s>0$; a negative value is outside the positive sound-speed convention used by these modes. The likely intended limit is **$0<c_s\ll1$**, which is analyzed explicitly here rather than silently substituted for the PDF.

To compare [primordial non-Gaussianity](../../../../../../../primordial-non-gaussianity.md), normalize by the [power spectrum](../../../../../../../power-spectrum.md), not only by the raw three-point amplitude. Here

$$
P_\zeta(k)=\frac{H^2}{4\epsilon M_{\rm Pl}^2c_sk^3},\qquad \Delta_\zeta^2=\frac{k^3P_\zeta(k)}{2\pi^2}=\frac{H^2}{8\pi^2\epsilon M_{\rm Pl}^2c_s}.
$$

At an [equilateral bispectrum configuration](../../../../../../../equilateral-bispectrum-configuration.md), the exact normalized amplitude is

$$
\boxed{\frac{B(k,k,k)}{P_\zeta(k)^2}=\frac29(\epsilon+1-c_s^2).}
$$

Thus $c_s\to1$ gives an amplitude of order $\epsilon$, consistent with weak non-Gaussianity in [single-field slow-roll inflation](../../../../../../../single-field-slow-roll-inflation.md). For $0<c_s\ll1$, this vertex gives an amplitude of order one, enhanced relative to the slow-roll limit but not diverging as $c_s^{-2}$ after power-spectrum normalization. At fixed $H,\epsilon,M_{\rm Pl}$ the raw bispectrum does scale as $c_s^{-2}$, but $P_\zeta^2$ has the same scaling. The often-quoted larger small-sound-speed amplitudes of more general inflationary actions require their actual interaction coefficients and other vertices; they do not follow from the lone supplied vertex. These conclusions concern its tree contribution within the stated weak-perturbation approximation.

The [bispectrum shape function](../../../../../../../primordial-bispectrum-shape-function.md) is

$$
S\propto\frac{k_1k_2k_3}{(k_1+k_2+k_3)^3}.
$$

At fixed perimeter, the [arithmetic-geometric mean inequality](../../../../../../../arithmetic-geometric-mean-inequality.md) bounds this by $1/27$, attained only at an [equilateral bispectrum configuration](../../../../../../../equilateral-bispectrum-configuration.md). In a [squeezed bispectrum configuration](../../../../../../../squeezed-bispectrum-configuration.md) with $k_1=q\ll k_2\simeq k_3=k$, it behaves as $q/(8k)\to0$. At a [flattened bispectrum configuration](../../../../../../../flattened-bispectrum-configuration.md) $(k,k,2k)$ it is finite, $1/32$, with no boundary singularity. Thus **the shape prefers equilateral triangles and suppresses squeezed triangles**, with a broad finite flattened contribution. This is a shape preference, not a complete signal-to-noise calculation: actual observational weighting also depends on [cosmological transfer functions](../../../../../../../cosmological-transfer-function.md), [covariance](../../../../../../../covariance.md) and accessible triangles. If $C=0$, this vertex produces no bispectrum at any configuration; if $C<0$, the signed shape reverses while its absolute triangle preference is unchanged.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
