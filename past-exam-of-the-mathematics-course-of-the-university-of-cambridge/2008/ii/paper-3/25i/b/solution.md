<h1 id="25i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this [alternating arrival and service queue](../../../../../../alternating-arrival-and-service-queue.md), set $\theta=\lambda(\mu+\beta)/[\mu(\lambda+\alpha)]$. Direct multiplication gives $(\theta,\lambda/\mu)B=\theta(\theta,\lambda/\mu)$, so the initial row is a left [eigenvector](../../../../../../eigenvector.md) and $(\pi_{iC},\pi_{iW})=\theta^{i-1}(\pi_{1C},\pi_{1W})$. Consequently

$$
\pi_{iC}=\frac{\beta z}{\lambda+\alpha}\theta^i\quad(i\geq0),\qquad
\pi_{iW}=\frac{\beta\lambda z}{\mu(\lambda+\alpha)}\theta^{i-1}\quad(i\geq1),\qquad\pi_{0W}=z.
$$

These nonnegative probabilities can be normalized exactly when $\theta<1$, equivalently $\mu\alpha>\lambda\beta$. Summing the [geometric series](../../../../../../geometric-series.md) gives

$$
\boxed{z=\frac{\mu\alpha-\lambda\beta}{\mu(\alpha+\beta)},\qquad\text{positive recurrence}\iff\mu\alpha>\lambda\beta.}
$$

When $\theta\geq1$ no positive multiple of the invariant sequence is summable, so no [stationary distribution](../../../../../../stationary-distribution.md) exists. This rules out positive recurrence; absence of a stationary probability alone should not be used to distinguish null recurrence from transience.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
