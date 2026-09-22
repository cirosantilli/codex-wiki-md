<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [stochastic integral](../../../../../../stochastic-integral.md)

$$
\boxed{W_t=\frac1{\sqrt{2\lambda}}\int_1^{e^{2\lambda t}}u^{-1/2}\,dB_u.}
$$

It is adapted to $\mathcal G_t$, starts at zero and has continuous paths. Integrals over disjoint clock intervals are centered Gaussian and independent, and an increment from $s$ to $t$ is independent of $\mathcal G_s$. The [Itô isometry](../../../../../../ito-isometry.md) gives its [variance](../../../../../../variance-split.md)

$$
\frac1{2\lambda}\int_{e^{2\lambda s}}^{e^{2\lambda t}}\frac{du}{u}=t-s.
$$

These are precisely the defining properties of a $\mathcal G_t$-[Brownian motion](../../../../../../brownian-motion-split.md); in particular its future increments are independent of $\mathcal G_0=\mathcal F_1$.

Deterministic substitution in the [stochastic integral](../../../../../../stochastic-integral.md), first for step integrands and then by the [Itô isometry](../../../../../../ito-isometry.md), gives $dX_s=\sqrt{2\lambda}e^{\lambda s}dW_s$. Hence

$$
\boxed{X_t=B_1+\sqrt{2\lambda}\int_0^te^{\lambda s}\,dW_s.}
$$

The initial term is essential: a [stochastic integral](../../../../../../stochastic-integral.md) from time zero alone cannot equal $X$, since $X_0=B_1$. This is the unscaled part of the [exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](../../../../../../exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
