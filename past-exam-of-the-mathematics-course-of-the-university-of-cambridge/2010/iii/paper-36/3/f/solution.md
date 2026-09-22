<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For retained [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) draws $\theta^{(1)},\ldots,\theta^{(S)}$, calculate both the parameter average $\widehat m=S^{-1}\sum_s\theta^{(s)}$ and the average deviance $\widehat D_{\mathrm{av}}=S^{-1}\sum_sD(\theta^{(s)})$. Two estimates are

$$
\boxed{\widehat D_{\min,1}=D(\widehat m),\qquad
\widehat D_{\min,2}=\widehat D_{\mathrm{av}}-p.}
$$

The first uses the approximate equality of the [posterior mean](../../../../../../posterior-mean.md) and [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md). The second subtracts the mean $p$ of the [chi-squared distribution](../../../../../../chi-squared-distribution.md) deviance excess. These are different operations: evaluation after averaging versus averaging after evaluation. Both rely on a well-mixed chain and the regular locally flat-prior approximation. The smallest sampled deviance is an upper bound on the true minimum, but merely taking that minimum can be inefficient in high dimension because few draws approach the mode closely.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
