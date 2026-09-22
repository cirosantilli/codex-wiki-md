<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [quantum channel discrimination](../../../../../../quantum-channel-discrimination.md), prepare a [density operator](../../../../../../density-matrix.md) $\rho_{HR}$ on the channel input $H$ and an optional [quantum ancilla](../../../../../../quantum-ancilla.md) $R$. Under hypothesis $j\in\{1,2\}$ the output is

$$
\omega_j=(T_j\otimes\operatorname{id}_R)(\rho_{HR}).
$$

Use a two-outcome [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) $\{Q,I-Q\}$ and decide for $T_1$ on outcome $Q$. The conditional [Type I error](../../../../../../type-i-and-type-ii-errors.md) and [Type II error](../../../../../../type-i-and-type-ii-errors.md) are

$$
\alpha=\operatorname{Tr}[(I-Q)\omega_1],
\qquad
\beta=\operatorname{Tr}[Q\omega_2].
$$

With [prior probabilities](../../../../../../prior-probability.md) $p$ and $1-p$, symmetric Bayesian discrimination minimizes the average error $p\alpha+(1-p)\beta$ over the input and measurement.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
