<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Stop just before a large [predictable](../../../../../../predictable-process.md) coefficient would be used. Set

$$
\sigma_j=\inf\{t\geq0:|K_{t+1}|>j\},
$$

with the infimum of the empty set equal to infinity. Because $K_{t+1}$ is $\mathcal F_t$-measurable, $\sigma_j$ is a [stopping time](../../../../../../stopping-time.md). The increment of the stopped [martingale transform](../../../../../../martingale-transform.md) is

$$
Y_{t\wedge\sigma_j}-Y_{(t-1)\wedge\sigma_j}
=\mathbf1_{\{t\leq\sigma_j\}}K_t(M_t-M_{t-1}).
$$

Its coefficient is [predictable](../../../../../../predictable-process.md) and bounded by $j$: the first coefficient exceeding $j$ occurs at the step after stopping, and is never included. Part (c) makes $Y^{\sigma_j}$ a [martingale](../../../../../../martingale-split.md). Since the finitely many $K_s$ on any fixed finite horizon are finite almost surely, $\sigma_j\uparrow\infty$ almost surely. Thus

$$
\boxed{Y\text{ is a discrete-time local martingale}.}
$$

This is [predictable-coefficient localization of a martingale transform](../../../../../../predictable-coefficient-localization-of-a-martingale-transform.md). Stopping after taking the large increment would not give the required bound.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
