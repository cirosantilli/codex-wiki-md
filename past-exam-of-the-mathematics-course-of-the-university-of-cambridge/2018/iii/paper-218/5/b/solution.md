<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The parameters are $\mu\in\mathbb R$, $|\phi|<1$ and innovation [variance](../../../../../../variance-split.md) $\sigma^2>0$. Stationarity gives $X_1\sim N(\mu,\sigma^2/(1-\phi^2))$, and the [Markov property](../../../../../../markov-property.md) gives $X_t\mid X_{t-1}\sim N(\mu+\phi(X_{t-1}-\mu),\sigma^2)$. Multiplying the initial density and the transition densities yields the [stationary Gaussian AR1 likelihood](../../../../../../stationary-gaussian-ar1-likelihood.md), with $n=31$:

$$
\boxed{L(\mu,\phi,\sigma^2;x)=(2\pi\sigma^2)^{-n/2}\sqrt{1-\phi^2}\exp\left[-\frac{(1-\phi^2)(x_1-\mu)^2+\sum_{t=2}^n\{(x_t-\mu)-\phi(x_{t-1}-\mu)\}^2}{2\sigma^2}\right].}
$$

The initial-observation factor depends on all three parameters and must be retained for the full stationary [likelihood function](../../../../../../likelihood-function.md). Omitting it gives a conditional likelihood given $X_1$, a different objective.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
