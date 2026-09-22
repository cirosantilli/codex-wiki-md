<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

Put $S_1=\sum_{i=1}^nX_i$, $S_2=\sum_{i=1}^nX_i^2$. The joint [normal distribution](../../../../../normal-distribution.md) density can be written as

$$
p_\mu(\boldsymbol x)=(2\pi)^{-n/2}e^{-n/2}\mu^{-n}\exp\left(-\frac{S_2}{2\mu^2}+\frac{S_1}{\mu}\right).
$$

The [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md) says that, for a family dominated by a common measure, a statistic $T$ is a [sufficient statistic](../../../../../sufficient-statistic.md) when its densities have the form $g_\mu(T(\boldsymbol x))h(\boldsymbol x)$ with $h$ independent of the parameter. The displayed factorization therefore shows that **$(S_1,S_2)$ is a two-dimensional [sufficient statistic](../../../../../sufficient-statistic.md)**.

For [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md), discard parameter-independent terms from the [log-likelihood](../../../../../log-likelihood.md):

$$
\ell(\mu)=-n\log\mu-\frac{S_2}{2\mu^2}+\frac{S_1}{\mu},\qquad
\ell'(\mu)=\frac{S_2-S_1\mu-n\mu^2}{\mu^3}.
$$

If $S_2>0$, the quadratic equation has exactly one positive root. The numerator is positive before that root and negative after it, while the [likelihood](../../../../../likelihood-function.md) tends to zero at both ends of $\mu>0$. Hence the [normal likelihood with variance equal to squared mean](../../../../../normal-likelihood-with-variance-equal-to-squared-mean.md) gives the global maximizer

$$
\boxed{\widehat\mu=\frac{\sqrt{S_1^2+4nS_2}-S_1}{2n}}.
$$

This holds almost surely. The exceptional all-zero sample has $S_2=0$ and [likelihood](../../../../../likelihood-function.md) proportional to $\mu^{-n}$, so its supremum is approached as $\mu\downarrow0$ and there is no positive maximizer.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
