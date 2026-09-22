# Finite-acceptance dilution of beta asymmetry

↑ **Parent:** [Spin-reversal cross-ratio for beta decay](spin-reversal-cross-ratio-for-beta-decay.md)

A detector collects a range of [solid angles](solid-angle.md), not a single direction. If its nonnegative angular response is $w(\Omega)$, define

$$
G=\int w(\Omega)\,d\Omega,\qquad
k=\frac1G\int w(\Omega)\cos\theta\,d\Omega.
$$

Integrating the [polarized beta-decay angular distribution](polarized-beta-decay-angular-distribution.md) gives a count proportional to $G(1+ak)$. For a uniform forward cone with half-angle $\theta_0$, put $c_0=\cos\theta_0$. Direct integration gives

$$
k=\frac{\int_{c_0}^{1}u\,du}{\int_{c_0}^{1}du}=\frac{1+c_0}{2}.
$$

The opposite cone has mean cosine $-k$. A hemisphere gives $k=1/2$; a narrow cone tends to $k=1$. Hence a [spin-reversal cross-ratio for beta decay](spin-reversal-cross-ratio-for-beta-decay.md) measures $ak$, and an acceptance correction is needed to obtain $a$.

With unequal angular responses, let the two laboratory mean cosines be $k_+$ and $k_-$, including their signs. Then the actual expectation is

$$
R=\frac{(1+ak_+)(1-ak_-)}{(1+ak_-)(1-ak_+)},
$$

which reduces to the simple square only when $k_-=-k_+$. The cancellation of stable multiplicative [detection efficiencies](detection-efficiency.md) survives, but their angular shapes still matter. An [energy](energy-split.md)-integrated response likewise averages $A(E)P\beta(E)\cos\theta$ with the accepted spectrum; a mean speed cannot in general be substituted independently of acceptance.

Additive backgrounds, unequal polarization magnitudes or [detection efficiencies](detection-efficiency.md) that change on reversal do not have the assumed factorization. For example, a reversal-dependent efficiency cross-ratio multiplies $R$ by $\eta_+^{\,+}\eta_-^{\,-}/(\eta_-^{\,+}\eta_+^{\,-})$. [Background subtraction](background-subtraction.md) also creates statistical complications: positive expected signal counts are assumed in this derivation, whereas finite samples with [Poisson distributions](poisson-distribution.md) can contain zero counts. Taking square roots of negative background-subtracted counts is not a valid estimator. These limits explain why reversal and independent preparation checks belong together.

## ↑ Ancestors (9)

1. [Spin-reversal cross-ratio for beta decay](spin-reversal-cross-ratio-for-beta-decay.md)
2. [Polarized beta-decay angular distribution](polarized-beta-decay-angular-distribution.md)
3. [Parity violation](parity-violation.md)
4. [Weak interaction](weak-interaction.md)
5. [Standard Model](standard-model-split.md)
6. [Quantum field theory](quantum-field-theory-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
