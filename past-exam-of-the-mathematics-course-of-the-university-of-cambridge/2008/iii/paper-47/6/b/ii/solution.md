<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Within the merged third observed cell, the probability of belonging to the original fourth cell is

$$
\frac{p_4}{p_3+p_4}=\frac{1/2}{\theta^{(t)}/4+1/2}=\frac{2}{2+\theta^{(t)}}.
$$

The allocation therefore has the conditional [binomial distribution](../../../../../../../binomial-distribution.md)

$$
Z\mid x,\theta^{(t)}\sim\operatorname{Bin}\left(x_3,\frac{2}{2+\theta^{(t)}}\right).
$$

Its conditional [expectation](../../../../../../../expected-value.md) and the filled-in missing counts are

$$
\boxed{z^{(t)}=\frac{2x_3}{2+\theta^{(t)}},\qquad
y_3^{(t)}=\frac{x_3\theta^{(t)}}{2+\theta^{(t)}},\qquad
y_4^{(t)}=z^{(t)},}
$$

with $y_1^{(t)}=x_1$ and $y_2^{(t)}=x_2$.

Taking the conditional [expectation](../../../../../../../expected-value.md) of the complete [log-likelihood](../../../../../../../log-likelihood.md) gives the [EM for merged multinomial cells](../../../../../../../em-for-merged-multinomial-cells.md) E-step:

$$
\boxed{Q(\theta\mid\theta^{(t)})=x_1\log(1-\theta)
 +(x_2+y_3^{(t)})\log\theta+C_t.}
$$

This is the parameter-dependent part of $\log L(y^{(t)}\mid\theta)$. More precisely, $Q(\theta\mid\theta^{(t)})=\log L(y^{(t)}\mid\theta)+C'_t$, where the constant is independent of the candidate $\theta$, interpreting factorials of noninteger filled counts through the [gamma function](../../../../../../../gamma-function.md). The expected log-factorials are not generally the log-factorials of expected counts, so literal equality including the normalization would be false. Equality up to this constant is exactly what the M-step needs. Filling in conditional means works here because the candidate-parameter terms are linear in the missing counts; it is not a universal rule for the [expectation-maximization algorithm](../../../../../../../expectation-maximization-algorithm.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
