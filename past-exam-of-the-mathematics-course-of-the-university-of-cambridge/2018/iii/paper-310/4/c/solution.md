<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the Fourier normalization of the PDF. The [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) obey

$$
\boxed{[\widehat a_{\mathbf k},\widehat a_{\mathbf k'}^\dagger]=\delta^3(\mathbf k-\mathbf k'),\qquad
[\widehat a_{\mathbf k},\widehat a_{\mathbf k'}]=[\widehat a_{\mathbf k}^\dagger,\widehat a_{\mathbf k'}^\dagger]=0.}
$$

There is no $(2\pi)^3$ in this commutator because the expansion uses $(2\pi)^{-3/2}$. The [Bunch-Davies vacuum](../../../../../../bunch-davies-vacuum.md) satisfies $\widehat a_{\mathbf k}|0\rangle=0$. Write $u_k=f_k^*$ for the coefficient of the annihilation operator. Only the contraction $\langle0|\widehat a_{\mathbf k}\widehat a_{\mathbf k'}^\dagger|0\rangle=\delta^3(\mathbf k-\mathbf k')$ contributes, so

$$
\boxed{\langle0|\widehat{\delta\phi}(\tau,\mathbf x)\widehat{\delta\phi}(\tau,\mathbf x+\mathbf r)|0\rangle
=\int\frac{d^3k}{(2\pi)^3}\frac{|u_k(\tau)|^2}{a^2}e^{-i\mathbf k\cdot\mathbf r}.}
$$

The given mode has

$$
|u_k|^2=\frac1{2k}\left(1+\frac1{k^2\tau^2}\right).
$$

Since $a^{-2}=H^2\tau^2$, the [equal-time two-point function of a de Sitter scalar](../../../../../../equal-time-two-point-function-of-a-de-sitter-scalar.md) therefore has dimensional power spectrum

$$
P_{\delta\phi}(k,\tau)=\frac{H^2}{2k^3}(1+k^2\tau^2).
$$

Comparing with the dimensionless power convention in the hint gives

$$
\boxed{\Delta_{\delta\phi}^2(k,\tau)=\frac{k^3}{2\pi^2}P_{\delta\phi}(k,\tau)
=\left(\frac{H}{2\pi}\right)^2(1+k^2\tau^2).}
$$

Equivalently, angular integration expresses the correlation as $\int_0^\infty(dk/k)\,\Delta_{\delta\phi}^2\sin(kr)/(kr)$, where $r=|\mathbf r|$.

On [superhorizon scales](../../../../../../superhorizon-scale.md), $k\ll aH$ is $|k\tau|\ll1$, and

$$
\boxed{\Delta_{\delta\phi}^2\longrightarrow\left(\frac H{2\pi}\right)^2.}
$$

This [scale-invariant inflationary power spectrum](../../../../../../scale-invariant-inflationary-power-spectrum.md) gives equal variance per logarithmic wavenumber interval. It is exactly scale invariant in the massless constant-$H$ approximation here; slow evolution of $H$ and small field mass produce a small [spectral tilt](../../../../../../scalar-spectral-index.md). Such quantum [primordial perturbations](../../../../../../primordial-perturbation.md) supply the initial fluctuations that subsequently seed cosmological structure after conversion to curvature and density perturbations. The curvature conversion itself requires the metric perturbations excluded from this calculation.

The continuum correlation is understood with the usual infrared regulator, such as finite volume or finite inflationary duration. The strictly massless infinite-volume model has a logarithmic infrared divergence. Coincident products also require ultraviolet regularization or smearing; the finite mode spectrum is unaffected by these qualifications.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
