<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $S_n=\sum_{i=1}^nX_i$. The [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell_n(\theta)=n\log\theta-\theta S_n,
$$

with [score function](../../../../../../informant-function.md) $n/\theta-S_n$ and second derivative $-n/\theta^2<0$. The unique [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is therefore

$$
\boxed{\widehat\theta_{\rm MLE}=\frac n{S_n}=\frac1{\overline X}.}
$$

For an [exponential distribution](../../../../../../exponential-distribution.md) of rate $\theta$,

$$
\mathbb E[X_i]=\frac1\theta,
\qquad
\operatorname{var}(X_i)=\frac1{\theta^2}.
$$

The [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\sqrt n\left(\overline X-\frac1\theta\right)
\xrightarrow dN\left(0,\frac1{\theta^2}\right).
$$

Applying the [delta method](../../../../../../delta-method.md) to $h(x)=1/x$, for which $h'(1/\theta)=-\theta^2$, yields the [exponential-rate maximum-likelihood estimator](../../../../../../exponential-rate-maximum-likelihood-estimator.md) limit

$$
\boxed{
\sqrt n(\widehat\theta_{\rm MLE}-\theta)
\xrightarrow dN(0,\theta^2).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
