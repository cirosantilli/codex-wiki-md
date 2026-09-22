<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiplying the [likelihood function](../../../../../../likelihood-function.md) by the [Pareto distribution](../../../../../../pareto-distribution.md) prior gives

$$
p(\theta\mid\mathbf y)\propto
\theta^{-(\alpha+n)-1}\mathbf1_{\{\theta>m\}},
\qquad m=\max(\beta,M).
$$

The integral of this kernel is $m^{-(\alpha+n)}/(\alpha+n)$, so the normalized [posterior distribution](../../../../../../bayesian-posterior.md) is

$$
\boxed{p(\theta\mid\mathbf y)
=(\alpha+n)m^{\alpha+n}\theta^{-(\alpha+n)-1}
\mathbf1_{\{\theta>m\}}.}
$$

Thus it is $\operatorname{Pareto}(\alpha+n,m)$. This proves [uniform-Pareto conjugacy](../../../../../../uniform-pareto-conjugacy.md): applying [Bayes' theorem](../../../../../../bayes-theorem.md) preserves the family of [prior distributions](../../../../../../prior-probability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
