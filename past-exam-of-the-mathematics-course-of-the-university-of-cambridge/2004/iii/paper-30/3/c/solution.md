<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Itô product rule](../../../../../../ito-product-rule.md) with the deterministic factor $e^{-\lambda t}$. Its [quadratic covariation](../../../../../../quadratic-covariation.md) with $X$ is zero, giving

$$
dY_t=e^{-\lambda t}dX_t-\lambda e^{-\lambda t}X_tdt
=\sqrt{2\lambda}\,dW_t-\lambda Y_tdt.
$$

Multiplication by the integrating factor $e^{\lambda t}$ solves the [Ornstein-Uhlenbeck stochastic differential equation](../../../../../../ornstein-uhlenbeck-stochastic-differential-equation.md):

$$
\boxed{Y_t=e^{-\lambda t}B_1+\sqrt{2\lambda}\int_0^te^{-\lambda(t-s)}\,dW_s.}
$$

The initial value $B_1$ is standard normal and independent of the future driving [Brownian motion](../../../../../../brownian-motion-split.md). Thus $Y$ is a centered [Gaussian process](../../../../../../gaussian-process.md) with [variance](../../../../../../variance-split.md) one. For $s\le t$, its independent future noise gives $\mathbb E(Y_sY_t)=e^{-\lambda(t-s)}$. Its Gaussian finite-dimensional distributions consequently depend only on time differences, so it is a [stationary process](../../../../../../stationary-process.md). This verifies the [exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](../../../../../../exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process.md) directly.

## ↑ Ancestors (11)

1. [C](../c.md)
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
