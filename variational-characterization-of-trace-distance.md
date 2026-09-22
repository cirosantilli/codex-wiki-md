# Variational characterization of trace distance

↑ **Parent:** [Trace distance](trace-distance.md)

The [variational characterization of trace distance](variational-characterization-of-trace-distance.md) turns a [matrix](matrix.md) distance into the best possible binary experiment. For [density operators](density-matrix.md) $\rho,\sigma$ on the same [finite-dimensional vector space](finite-dimensional-vector-space.md),

$$
D(\rho,\sigma)=\max_{0\leq P\leq I}\operatorname{Tr}[P(\rho-\sigma)]
=\max_{0\leq P\leq I}|\operatorname{Tr}[P(\rho-\sigma)]|.
$$

An operator $P$ with $0\leq P\leq I$ is an effect of a [POVM](positive-operator-valued-measure.md): both $P$ and $I-P$ are [positive operators](positive-operator.md). The [Born rule](born-rule.md) assigns the first outcome [probabilities](probability.md) $\operatorname{Tr}(P\rho)$ and $\operatorname{Tr}(P\sigma)$. Their signed gap is $\operatorname{Tr}(P\Delta)$, where $\Delta=\rho-\sigma$. Since $\operatorname{Tr}\Delta=0$, replacing $P$ by $I-P$ reverses this gap, explaining the equality with the absolute-value maximum.

One optimal $P$ is the [spectral projector](spectral-projector.md) $P_+$ onto the positive [eigenspaces](eigenspace.md) of $\Delta$. In the [spectral decomposition](spectral-decomposition.md) of $\Delta$, this choice includes all positive [eigenvalues](eigenvalue.md) and excludes all negative [eigenvalues](eigenvalue.md). Their positive sum equals the [trace distance](trace-distance.md) by the [spectral-parts formula for trace distance](spectral-parts-formula-for-trace-distance.md). Any zero [eigenspace](eigenspace.md) can be assigned to either outcome without changing the gap. This is the effect selected by the equal-prior [Holevo–Helstrom theorem](holevo-helstrom-theorem.md). [Watrous, The Theory of Quantum Information, Theorem 3.4, equations (3.16)–(3.19)](https://cs.uwaterloo.ca/~watrous/TQI/TQI.3.pdf)

The same optimum has a classical description. For any finite-outcome [POVM](positive-operator-valued-measure.md) $\{E_i\}$, let $p_i=\operatorname{Tr}(E_i\rho)$ and $q_i=\operatorname{Tr}(E_i\sigma)$. Then

$$
D(\rho,\sigma)=\max_{\{E_i\}}\frac12\sum_i|p_i-q_i|
=\max_{\{E_i\}}\max_A\left|\sum_{i\in A}(p_i-q_i)\right|.
$$

The expression $\frac12\sum_i|p_i-q_i|$ is the [total variation distance](total-variation-distance.md) of the entire outcome [probability distributions](probability-distribution.md); the expression for $A$ is the gap for one event. Grouping outcomes in $A$ gives the single effect $P_A=\sum_{i\in A}E_i$. Conversely, an effect $P$ gives the binary [POVM](positive-operator-valued-measure.md) $\{P,I-P\}$, whose two [probability](probability.md) gaps are opposites, so their [total variation distance](total-variation-distance.md) is $|\operatorname{Tr}(P\Delta)|$. Thus the optimum over all [POVMs](positive-operator-valued-measure.md) is already attained by one binary [projective measurement](projective-measurement.md). [Watrous, The Theory of Quantum Information, §3.1.1, Proposition 3.5 and the discussion following Theorem 3.4](https://cs.uwaterloo.ca/~watrous/TQI/TQI.3.pdf)

For [quantum state discrimination](quantum-state-discrimination.md) with equal prior [probabilities](probability.md), declare $\rho$ on outcome $P$ and $\sigma$ on outcome $I-P$. Directly averaging the two conditional success [probabilities](probability.md) gives

$$
P_{\mathrm{success}}(P)=\frac12\operatorname{Tr}(P\rho)
+\frac12\operatorname{Tr}((I-P)\sigma)
=\frac12\left(1+\operatorname{Tr}(P\Delta)\right).
$$

Optimizing this expression gives $(1+D)/2$. For the diagonal example in [trace distance](trace-distance.md), $P=|0\rangle\langle0|$ gives a gap $0.8-0.3=0.5$. For zero versus plus, that same effect gives only $1-1/2=1/2$, while the effect in [Helstrom measurement for the zero and plus states](helstrom-measurement-for-the-zero-and-plus-states.md) gives the larger gap $1/\sqrt2$. The [trace-distance-preserving binary measurement](trace-distance-preserving-binary-measurement.md) depends on the pair of preparations; a fixed measurement [basis](basis.md) does not generally attain the [trace distance](trace-distance.md) for every pair.

**Table of contents**

- [Trace-distance-preserving binary measurement](trace-distance-preserving-binary-measurement.md)

## ↑ Ancestors (6)

1. [Trace distance](trace-distance.md)
2. [Density matrix](density-matrix.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Helstrom measurement for the zero and plus states](helstrom-measurement-for-the-zero-and-plus-states.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323/4/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323/4/b/i/solution.md)
- [Spectral-parts formula for trace distance](spectral-parts-formula-for-trace-distance.md)
- [Trace distance](trace-distance.md)
- [Trace-distance contraction under quantum channels](trace-distance-contraction-under-quantum-channels.md)
- [Variational characterization of trace distance](variational-characterization-of-trace-distance.md)
