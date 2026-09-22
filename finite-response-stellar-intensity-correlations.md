# Finite-response stellar intensity correlations

↑ **Parent:** [Stellar intensity interferometry](stellar-intensity-interferometry.md)

An exact teaching model makes the peak suppression explicit. Assume the narrowband field correlation separates as $g^{(1)}_{12}(B,u)=\gamma(B)g_t^{(1)}(u)$ after delay compensation. Average each channel's [light intensity](light-intensity.md) over the same rectangular gate of duration $T$. The two time integrals have triangular relative-delay weight

$$
W_T(u)=\begin{cases}(T-|u|)/T^2,&|u|\leq T,\\0,&|u|>T,\end{cases}
\qquad \int_{-\infty}^{\infty}W_T(u)\,du=1.
$$

Integrating the [Siegert relation](siegert-relation.md) against this weight gives

$$
\beta=\int_{-\infty}^{\infty}W_T(u)|g_t^{(1)}(u)|^2\,du,
\qquad 0\leq\beta\leq1.
$$

The factor $p$ is one for a selected [polarization of waves](polarization-waves.md) and $1/2$ for two independent equally populated polarizations. The signal fraction $\rho_j=s_j/(s_j+b_j)$ uses mean stellar signal $s_j$ and independent additive background $b_j$ in each detector. The [photon correlation loss and background model](photon-correlation-loss-and-background-model.md) then supplies $\rho_1\rho_2$. This assumes no correlated [sky background](sky-brightness.md) or electronic coupling.

For the original model $|g_t^{(1)}(u)|^2=e^{-|u|/\tau_0}$, elementary [integration](integral-split.md) gives

$$
\beta=\frac{2\tau_0}{T}-2\left(\frac{\tau_0}{T}\right)^2(1-e^{-T/\tau_0}).
$$

The area-based [optical coherence time](optical-coherence-time.md) of this intensity envelope is $\tau_c=\int|g_t^{(1)}(u)|^2du=2\tau_0$. For $T\gg\tau_0$, $\beta\approx\tau_c/T$; for $T\ll\tau_0$, $\beta\to1$. With the chosen $\tau_0=1\,\mathrm{ps}$, $T=50\,\mathrm{ps}$, $p=1$, and $\rho_1=\rho_2=0.8$, $\beta\approx0.0392$ and $g^{(2)}_{\rm obs}(0,0)=1.025088$. At $B=10\,\mathrm m$ the stipulated disk gives approximately $1.013617$. A nearly unit measured $g^{(2)}$ can therefore conceal a substantial $V^2$.

This rectangular-gate calculation specifies a counting model. An analog instrument's amplifier [bandwidth](bandwidth-signal-processing.md) and impulse response instead weight the fluctuations it actually passes; the Sirius amplifiers were bandpass devices. Both require measuring the response and calibrating the zero-baseline excess. When $p$, $\rho_j$, and the temporal response are unchanged, the ratio of excesses recovers $V^2$:

$$
\frac{g^{(2)}_{\rm obs}(B,0)-1}{g^{(2)}_{\rm obs}(0,0)-1}=|\gamma(B)|^2.
$$

A sufficiently unresolved calibration source can supply the denominator; dividing the full $g^{(2)}$ values would give the wrong result. Narrower optical [bandwidth](bandwidth-signal-processing.md) lengthens [optical coherence time](optical-coherence-time.md), whereas wider usable electronic [bandwidth](bandwidth-signal-processing.md) can resolve faster fluctuations; these are distinct bandwidths. Background changes, unequal spectral responses, drift, or averaging over changing [interferometric baselines](interferometric-baseline.md) can invalidate a common calibration. Resolving a disk means establishing a reproducible decline of calibrated correlation, supported by those controls.

## ↑ Ancestors (7)

1. [Stellar intensity interferometry](stellar-intensity-interferometry.md)
2. [Hanbury Brown and Twiss effect](hanbury-brown-and-twiss-effect.md)
3. [Quantum optics](quantum-optics-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
