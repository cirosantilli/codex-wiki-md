<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $t=(t_2,\ldots,t_n)$, with all $t_j>0$, and put $L(t)=\sum_{j=2}^n jt_j$. The independent exponential epoch times have joint density

$$
q(t)=\prod_{j=2}^n\lambda_j e^{-\lambda_jt_j},\qquad \lambda_j=\binom j2.
$$

Take a proper [prior distribution](../../../../../../prior-probability.md) density $\pi(\theta)$ on $\theta\ge0$, independent of the neutral genealogy. [Independence](../../../../../../independent-random-variables.md) is appropriate because the specified neutral [Kingman's coalescent](../../../../../../kingman-s-coalescent.md) does not depend on the [mutation](../../../../../../mutation.md) parameter. The conditional observed-count [likelihood function](../../../../../../likelihood-function.md) is

$$
a_k(\theta,t)=P(S=k\mid\theta,t)=\frac{e^{-\theta L(t)/2}[\theta L(t)/2]^k}{k!}.
$$

Its [prior](../../../../../../prior-probability.md) predictive [probability](../../../../../../probability.md), or [Bayesian model evidence](../../../../../../bayesian-model-evidence.md), is

$$
m_k=\int_0^\infty\!\int_{(0,\infty)^{n-1}}\pi(\theta)q(t)a_k(\theta,t)\,dt\,d\theta.
$$

Assuming $m_k>0$, [Bayes' theorem](../../../../../../bayes-theorem.md) gives the [joint posterior of mutation rate and coalescent times](../../../../../../joint-posterior-of-mutation-rate-and-coalescent-times.md):

$$
\boxed{f(\theta,t\mid S=k)=\frac{\pi(\theta)}{m_k k!}\prod_{j=2}^n\lambda_j e^{-\lambda_jt_j}\,e^{-\theta L(t)/2}\left[\frac{\theta L(t)}2\right]^k.}
$$

It is zero outside the [prior](../../../../../../prior-probability.md) support and positive-time region. For $k=0$, use the usual convention $0^0=1$ in the Poisson mass. An improper [prior](../../../../../../prior-probability.md) cannot be sampled as the proposal in the following algorithm, even in cases where its formal [posterior](../../../../../../bayesian-posterior.md) can be normalized.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
