<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Adaptive rejection sampling](../../../../../../adaptive-rejection-sampling.md) is exact [rejection sampling](../../../../../../rejection-sampling.md) for a differentiable [log-concave probability density](../../../../../../log-concave-probability-density.md). Given interior evaluation points $s_j$, construct the upper envelope

$$
u(x)=\min_j\{\ell(s_j)+\ell'(s_j)(x-s_j)\},\qquad \ell(x)=\log h(x),
$$

where $h$ is the unnormalized target [probability density function](../../../../../../probability-density-function.md). The [concave function](../../../../../../concave-function.md) $\ell$ lies below all its [tangent lines](../../../../../../tangent-line.md), so $e^u\geq h$. Interpolation between adjacent evaluation points gives a lower envelope $l\leq\ell$ there, allowing a squeeze test. The normalized upper envelope $g=e^u/\int e^u$ is a piecewise exponential [proposal distribution](../../../../../../proposal-distribution.md).

Draw $X\sim g$ and an independent $W$ from the [uniform distribution](../../../../../../continuous-uniform-distribution.md), and accept when $W\leq e^{\ell(X)-u(X)}$. A squeeze test $W\leq e^{l(X)-u(X)}$ can establish acceptance without evaluating $\ell(X)$. Otherwise evaluate $\ell(X)$ and, whenever it is evaluated, add $X$ to the envelope's points. Repeat until acceptance. On each linear piece $u(x)=r x+s$, its [integral](../../../../../../integral.md) is $e^s(e^{r d}-e^{r c})/r$ on $[c,d]$, with value $e^s(d-c)$ when $r=0$. These [integrals](../../../../../../integral.md) select a piece; [inverse transform sampling](../../../../../../inverse-transform-sampling.md) samples within it.

Here, with $a=y_4$ and $b=y_2+y_3$, the [log-posterior](../../../../../../log-posterior.md) on $(0,1)$ has

$$
\ell(\theta)=y_1\log(2+\theta)+a\log\theta+b\log(1-\theta),\qquad
\boxed{\ell''(\theta)=-\frac{y_1}{(2+\theta)^2}-\frac{a}{\theta^2}-\frac{b}{(1-\theta)^2}\leq0.}
$$

Choose evaluation points strictly inside $(0,1)$, avoiding any endpoint singularities of the [logarithm](../../../../../../logarithm.md). Every finite set of [tangent lines](../../../../../../tangent-line.md) gives a finite upper-envelope [integral](../../../../../../integral.md) on this bounded interval; slope conditions needed for unbounded supports are unnecessary. When $N=0$ the [posterior distribution](../../../../../../bayesian-posterior.md) is simply the [uniform distribution](../../../../../../continuous-uniform-distribution.md) and may be sampled directly.

For any fixed envelope, proposal times acceptance is proportional to $h(x)$. Conditional on all past evaluations and rejections, the next accepted value therefore has the same normalized [posterior density](../../../../../../posterior-density.md). To see that adaptation does not spoil this, at every attempted draw its accepted mass is a scalar times that fixed [posterior density](../../../../../../posterior-density.md); summing over possible rejection histories preserves it. The acceptance [probability](../../../../../../probability.md) stays bounded below by its positive initial-envelope value because insertion only lowers the upper envelope. Thus acceptance occurs almost surely. With fresh independent randomness, successive accepted values are **exact [independent](../../../../../../independent-random-variables.md) samples from the [posterior distribution](../../../../../../bayesian-posterior.md)**, even when the envelope is retained and improved between them.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
