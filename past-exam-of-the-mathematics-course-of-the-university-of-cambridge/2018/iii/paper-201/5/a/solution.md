<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [stopping time](../../../../../../stopping-time.md) $T$ of a [Brownian filtration](../../../../../../brownian-filtration.md), define the reflected [stochastic process](../../../../../../stochastic-process-split.md)

$$
\boxed{\widehat B_t=\begin{cases}B_t,&t\leq T,\\2B_T-B_t,&t>T.\end{cases}}
$$

The [Brownian reflection at a stopping time](../../../../../../brownian-reflection-at-a-stopping-time.md) form of the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) states that **$\widehat B$ is again standard [Brownian motion](../../../../../../brownian-motion-split.md)**. If $T=\infty$, leave the path unchanged; the second branch is used only when $T<t$.

For an [almost surely](../../../../../../almost-sure-convergence.md) finite $T$, the [Strong Markov property](../../../../../../strong-markov-property.md) says that $(B_{T+s}-B_T)_{s\geq0}$ is a fresh [Brownian motion](../../../../../../brownian-motion-split.md) [independent](../../../../../../independent-random-variables.md) of $\mathcal F_T$. Its negative has the same [probability distribution](../../../../../../probability-distribution.md), so reflecting the future preserves the full path [probability distribution](../../../../../../probability-distribution.md). Allowing $T=\infty$ follows by applying this argument to $T\wedge n$ and restricting to each fixed finite time interval.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
