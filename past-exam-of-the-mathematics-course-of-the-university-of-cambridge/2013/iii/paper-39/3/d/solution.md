<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $H$ replicate $\xi_1$, so $\xi_1=H^TP_1$. The positive-definite [Gram matrix](../../../../../../gram-matrix.md) $Q=\mathbb E[P_1P_1^T]$ is invertible. Multiplication by $P_1$ and taking [expected values](../../../../../../expected-value.md) give

$$
\mathbb E[P_1\xi_1]=QH,\qquad
H=Q^{-1}\mathbb E[P_1\xi_1].
$$

All quantities are integrable: the finite-atom representation from completeness gives finite terminal values, and the matrix $Q$ has finite entries. Positive definiteness also guarantees uniqueness of holdings, since $h^TP_1=0$ would imply $h^TQh=0$ and hence $h=0$.

Thus the replication cost is

$$
H^TP_0=P_0^TQ^{-1}\mathbb E[P_1\xi_1]
=\mathbb E[(P_0^TQ^{-1}P_1)\xi_1].
$$

Consequently the [one-period Gram-matrix replication formula](../../../../../../one-period-gram-matrix-replication-formula.md) is

$$
\boxed{\xi_0=\mathbb E[Z\xi_1],\qquad Z=P_0^TQ^{-1}P_1,\qquad W=Q^{-1}P_1,\quad H=\mathbb E[W\xi_1].}
$$

The symmetry of $Q^{-1}$ makes the displayed orientations consistent. Positivity of this $Z$ would require an additional no-arbitrage condition; positive definiteness of the payoff [Gram matrix](../../../../../../gram-matrix.md) alone proves the representation and uniqueness, not positivity of prices across states.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
