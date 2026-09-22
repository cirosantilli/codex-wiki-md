# Measurement backaction

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement-split.md)

Measurement backaction is the effect of a [measurement in quantum mechanics](quantum-measurement-split.md) on later predictions for the measured system. A [quantum instrument](quantum-instrument.md) with one [Kraus operator](kraus-operator.md) $K_m$ per recorded outcome has

$$
p_m=\operatorname{Tr}(K_m\rho K_m^\dagger),\qquad
\rho_m=\frac{K_m\rho K_m^\dagger}{p_m},\qquad
\sum_m K_m^\dagger K_m=I.
$$

The conditional [density operator](density-matrix.md) $\rho_m$ exists only when $p_m>0$. Its nonlinear normalization expresses conditioning; the unnormalized map $\rho\mapsto K_m\rho K_m^\dagger$ is linear. More generally, an unresolved outcome can contain several [Kraus operators](kraus-operator.md): replace the numerator by $\sum_a K_{ma}\rho K_{ma}^\dagger$ and take its [trace](matrix-trace.md) for $p_m$. [Watrous, The Theory of Quantum Information, §2.3.2](https://cs.uwaterloo.ca/~watrous/TQI/TQI.pdf).

Keeping the outcome gives a [selective quantum measurement](selective-quantum-measurement.md). Discarding it gives a [nonselective quantum measurement](nonselective-quantum-measurement.md) with [quantum channel](quantum-channel.md) $\rho\mapsto\sum_m p_m\rho_m$. The latter describes the whole measured population without its labels, whereas each $\rho_m$ describes a selected subpopulation. Neither description requires the measured quantity to have possessed its eventual value before the interaction.

For a concrete test, prepare the [Pauli X eigenstate](pauli-x-eigenstate.md) $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$. Its $X=+1$ [probability](probability.md) is one. An ideal $Z$ [projective measurement](projective-measurement.md) gives zero or one with equal [probability](probability.md), leaving $|0\rangle$ or $|1\rangle$ under the [Lüders rule](luders-rule.md). Discarding the result leaves the [maximally mixed state](maximally-mixed-state.md) $I/2$. A subsequent $X$ measurement now gives either sign with [probability](probability.md) one half, even if the $Z$ result was kept. This observable change in statistics is backaction. Measuring $X$ on the original $|+\rangle$ instead leaves it unchanged: disturbance depends on both the preparation and the instrument. [Measurement-based quantum feedback](measurement-based-quantum-feedback.md) uses the recorded outcome to choose a subsequent control operation, so both parts of the instrument matter.

## ↑ Ancestors (5)

1. [Measurement in quantum mechanics](quantum-measurement-split.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/a/solution.md)
