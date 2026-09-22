# Brownian weighted quadratic variation in L2

↑ **Parent:** [Quadratic variation](quadratic-variation.md)

For [Brownian motion](brownian-motion-split.md) and deterministic [partitions of an interval](partition-of-an-interval.md) $[0,t]$ whose mesh $|\pi|$ tends to zero, the displayed limit holds in [L2 space](l2-space-is-a-hilbert-space.md). Split the error into $U_\pi=\sum_jB_{t_j}((\Delta B_j)^2-\Delta t_j)$ and the [Riemann sum](riemann-sum.md) error $V_\pi=\sum_jB_{t_j}\Delta t_j-\int_0^tB_sds$. The summands of $U_\pi$ are [martingale differences](martingale-difference.md), hence [orthogonal](orthogonal-vectors.md) in [L2 space](l2-space-is-a-hilbert-space.md), and the [Gaussian fourth moment](gaussian-fourth-moment.md) gives

$$
\mathbb EU_\pi^2=2\sum_jt_j(\Delta t_j)^2\leq2t^2|\pi|.
$$

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) and the [Brownian increment](brownian-increment.md) [variance](variance-split.md) give $\mathbb EV_\pi^2\leq(t/2)\sum_j(\Delta t_j)^2\leq t^2|\pi|/2$. Both vanish. This proves the limit directly without a stochastic change-of-variables formula.

## ↑ Ancestors (8)

1. [Quadratic variation](quadratic-variation.md)
2. [Stochastic calculus](stochastic-calculus-split.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford/2023/2/b/i/solution.md)
