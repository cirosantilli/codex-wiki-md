<h1 id="a/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For every $m$, $D_m$ is a continuous square-integrable vector [martingale](../../../../../martingale-split.md). Its norm is a [submartingale](../../../../../submartingale.md), so the [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) and the estimate from part (c) give

$$
\mathbb E\sup_{t\leq T}|D_m(t)|^2\leq4|a|^2\frac{(KT)^{m+1}}{(m+1)!}.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) now shows

$$
\sum_m\mathbb E\sup_{t\leq T}|D_m(t)|
\leq2|a|\sum_m\frac{(KT)^{(m+1)/2}}{\sqrt{(m+1)!}}<\infty.
$$

By [Tonelli's theorem](../../../../../tonelli-theorem.md), the random sum of these suprema is finite almost surely. Therefore the telescoping series $a+\sum_mD_m(t)$ converges absolutely and uniformly on $[0,T]$ outside one null event. Its limit is continuous and agrees at each fixed time with the $L^2$ limit from part (c). Taking the intersection of the probability-one events for integer $T$ provides a single version on the whole half-line. Hence

$$
\boxed{\sup_{t\leq T}|y_t^{(n)}-y_t^{(\infty)}|\longrightarrow0\quad\text{almost surely for every finite }T.}
$$

This also gives the requested pointwise almost-sure convergence of the full sequence.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
