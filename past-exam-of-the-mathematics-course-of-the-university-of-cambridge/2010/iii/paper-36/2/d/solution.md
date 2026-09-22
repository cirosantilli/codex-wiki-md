<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under independent area counts and independent area [prior distributions](../../../../../../prior-probability.md), the joint [posterior distribution](../../../../../../bayesian-posterior.md) factors into the gamma posteriors. For each simulation $s=1,\ldots,S$, draw one joint vector by independently generating

$$
\lambda_i^{(s)}\sim\operatorname{Gamma}(y_i+1/2,E_i),\qquad i=1,\ldots,I.
$$

Rank the risks within that joint draw, taking rank one to mean highest risk:

$$
r_i^{(s)}=1+\sum_{k\ne i}\mathbf1\{\lambda_k^{(s)}>\lambda_i^{(s)}\}.
$$

The empirical [posterior rank distribution](../../../../../../posterior-rank-distribution.md) and highest-risk probability are

$$
\boxed{\widehat{\mathbb P}(r_i=k\mid y)=\frac1S\sum_{s=1}^S\mathbf1\{r_i^{(s)}=k\},\qquad
\widehat{\mathbb P}(i\text{ highest}\mid y)=\frac1S\sum_{s=1}^S\mathbf1\{r_i^{(s)}=1\}.}
$$

Independent gamma draws make this direct [Monte Carlo integration](../../../../../../monte-carlo-integration.md), so [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) is unnecessary here. Continuous posteriors give ties probability zero, and the highest-risk probabilities sum to one. The same ranking calculation can be applied to dependent joint draws from a richer [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md); ranking separate posterior means would discard the uncertainty that the program is intended to measure.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
