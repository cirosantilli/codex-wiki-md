<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Let $S=\sum_{i=1}^nX_i$. The [likelihood ratio](../../../../../likelihood-ratio.md) of rate two to rate one is $2^n e^{-S}$, which decreases strictly with $S$. By the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md), the **most powerful test rejects for small values of the sum**:

$$
\boxed{\text{reject if }S<c_\alpha,\qquad \mathbb P_{\lambda=1}(S<c_\alpha)=\alpha.}
$$

Under the null, $S$ has the [gamma distribution](../../../../../gamma-distribution.md) with shape $n$ and rate one. Thus $c_\alpha$ is its $\alpha$-quantile, equivalently half the $\alpha$-quantile of the [chi-squared distribution](../../../../../chi-squared-distribution.md) with $2n$ degrees of freedom. The [distribution](../../../../../distribution-mathematical-analysis.md) is continuous, so boundary randomization is unnecessary for $0<\alpha<1$.

For every fixed alternative $\lambda>1$, the [likelihood ratio](../../../../../likelihood-ratio.md) against rate one is $\lambda^n e^{-(\lambda-1)S}$, again strictly decreasing. Therefore the same region is most powerful against every such alternative. Moreover, if $G$ has the shape-$n$, rate-one [gamma distribution](../../../../../gamma-distribution.md), then $S$ at rate $\lambda$ has the same [distribution](../../../../../distribution-mathematical-analysis.md) as $G/\lambda$. It follows that $\mathbb P_\lambda(S<c_\alpha)=\mathbb P(G<\lambda c_\alpha)$ increases with $\lambda$, so the maximum rejection probability over $\lambda\leq1$ is $\alpha$ at one. Any competing size-$\alpha$ test for the composite null is also of level at most $\alpha$ at rate one, and is bounded in power by the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) for each alternative. **The test is uniformly most powerful for the composite hypotheses as well.** This is the [uniformly most powerful test for an exponential rate](../../../../../uniformly-most-powerful-test-for-an-exponential-rate.md) based on the sample sum.

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
