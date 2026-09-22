<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

There are two distinct parts of the [hierarchy problem](../../../../../hierarchy-problem.md). The first asks why the scale of [electroweak symmetry breaking](../../../../../electroweak-symmetry-breaking.md) is so much smaller than a fundamental scale such as the [Planck mass](../../../../../planck-mass.md). The second, the [technical hierarchy problem](../../../../../technical-hierarchy-problem.md), asks why that separation survives quantum corrections once it is chosen. With a fundamental [Higgs boson](../../../../../higgs-boson.md), a mass term $m_H^2H^\dagger H$ is allowed by the ordinary [gauge symmetry](../../../../../gauge-invariance.md), so heavy thresholds can contribute additive terms of order a heavy mass squared. This is different from the [chiral protection of a fermion mass](../../../../../chiral-protection-of-a-fermion-mass.md) and the [gauge protection of a vector mass](../../../../../gauge-protection-of-a-vector-mass.md).

For example, a cutoff description of the [Standard Model](../../../../../standard-model-split.md) gives the schematic one-loop sensitivity

$$
\delta m_H^2\simeq\frac{\Lambda^2}{16\pi^2}\left(6\lambda_H+\frac94g^2+\frac34g'^2-6y_t^2\right).
$$

The regulator-dependent quadratic term is not itself an observable, but a physical heavy particle of mass $M$ coupled to the Higgs likewise produces a matching correction of order coupling squared times $M^2/(16\pi^2)$. Maintaining $|m_H^2|\ll M^2$ then generically requires cancellation between large unrelated terms. This is the [naturalness](../../../../../naturalness-physics.md) concern; changing the regulator does not eliminate the heavy-threshold issue.

Exact [supersymmetry](../../../../../supersymmetry-split.md) relates bosonic and fermionic couplings and masses. Their loop contributions have opposite signs, and the relations enforce [supersymmetric cancellation of quadratic divergences](../../../../../supersymmetric-cancellation-of-quadratic-divergences.md). [Boson-fermion degeneracy in a supermultiplet](../../../../../boson-fermion-degeneracy-in-a-supermultiplet.md) also transfers fermionic mass protection to its scalar partners. It is not sufficient merely to add arbitrary scalars: the supersymmetric coupling relations are what make the cancellation persist. Perturbative [superpotential non-renormalization](../../../../../non-renormalization-theorem.md) further protects holomorphic mass parameters, although [wave-function renormalization](../../../../../wave-function-renormalization.md) still makes canonically normalized couplings run.

For a realistic separation between ordinary particles and their partners, [supersymmetry](../../../../../supersymmetry-split.md) must be broken. [Soft supersymmetry breaking](../../../../../soft-supersymmetry-breaking.md) introduces masses and selected positive-mass-dimension interactions without reinstating the original ultraviolet quadratic divergence. A paired propagator difference behaves at high Euclidean momentum as

$$
\frac1{k^2+m_B^2}-\frac1{k^2+m_F^2}=\frac{m_F^2-m_B^2}{k^4}+O(k^{-6}),
$$

so a residual scalar correction is of the order

$$
\boxed{\delta m_H^2\sim\frac{|y|^2}{16\pi^2}m_{\rm soft}^2\log\frac{\Lambda}{m_{\rm soft}},\qquad\text{rather than order }\Lambda^2.}
$$

This [soft scalar-mass sensitivity](../../../../../soft-scalar-mass-sensitivity.md) controls the technical problem if the relevant soft masses and thresholds are not too far above the weak scale. Very heavy partners can still require tuning through finite and logarithmic terms. Supersymmetric cancellations alone therefore do not guarantee a naturally small weak scale for an arbitrary broken spectrum.

The origin of the hierarchy needs further dynamics. In [dynamical supersymmetry breaking](../../../../../dynamical-supersymmetry-breaking.md), an asymptotically free [hidden supersymmetry-breaking sector](../../../../../hidden-supersymmetry-breaking-sector.md) can generate an exponentially smaller scale by [dimensional transmutation](../../../../../dimensional-transmutation.md),

$$
\Lambda_{
m hid}=M\exp\left[-\frac{8\pi^2}{b_0g^2(M)}\right],\qquad b_0>0.
$$

If that sector actually has no supersymmetric vacuum, its breaking can be communicated to the visible sector to produce small soft terms. The exponential creates a hierarchy without specifying a tiny dimensionless coupling at the high scale, but the existence of breaking and its mediation are additional model-building requirements. In the [MSSM](../../../../../minimal-supersymmetric-standard-model.md), running Higgs soft masses can trigger [electroweak symmetry breaking](../../../../../electroweak-symmetry-breaking.md). The [supersymmetric mu problem](../../../../../supersymmetric-mu-problem.md) remains: the allowed superpotential mass $\mu H_uH_d$ must also be near the soft scale, and non-renormalization protects a chosen small $\mu$ without explaining its origin.

Extra-dimensional proposals use geometry to explain why observable gravitational and weak scales differ. In [large extra dimensions](../../../../../large-extra-dimensions.md), assume gravity propagates in $4+n$ dimensions with fundamental scale $M_*$, while ordinary fields are localized on a [brane](../../../../../brane.md). Integrating the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) over compact volume $V_n$ gives the [Planck mass from compactification volume](../../../../../planck-mass-from-compactification-volume.md) relation

