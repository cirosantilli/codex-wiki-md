# Bernstein bound for bounded-jump martingales

↑ **Parent:** [Martingale](martingale-split.md)

For a compensated jump [martingale](martingale-split.md) starting at zero, with jumps bounded in absolute value by $c$ and [predictable quadratic variation](predictable-quadratic-variation.md) at most $v$ on the interval, the displayed maximal bound holds. For $0<\theta c<3$, the elementary exponential bound

$$
e^{\theta h}-1-\theta h\le\frac{\theta^2h^2}{2(1-\theta c/3)}\qquad(|h|\le c)
$$

makes the exponential of $\theta M$ minus that multiple of its predictable bracket a nonnegative supermartingale. Stop at the first crossing of $\eta$ and use its mean bound. Taking $\theta=\eta/(v+c\eta/3)$ yields the one-sided bound; apply the same argument to $-M$ and use the [union bound](boole-s-inequality.md) for the displayed two-sided version. The elementary estimate follows from the exponential series and $k!\ge2\,3^{k-2}$ for $k\ge2$. If $v=0$, the compensated martingale is constant and the crossing probability is zero; the parameter choice above is needed only for $v>0$.

## ↑ Ancestors (6)

1. [Martingale](martingale-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38/6/solution.md)
