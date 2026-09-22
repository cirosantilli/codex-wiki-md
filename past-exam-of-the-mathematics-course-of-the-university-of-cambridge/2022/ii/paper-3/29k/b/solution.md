<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
\theta=\frac{\mu+\frac12\sigma^2-r}{\sigma}
$$

and define $Q$ on $\mathcal F_T$ by

$$
\frac{dQ}{dP}
=\exp\left(-\theta W_T-\frac12\theta^2T\right).
$$

The [Cameron-Martin theorem for a linear drift](../../../../../../cameron-martin-theorem-for-a-linear-drift.md) says that

$$
W_t^Q=W_t+\theta t
$$

is a [Brownian motion](../../../../../../brownian-motion-split.md) under $Q$. Therefore

$$
S_t=S_0
\exp\left(\left(r-\frac12\sigma^2\right)t+\sigma W_t^Q\right).
$$

The discounted stock is an exponential Brownian martingale, so $e^{-rt}S_t$ is a $Q$-martingale. Thus $Q$ is a [Risk-neutral measure for the Black-Scholes model](../../../../../../risk-neutral-measure-for-the-black-scholes-model.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
