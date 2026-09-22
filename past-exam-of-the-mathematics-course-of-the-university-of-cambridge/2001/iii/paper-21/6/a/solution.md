<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By the usual definition of a [Lévy process](../../../../../../levy-process.md), $X_0=0$ almost surely. The two [martingale](../../../../../../martingale-split.md) assumptions give

$$
\mathbb E X_t=0,\qquad \mathbb E X_t^2=t.
$$

For a continuous [Lévy process](../../../../../../levy-process.md), the jump measure in the [Lévy–Khintchine formula](../../../../../../levy-khintchine-formula.md) is zero, and the process has the form of a Brownian Gaussian component plus a deterministic drift. Thus its [characteristic function](../../../../../../characteristic-function.md) is

$$
\mathbb E e^{iuX_t}=\exp\left(iumt-\tfrac12\sigma^2tu^2\right).
$$

The first moment makes $m=0$, and the second moment makes $\sigma^2=1$. Consequently

$$
\boxed{X_1\sim N(0,1),\qquad (X_t)\text{ is standard Brownian motion}.}
$$

Equivalently, continuity and the martingale identity $X_t^2-t$ identify the [quadratic variation](../../../../../../quadratic-variation.md) as $t$, so the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) gives the same conclusion. A continuous nonzero drift is excluded by the mean-zero martingale assumption.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
