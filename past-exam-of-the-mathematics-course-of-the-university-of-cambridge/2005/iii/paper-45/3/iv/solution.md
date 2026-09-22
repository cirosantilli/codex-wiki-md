<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the joint [prior](../../../../../../prior-probability.md) density $g(\theta,t)=\pi(\theta)q(t)$ as the proposal for [rejection sampling](../../../../../../rejection-sampling.md). Since the Poisson [probability](../../../../../../probability.md) $a_k(\theta,t)$ lies in $[0,1]$, the following algorithm is valid:

- Draw $\theta$ from the proper [prior distribution](../../../../../../prior-probability.md) $\pi$.
- Independently draw $T_j$ from the [exponential distributions](../../../../../../exponential-distribution.md) with rates $\binom j2$, for $j=2,\ldots,n$, and calculate $L=\sum jT_j$.
- Draw $U$ uniformly on $[0,1]$, independently of all previous draws. Retain $(\theta,T)$ if $U\le e^{-\theta L/2}(\theta L/2)^k/k!$; otherwise restart.

The joint density of a proposed pair together with its acceptance event is $g(\theta,t)a_k(\theta,t)$. Its integral is $m_k$, so conditioning on acceptance gives precisely $g a_k/m_k$, the desired [posterior density](../../../../../../posterior-density.md). Repeating independent proposal trials until each acceptance produces independent [posterior](../../../../../../bayesian-posterior.md) observations. This is [Bayesian rejection sampling for a segregating-site count](../../../../../../bayesian-rejection-sampling-for-a-segregating-site-count.md).

An equivalent implementation simulates $S^*\sim\operatorname{Poisson}(\theta L/2)$ and accepts exactly when $S^*=k$. Its acceptance [probability](../../../../../../probability.md) is the same Poisson mass. **Propose from the joint [prior](../../../../../../prior-probability.md) and accept according to the exact observed-count [likelihood](../../../../../../likelihood-function.md).** No approximation to the [posterior distribution](../../../../../../bayesian-posterior.md) is involved in the accepted draws.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
