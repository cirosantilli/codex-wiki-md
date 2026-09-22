<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

A [Bayes estimator](../../../../../bayes-estimator.md) minimizes the integrated [loss function](../../../../../loss-function.md) under the prior and sampling distribution. For a nonnegative loss, [Tonelli's theorem](../../../../../tonelli-theorem.md) and the [posterior distribution](../../../../../bayesian-posterior.md) give the risk decomposition

$$
\int\!\int L(\theta,\delta(x))f(x\mid\theta)\pi(\theta)dxd\theta
=\int m(x)\left[\int L(\theta,\delta(x))\pi(\theta\mid x)d\theta\right]dx,
$$

where $m$ is the marginal density. Thus choosing, for each observed $x$, a measurable minimizer of the [posterior expected loss](../../../../../posterior-expected-loss.md) minimizes the integrated risk. Observations of marginal probability zero do not affect the rule.

Here the likelihood is $\theta e^{-\theta x}$ and the prior is $\mu e^{-\mu\theta}$ on positive parameters. Put $b=\mu+x$. Their product is $\mu\theta e^{-b\theta}$, and $\int_0^\infty\theta e^{-b\theta}d\theta=b^{-2}$. The marginal density and posterior are therefore

$$
m(x)=\frac{\mu}{(\mu+x)^2},\qquad
\boxed{\pi(\theta\mid x)=b^2\theta e^{-b\theta},\quad\theta>0.}
$$

This [Gamma-exponential conjugacy](../../../../../gamma-exponential-conjugacy.md) calculation gives a [Gamma distribution](../../../../../gamma-distribution.md) with shape $2$ and rate $b$. It is the posterior, rather than the prior alone, which determines both requested estimators.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
