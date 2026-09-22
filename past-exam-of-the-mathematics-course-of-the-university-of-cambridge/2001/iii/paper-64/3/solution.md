<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Polyakov path integral](../../../../../polyakov-path-integral.md) integrates over both the [string embedding map](../../../../../string-embedding-map.md) and the [worldsheet metric](../../../../../worldsheet-metric.md). After the usual analytic continuation, a formal closed-string vacuum functional has the schematic form

$$
Z=\sum_{g\ge0}g_s^{2g-2}\int\frac{\mathcal DX\,\mathcal Dh}{\operatorname{Vol}(\operatorname{Diff}\times\operatorname{Weyl})}e^{-S_E[X,h]},\qquad
S_E=\frac1{4\pi\alpha'}\int\sqrt h\,h^{ab}\partial_aX\cdot\partial_bX\,d^2\sigma.
$$

The genus weights organize [string perturbation theory](../../../../../string-perturbation-theory.md); the coupling $g_s$ is related to the constant [dilaton](../../../../../dilaton.md). External states are inserted as [string vertex operators](../../../../../string-vertex-operator.md), with the usual additional external coupling normalization. Division by the gauge group prevents counting different parameterizations and Weyl representatives as distinct configurations.

Gauge-fix $h=e^{2\phi}\widehat h(m)$, where $m$ labels inequivalent conformal structures. [Conformal gauge](../../../../../conformal-gauge.md) fixes the local metric redundancies, not the [worldsheet moduli](../../../../../worldsheet-moduli.md). Unmarked compact surfaces have no complex moduli at genus zero, one at genus one and $3g-3$ at genus $g\ge2$. Integrating over the appropriate moduli quotient includes large diffeomorphisms; at genus one it requires a modular fundamental domain, as in [torus modular invariance](../../../../../torus-modular-invariance.md).

The infinitesimal traceless diffeomorphism operator is

$$
(P_1c)_{ab}=\nabla_ac_b+\nabla_bc_a-h_{ab}\nabla_dc^d.
$$

Its [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is represented by anticommuting [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md) $c^a$ and traceless symmetric $b^{ab}$, with action proportional to $\int\sqrt h\,b^{ab}(P_1c)_{ab}$. In conformal complex coordinates this is the pair of chiral [bc systems](../../../../../bc-system.md) of weights $(2,-1)$. Ghost zero modes must be handled rather than included in an ordinary nonzero determinant: conformal Killing vectors correspond to residual gauge transformations, while antighost zero modes pair with surviving moduli variations. At genus zero three insertion positions can be fixed by the [Möbius transformations](../../../../../mobius-transformation.md); corresponding $c\widetilde c$ factors supply the ghost zero modes. At higher genus the measure includes antighost insertions paired with the moduli.

In a flat target, integrating the free coordinate fields gives a Gaussian determinant $[\det'(-\Delta_{\widehat h})]^{-d/2}$, with the zero-mode integral supplying target volume or momentum conservation. Vertex insertions give the corresponding free-field correlators. For example, on a sphere, exponential operators have the factor

$$
\left\langle\prod_i:e^{ik_i\cdot X(z_i)}:\right\rangle
\propto\delta^{(d)}\left(\sum_i k_i\right)\prod_{i<j}|z_i-z_j|^{\alpha'k_i\cdot k_j}.
$$

The remaining unfixed insertion positions and moduli are integrated with the ghost measure. Physical closed-string operators have matter conformal weights $(1,1)$; an unintegrated insertion is $c\widetilde c V$, while an integrated insertion uses $\int d^2z\,V$. This explains how on-shell scattering amplitudes arise from the metric-and-embedding functional integral.

The quantum measure can break the classical Weyl symmetry. Each free coordinate contributes central charge one, while each chiral reparameterization ghost system contributes $-26$. Hence $c_{\rm total}=d-26$, and the [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md) vanishes for the ordinary flat bosonic string exactly at **$d=26$**. Only then can the conformal factor be removed as a gauge degree of freedom without adding further dynamics. For a subcritical matter system it generally produces a Liouville-type theory, unless an appropriate additional conformal sector restores the central charge balance.

Equivalently the gauge-fixed construction uses a nilpotent string [BRST operator](../../../../../brst-operator.md). Physical states are its closed states modulo exact states, expressing the [BRST cohomology](../../../../../brst-cohomology.md) of the gauge constraints. In the critical theory the ghost and matter contributions make this operator nilpotent and the measure gauge independent. Degenerations of moduli describe long-tube propagation and factorization onto intermediate string states. The bosonic tachyon can still cause infrared divergences; anomaly cancellation is not a claim that every vacuum integral is finite or that the bosonic vacuum is stable. **The path integral sums embeddings and conformal structures, with ghosts removing local gauge overcounting and moduli retaining the genuine geometry.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
