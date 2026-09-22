# Trace distance

↑ **Parent:** [Density matrix](density-matrix-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trace_distance)

How different can two preparations look to someone who can perform any [measurement in quantum mechanics](quantum-measurement-split.md)? The [trace distance](trace-distance.md) answers this question for [density operators](density-matrix-split.md) $\rho,\sigma$ on the same [finite-dimensional vector space](finite-dimensional-vector-space.md):

$$
D(\rho,\sigma)=\frac12\lVert\rho-\sigma\rVert_1
=\frac12\operatorname{Tr}|\rho-\sigma|,\qquad
|A|=\sqrt{A^\dagger A}.
$$

Here $|A|$ is the [absolute value of an operator](absolute-value-of-an-operator.md), and $\lVert A\rVert_1$ is its [trace norm](trace-norm.md). Because $\Delta=\rho-\sigma$ is [Hermitian](hermitian-operator.md), its [trace norm](trace-norm.md) is the sum of the absolute values of its [eigenvalues](eigenvalue.md); it is not the sum of the absolute values of its [matrix](matrix.md) entries. The factor $1/2$ gives

$$
0\leq D(\rho,\sigma)\leq1.
$$

The [trace distance](trace-distance.md) is a [metric](metric.md): it is symmetric, vanishes exactly when $\rho=\sigma$, and obeys the [triangle inequality](triangle-inequality.md). Identical preparations have [trace distance](trace-distance.md) zero; preparations with orthogonal occupied [eigenspaces](eigenspace.md) have [trace distance](trace-distance.md) one and can be identified perfectly in a single [measurement in quantum mechanics](quantum-measurement-split.md).

Operationally, the [trace distance](trace-distance.md) is the largest [total variation distance](total-variation-distance.md) between the outcome [probability distributions](probability-distribution-split.md) obtainable by a [POVM](positive-operator-valued-measure.md). Equivalently, the [variational characterization of trace distance](variational-characterization-of-trace-distance.md) says it is the largest possible [probability](probability.md) gap for one event in a binary [measurement in quantum mechanics](quantum-measurement-split.md). For one copy of either known preparation, each chosen with prior [probability](probability.md) $1/2$, the [Holevo–Helstrom theorem](holevo-helstrom-theorem.md) gives

$$
P_{\mathrm{success}}^{\mathrm{opt}}=\frac{1+D(\rho,\sigma)}2.
$$

Thus [trace distance](trace-distance.md) zero leaves only guessing, while [trace distance](trace-distance.md) one permits perfect [quantum state discrimination](quantum-state-discrimination.md). The optimum ranges over measurements; different measurement [bases](basis.md) can expose different amounts of distinguishability. [Watrous, The Theory of Quantum Information, §3.1, Theorem 3.4 and Proposition 3.5](https://cs.uwaterloo.ca/~watrous/TQI/TQI.3.pdf)

For a worked example with commuting [density operators](density-matrix-split.md), take a [qubit](qubit.md) with

$$
\rho=\begin{pmatrix}0.8&0\\0&0.2\end{pmatrix},\qquad
\sigma=\begin{pmatrix}0.3&0\\0&0.7\end{pmatrix}.
$$

Their difference has [eigenvalues](eigenvalue.md) $0.5,-0.5$, so $D=(|0.5|+|-0.5|)/2=0.5$. Measuring in the [computational basis](computational-basis.md) produces outcome [probability distributions](probability-distribution-split.md) $(0.8,0.2)$ and $(0.3,0.7)$, whose [total variation distance](total-variation-distance.md) is also $0.5$. Guessing $\rho$ on outcome zero and $\sigma$ on outcome one succeeds with [probability](probability.md) $(0.8+0.7)/2=0.75$. A [projective measurement](projective-measurement.md) in the [Hadamard basis](hadamard-basis.md) instead produces $(0.5,0.5)$ for both preparations and gives no discrimination advantage.

The [trace-distance contraction under quantum channels](trace-distance-contraction-under-quantum-channels.md) ensures that a common [quantum channel](quantum-channel.md), including the [partial trace](partial-trace.md), cannot increase the [trace distance](trace-distance.md). This makes [trace distance](trace-distance.md) a useful error measure: if $D\leq\epsilon$, every event in every [measurement in quantum mechanics](quantum-measurement-split.md) has a [probability](probability.md) gap at most $\epsilon$. Losing access to a subsystem can hide distinguishability, but cannot create more of it.

**Table of contents**

- [Trace distance between qubit states](trace-distance-between-qubit-states.md)
- [Trace-distance contraction under quantum channels](trace-distance-contraction-under-quantum-channels.md)
- [Trace distance for qubit dephasing](trace-distance-for-qubit-dephasing.md)
- [Pure-target upper bound on trace distance](pure-target-upper-bound-on-trace-distance.md)
- [Spectral-parts formula for trace distance](spectral-parts-formula-for-trace-distance.md)
- [Pure-target lower bound on trace distance](pure-target-lower-bound-on-trace-distance.md)
- [Variational characterization of trace distance](variational-characterization-of-trace-distance.md)
  - [Trace-distance-preserving binary measurement](trace-distance-preserving-binary-measurement.md)

## ↑ Ancestors (5)

1. [Density matrix](density-matrix-split.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (36)

- [Asymptotic pure-state entanglement conversion rate](asymptotic-pure-state-entanglement-conversion-rate.md)
- [Copy-number trace-distance obstruction](copy-number-trace-distance-obstruction.md)
- [Entropy of a binary diagonal qubit mixture](entropy-of-a-binary-diagonal-qubit-mixture.md)
- [Fidelity of commuting mixed states](fidelity-of-commuting-mixed-states.md)
- [Fidelity of quantum states](fidelity-of-quantum-states.md)
- [Fuchs-van de Graaf inequalities](fuchs-van-de-graaf-inequalities.md)
- [Helstrom measurement for the zero and plus states](helstrom-measurement-for-the-zero-and-plus-states.md)
- [Lower asymptotic semicontinuity of quantum relative entropy](lower-asymptotic-semicontinuity-of-quantum-relative-entropy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/3/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-59/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/3/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323/4/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-323/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-323/4/iii/solution.md)
- [Pure-state trace distance and fidelity identity](pure-state-trace-distance-and-fidelity-identity.md)
- [Pure-target upper bound on trace distance](pure-target-upper-bound-on-trace-distance.md)
- [Quantum Pinsker inequality](quantum-pinsker-inequality.md)
- [Qubit fidelity along a Bloch meridian](qubit-fidelity-along-a-bloch-meridian.md)
- [Spectral-parts formula for trace distance](spectral-parts-formula-for-trace-distance.md)
- [Trace distance](trace-distance.md)
- [Trace distance between qubit states](trace-distance-between-qubit-states.md)
- [Trace distance for qubit dephasing](trace-distance-for-qubit-dephasing.md)
- [Trace-distance-preserving binary measurement](trace-distance-preserving-binary-measurement.md)
- [Unitary invariance of trace distance and fidelity](unitary-invariance-of-trace-distance-and-fidelity.md)
- [Variational characterization of trace distance](variational-characterization-of-trace-distance.md)
