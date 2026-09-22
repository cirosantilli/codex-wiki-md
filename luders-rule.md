<h1 id="luders-rule">Lüders rule</h1>

↑ **Parent:** [Projective measurement](projective-measurement.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lüders_rule)

The [Lüders rule](luders-rule.md) specifies the ideal [quantum instrument](quantum-instrument.md) for a [projective measurement](projective-measurement.md). Conditional on an outcome with nonzero [probability](probability.md), it gives

$$
\rho_i=\frac{P_i\rho P_i}{\operatorname{Tr}(P_i\rho)},\qquad
|\psi_i\rangle=\frac{P_i|\psi\rangle}{\sqrt{\langle\psi|P_i|\psi\rangle}}
$$

for a [density operator](density-matrix.md) and a [pure state](pure-state.md), respectively. The second formula applies only to a [pure state](pure-state.md) input. If the result is discarded, the output is the [nonselective projective measurement](nonselective-projective-measurement.md) $\sum_iP_i\rho P_i$.

The crucial feature for a degenerate [eigenvalue](eigenvalue.md) is preservation of [quantum coherence](quantum-coherence-in-a-specified-basis.md) within its [eigenspace](eigenspace.md). For a [qutrit](qutrit.md) with [orthonormal basis](orthonormal-basis.md) $|0\rangle,|1\rangle,|2\rangle$, consider

$$
A=0P_0+1P_1,\qquad P_0=|0\rangle\langle0|+|1\rangle\langle1|,\quad P_1=|2\rangle\langle2|.
$$

On $|\chi\rangle=(|0\rangle+|1\rangle)/\sqrt2$, outcome zero has [probability](probability.md) one and the [Lüders rule](luders-rule.md) leaves $|\chi\rangle$ unchanged. Measuring all three rank-one projectors and then forgetting whether the label was zero or one instead gives

$$
\widetilde\rho=\tfrac12|0\rangle\langle0|+\tfrac12|1\rangle\langle1|.
$$

Both procedures always report the coarse value zero, but a subsequent test with projector $|\chi\rangle\langle\chi|$ succeeds with [probability](probability.md) one for the first and one half for the second. Resolving extra information destroyed coherence. This explains why a [quantum nondemolition measurement](quantum-nondemolition-measurement.md) of a degenerate quantity must specify what information the apparatus actually records.

Gerhart Lüders proposed this state-change rule in 1951, explicitly discussing degenerate quantities and distinguishing selected subensembles from the aggregate measured ensemble. Kirkpatrick's translation was first posted in 2004; equations (7) and (8) give the unnormalized selective update and the nonselective update. [Lüders, 1951, translated by Kirkpatrick, 2004](https://arxiv.org/abs/quant-ph/0403007).

Repeatability follows briefly from $P_jP_i=\delta_{ij}P_i$: after outcome $i$, $\operatorname{Tr}(P_j\rho_i)=\delta_{ij}$. This assumes a second application of the same ideal instrument without intervening dynamics. An instrument with the same effects can rotate or reset the output and need not satisfy this conclusion; see [POVM does not determine the post-measurement state](povm-does-not-determine-the-post-measurement-state.md).

**Table of contents**

- [Post-measurement state](post-measurement-state.md)
- [Nonselective projective measurement](nonselective-projective-measurement.md)
  - [Pinching map](pinching-map.md)
  - [Rank-one dephasing](rank-one-dephasing.md)
    - [Relative-entropy identity for rank-one dephasing](relative-entropy-identity-for-rank-one-dephasing.md)
    - [Support inclusion under rank-one dephasing](support-inclusion-under-rank-one-dephasing.md)

## ↑ Ancestors (6)

1. [Projective measurement](projective-measurement.md)
2. [Measurement in quantum mechanics](quantum-measurement-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Aharonov-Bergmann-Lebowitz rule](aharonov-bergmann-lebowitz-rule.md)
- [Born rule](born-rule.md)
- [Context dependence of pre- and post-selected measurements](context-dependence-of-pre-and-post-selected-measurements.md)
- [Estimating a quantum expectation value](estimating-a-quantum-expectation-value.md)
- [Lüders rule](luders-rule.md)
- [Measurement backaction](measurement-backaction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57/3/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325/1/solution.md)
- [Post-measurement state](post-measurement-state.md)
- [Projective measurement](projective-measurement.md)
- [Quantum nondemolition measurement](quantum-nondemolition-measurement.md)
- [Singlet-triplet measurement causality obstruction](singlet-triplet-measurement-causality-obstruction.md)
