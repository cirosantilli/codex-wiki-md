<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**False.** In fact, standard one-dimensional [Brownian motion](../../../../../../brownian-motion-split.md) satisfies $\liminf_{t\to\infty}B_t=-\infty$ almost surely. For each integer $m\geq1$, let $\tau_{-m}=\inf\{t:B_t=-m\}$. The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md), applied to $-B$, gives

$$
\mathbb P(\tau_{-m}\leq t)=2\mathbb P(B_t\leq-m)=2\bigl(1-\Phi(m/\sqrt t)\bigr)\longrightarrow1,
$$

where $\Phi$ is the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). Thus each negative integer is reached almost surely. Intersecting these countably many probability-one events, all negative integer levels are reached on the same path. Their hitting times must become arbitrarily large, because a continuous path is bounded on every compact time interval. Hence the path cannot tend to positive infinity. Applying the same argument to positive levels also gives $\limsup_{t\to\infty}B_t=+\infty$ almost surely.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
