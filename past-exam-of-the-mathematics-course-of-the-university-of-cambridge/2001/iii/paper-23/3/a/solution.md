<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On a [filtered probability space](../../../../../../filtered-probability-space.md) carrying a standard [Brownian motion](../../../../../../brownian-motion-split.md) $W$ with independent increments relative to the [filtration](../../../../../../filtration-probability-theory.md), a strictly positive security price follows [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) with constant drift $\mu$ and volatility $\sigma$ if it solves the [stochastic differential equation](../../../../../../stochastic-differential-equation.md)

$$
\boxed{dS_t=\mu S_t\,dt+\sigma S_t\,dW_t,\qquad S_0>0.}
$$

Here $W_t-W_s$ is independent of $\mathcal F_s$ and has the [normal distribution](../../../../../../normal-distribution.md) $N(0,t-s)$ for $s<t$. The solution is

$$
S_t=S_0\exp\{(\mu-\sigma^2/2)t+\sigma W_t\}.
$$

Indeed applying the [Itô formula](../../../../../../ito-s-lemma.md) to this exponential gives the specified drift and volatility. Consequently the price is positive and continuous, and

$$
\log(S_t/S_s)\mid\mathcal F_s\sim
N((\mu-\sigma^2/2)(t-s),\sigma^2(t-s)).
$$

Thus disjoint log-return increments are independent and stationary. The parameter $\mu$ is the instantaneous expected relative return under the physical [probability measure](../../../../../../probability-measure.md), not the mean log-return. Under the pricing [risk-neutral measure](../../../../../../risk-neutral-measure.md) it becomes the risk-free rate for a non-dividend-paying [stock](../../../../../../stock.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
