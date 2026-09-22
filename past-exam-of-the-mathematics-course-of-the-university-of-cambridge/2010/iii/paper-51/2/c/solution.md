<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes: distinct density operators have a projective measurement with different outcome probabilities.** Let $\rho,\sigma$ be the two [density operators](../../../../../../density-matrix.md) and let $D=\rho-\sigma$. It is a nonzero [Hermitian operator](../../../../../../hermitian-operator.md) with trace zero. Its nonzero eigenvalues cannot all have the same sign, since their sum is zero. Let $P_+$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto its positive-eigenvalue subspace. Then the two-outcome [projective measurement](../../../../../../projective-measurement.md) $\{P_+,I-P_+\}$ satisfies

$$
P_\rho(+)-P_\sigma(+)=\operatorname{Tr}[P_+(\rho-\sigma)]
=\sum_{\lambda_j(D)>0}\lambda_j(D)>0.
$$

The outcome therefore carries statistical information about which [quantum ensemble](../../../../../../quantum-state-ensemble.md) was used.

For example, with equal prior probabilities, guess $\rho$ after $+$ and $\sigma$ after the other outcome. The success probability is

$$
P_{\rm succ}=\frac12\operatorname{Tr}(P_+\rho)+\frac12\operatorname{Tr}[(I-P_+)\sigma]
=\frac12+\frac12\operatorname{Tr}(P_+D).
$$

Since the positive and negative eigenvalue sums of $D$ have equal absolute value, $\operatorname{Tr}(P_+D)=\|D\|_1/2$. Consequently

$$
\boxed{P_{\rm succ}=\frac12+\frac14\|\rho-\sigma\|_1>\frac12.}
$$

This is the equal-prior measurement in the [Holevo–Helstrom theorem](../../../../../../holevo-helstrom-theorem.md), expressed using the [trace distance](../../../../../../trace-distance.md). The conclusion is some information, not necessarily perfect one-shot discrimination: nonorthogonal density operators generally cannot be distinguished with certainty.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
