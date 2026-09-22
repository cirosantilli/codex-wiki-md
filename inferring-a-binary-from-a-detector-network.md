# Inferring a binary from a detector network

↑ **Parent:** [GW150914](gw150914.md)

For detector $k$, model the calibrated data as $d_k(t)=h_k(t;\theta)+n_k(t)$, with a shared source parameter vector $\theta$, separate detector responses, propagation delays and [noise](noise-signal-processing.md) $n_k$. Under an independent stationary [Gaussian process](gaussian-process-split.md) approximation with one-sided [power spectral density](power-spectral-density.md) $S_k(f)$, define the noise-weighted [inner product](inner-product-split.md) and [likelihood function](likelihood-function.md)

$$
(a|b)_k=4\operatorname{Re}\int_{f_{\min}}^{f_{\max}}\frac{\widetilde a(f)^*\widetilde b(f)}{S_k(f)}\,df,\qquad
\log\mathcal L(\theta)=-\frac12\sum_k(d_k-h_k|d_k-h_k)_k+\mathrm{constant}.
$$

Strain [power spectral density](power-spectral-density.md) has units $\mathrm{Hz}^{-1}$; the displayed [inner product](inner-product-split.md) is dimensionless when the [Fourier transform](fourier-transform-split.md) integrates over seconds. A [matched filter](matched-filter.md) rewards agreement over the full evolving [wave phase](phase-waves.md), weighting frequency bands by their noise. One conspicuous peak is insufficient: a candidate should also have the right distribution of signal across frequency bands and compatible projections in the network.

The parameter paper used coherent [Bayesian inference](bayesian-statistics-split.md), [numerical relativity](numerical-relativity-split.md)-informed inspiral–merger–ringdown models and explicit calibration uncertainties. It found a strong distance–inclination correlation; source-frame [masses](mass.md) additionally require converting the detector-frame masses by a cosmological [redshift](redshift.md).[II Parameter estimation, equations (1)–(5), II.A waveform models; III Results, p. 7, Fig. 2](properties-of-the-binary-black-hole-merger-gw150914-by-b-p-abbott-and-others.md) Conceptually, multiply the [likelihood function](likelihood-function.md) by a [prior distribution](prior-probability.md) to obtain a [posterior distribution](bayesian-posterior.md). Changes in waveform families, residual structure after subtraction, and checks with a generic transient reconstruction test parts of the modeling assumptions. Detection significance and parameter uncertainty answer different questions.

## ↑ Ancestors (6)

1. [GW150914](gw150914.md)
2. [Gravitational wave](gravitational-wave-split.md)
3. [General relativity](general-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
