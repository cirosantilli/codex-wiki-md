# Siegert relation

↑ **Parent:** [Stellar intensity interferometry](stellar-intensity-interferometry.md)

For one selected [polarization of waves](polarization-waves.md), write the detected complex fields as $E_1(t),E_2(t+\tau)$ and their [light intensities](light-intensity.md) as $I_j=|E_j|^2$, absorbing a common conversion constant. With stationary [ensemble averages](expected-value-split.md) and nonzero $\bar I_j=\langle I_j\rangle$, define

$$
g^{(1)}_{12}(B,\tau)=\frac{\langle E_1^*(t)E_2(t+\tau)\rangle}{\sqrt{\bar I_1\bar I_2}},
\qquad
g^{(2)}_{12}(B,\tau)=\frac{\langle I_1(t)I_2(t+\tau)\rangle}{\bar I_1\bar I_2}.
$$

Here [second-order optical coherence](second-order-optical-coherence.md) concerns distinct detector channels, with the corresponding [normal ordering](normal-ordering.md) in the quantum formulation. Independent detection has $g^{(2)}=1$. Subtracting the means gives the normalized [covariance](covariance.md)

$$
\frac{\langle\delta I_1(t)\delta I_2(t+\tau)\rangle}{\bar I_1\bar I_2}=g^{(2)}_{12}(B,\tau)-1.
$$

Thus multiplying raw [photocurrents](photocurrent.md) contains a large mean-product contribution; multiplying their fluctuations isolates the small excess. Independent detector [shot noise](shot-noise.md) does not supply a mean cross-channel excess, although it increases [measurement uncertainty](measurement-uncertainty.md).

The displayed [Siegert relation](siegert-relation.md) requires a zero-mean, jointly circular complex [Gaussian random field](gaussian-random-field.md), the usual chaotic [thermal light](thermal-light.md) model. Circular means invariance under a common arbitrary complex phase rotation; in particular $\langle E_iE_j\rangle=0$. Apply the [Gaussian moment pairing theorem](isserlis-s-theorem.md) to the real and imaginary parts:

$$
\langle E_1^*E_1E_2^*E_2\rangle
=\langle|E_1|^2\rangle\langle|E_2|^2\rangle
+|\langle E_1^*E_2\rangle|^2.
$$

The remaining pairing vanishes by circularity. Division proves the [Siegert relation](siegert-relation.md). Gaussianity is an assumption about fourth moments, not a consequence of merely measuring [first-order optical coherence](first-order-optical-coherence.md); a [coherent state](coherent-state.md) or [photon antibunching](photon-antibunching.md) cannot be interpreted by this thermal formula.

For equal-intensity beams combined in a common optical mode with matched [wave polarizations](polarization-waves.md), [interferometric visibility](interferometric-visibility.md) is $V=|g^{(1)}_{12}|$. Consequently ideal thermal [stellar intensity interferometry](stellar-intensity-interferometry.md) measures $g^{(2)}-1=V^2$, while the full $g^{(2)}$ includes the independent-count reference one. Unpolarized [thermal light](thermal-light.md) with two independent equally populated [wave polarizations](polarization-waves.md) has half this excess: adding their [covariances](covariance.md) doubles the numerator while multiplying total means quadruples the denominator. Finite detector response further suppresses the peak and must be calibrated.[Guerin and others, Spatial intensity interferometry on three bright stars, arXiv:1805.06653v2 (13 August 2018), §§2.1–2.3: normalized correlation, thermal contrast and temporal-response calibration](spatial-intensity-interferometry-on-three-bright-stars-by-william-guerin-and-others.md)

## ↑ Ancestors (7)

1. [Stellar intensity interferometry](stellar-intensity-interferometry.md)
2. [Hanbury Brown and Twiss effect](hanbury-brown-and-twiss-effect.md)
3. [Quantum optics](quantum-optics-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Finite-response stellar intensity correlations](finite-response-stellar-intensity-correlations.md)
- [Siegert relation](siegert-relation.md)