$$
\boxed{M_{\rm Pl}^2=M_*^{n+2}V_n.}
$$

Here $M_{\rm Pl}$ denotes the four-dimensional [reduced Planck mass](../../../../../reduced-planck-mass.md). A sufficiently large internal volume lets $M_*$ be near the weak scale even though $M_{\rm Pl}$ is enormous. The Higgs need then be stable only up to the lower fundamental cutoff. This explains the weakness of long-distance gravity geometrically but trades the scale question for the origin and stabilization of a large compact volume. Ordinary matter is localized to avoid an unwanted low-mass tower of its own [Kaluza-Klein modes](../../../../../kaluza-klein-mode.md); gravitational modes, departures from four-dimensional gravity and bulk energy loss impose phenomenological requirements.

The [Randall–Sundrum model](../../../../../randall-sundrum-model.md) instead uses a warped five-dimensional interval, conventionally the doubled $S^1/\mathbb Z_2$ orbifold with fixed branes at $0$ and $L$:

$$
ds^2=e^{-2k|y|}\eta_{\mu\nu}dx^\mu dx^\nu+dy^2,\qquad M_{\rm Pl}^2=\frac{M_5^3}{k}(1-e^{-2kL}).
$$

For a scalar confined to the distant brane, the kinetic and mass terms carry factors $e^{-2kL}$ and $e^{-4kL}$. Canonical rescaling therefore produces

$$
\boxed{m_{\rm IR}=e^{-kL}m_0.}
$$

A moderately large $kL$ yields an exponentially small observable mass without a comparably large compact-volume factor. The inter-brane size is the [radion](../../../../../radion.md), so one still needs a mechanism fixing its expectation value. Consistent curvature, brane tensions and ultraviolet physics are also part of the model. Warping is a redshift mechanism; it does not provide the same cancellation of arbitrary scalar loops as supersymmetry.

Finally, protecting a Higgs mass is not the same as solving the vacuum-energy hierarchy. Exact global [supersymmetry](../../../../../supersymmetry-split.md) has zero-energy supersymmetric vacua, but broken supersymmetry generically leaves vacuum energy set by its breaking dynamics. In [supergravity](../../../../../supergravity.md), positive auxiliary-field contributions coexist with a negative superpotential term, and obtaining a very small cosmological constant requires further structure or cancellation. Neither soft supersymmetry nor the two geometric mechanisms automatically resolves that problem. The mechanisms can also coexist in one higher-dimensional supersymmetric theory.

**Supersymmetry protects a chosen hierarchy radiatively and can accompany dynamics generating a small scale; extra-dimensional volume or warping generates the scale separation geometrically, with stabilization still required.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
