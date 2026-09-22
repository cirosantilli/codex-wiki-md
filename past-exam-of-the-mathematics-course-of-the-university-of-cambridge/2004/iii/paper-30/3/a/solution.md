<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The deterministic clock is $a(t)=e^{2\lambda t}$, so $a(0)=1$. For $s\le t$, the [martingale](../../../../../../martingale-split.md) property of [Brownian motion](../../../../../../brownian-motion-split.md) gives

$$
\mathbb E(X_t\mid\mathcal G_s)=\mathbb E(B_{a(t)}\mid\mathcal F_{a(s)})=B_{a(s)}=X_s.
$$

Integrability follows from the Gaussian second moment. Thus $X$ is a [martingale](../../../../../../martingale-split.md) in the time-changed [filtration](../../../../../../filtration-probability-theory.md).

Its increments have [variance](../../../../../../variance-split.md) $a(t)-a(s)$ and are independent of $\mathcal G_s$. Equivalently, $X_t^2-a(t)$ is a [martingale](../../../../../../martingale-split.md). Since a [quadratic variation](../../../../../../quadratic-variation.md) starts at zero, its compensator must be normalized at $t=0$:

$$
\boxed{[X]_t=e^{2\lambda t}-1.}
$$

The initial random variable $X_0=B_1$ does not contribute to [quadratic variation](../../../../../../quadratic-variation.md). The expression $e^{2\lambda t}$ alone would violate $[X]_0=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
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
