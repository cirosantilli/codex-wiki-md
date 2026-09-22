<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\theta=(\mu-r)/\sigma$. The positive density

$$
Z_T=\exp\left(-\theta W_T-\frac12\theta^2T\right)
$$

has mean one, and the [Girsanov theorem](../../../../../../girsanov-theorem.md) makes $W_t^Q=W_t+\theta t$ a [Brownian motion](../../../../../../brownian-motion-split.md) under the equivalent measure $Q$. Hence

$$
dS_t=S_t(r\,dt+\sigma\,dW_t^Q).
$$

The [Black-Scholes equation](../../../../../../black-scholes-equation.md) makes $e^{-rt}V(t,S_t)$ a local martingale. Bounded $V$ on the finite horizon makes it a true martingale, so its terminal condition gives the [risk-neutral valuation](../../../../../../risk-neutral-pricing.md)

$$
V(t,S_t)=e^{-r(T-t)}\mathbb E_Q[g(S_T)\mid\mathcal F_t].
$$

The [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) solution under $Q$ is

$$
S_T=S_t\exp\left((r-\tfrac12\sigma^2)(T-t)+\sigma(W_T^Q-W_t^Q)\right).
$$

The Brownian increment is independent of $\mathcal F_t$ and equals $\sqrt{T-t}\,Z$ in distribution, where $Z$ has the [standard normal distribution](../../../../../../standard-normal-distribution.md). Therefore

$$
\boxed{V(t,s)=e^{-r(T-t)}\mathbb E\left[g\left(se^{a(t)+b(t)Z}\right)\right],\qquad
a(t)=(r-\tfrac12\sigma^2)(T-t),\quad b(t)=\sigma\sqrt{T-t}.}
$$

The expectation on the right is only an integral against the standard normal law; the physical drift $\mu$ has disappeared.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
