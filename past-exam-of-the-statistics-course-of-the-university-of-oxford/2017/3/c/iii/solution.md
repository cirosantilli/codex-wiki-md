<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For one [Bernoulli random variable](../../../../../bernoulli-distribution.md),

$$
\log f(x\mid\theta)=x\log\theta+(1-x)\log(1-\theta),\qquad
\partial_\theta\log f(x\mid\theta)=\frac{x-\theta}{\theta(1-\theta)}.
$$

Its [variance](../../../../../variance-split.md) is $\theta(1-\theta)$, so the expected [Fisher information](../../../../../fisher-information-matrix.md) and [Jeffreys prior](../../../../../jeffreys-prior.md) are

$$
I(\theta)=\frac1{\theta(1-\theta)},\qquad
\pi_J(\theta)\propto\theta^{-1/2}(1-\theta)^{-1/2}.
$$

The normalizer is $B(1/2,1/2)=\pi$. Therefore

$$
\boxed{\pi_J(\theta)=\frac1{\pi\sqrt{\theta(1-\theta)}},\quad0<\theta<1;\qquad
\theta\sim\operatorname{Beta}(1/2,1/2).}
$$

This [Jeffreys prior for a Bernoulli parameter](../../../../../jeffreys-prior-for-a-bernoulli-parameter.md) is proper despite its integrable endpoint singularities. It is the [arcsine distribution](../../../../../arcsine-distribution.md). It replaces the specified $a,b>1$ [prior distribution](../../../../../prior-probability.md) in part (a) when the [Jeffreys prior](../../../../../jeffreys-prior.md) rule is chosen; it is not one of those restricted priors.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
