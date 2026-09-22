<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $N(t)$ count observed events and $Y(t)$ count individuals still in the [risk set](../../../../../../risk-set.md) just before $t$. Under a common [hazard function](../../../../../../hazard-function.md) $h(t)$ and [independent censoring](../../../../../../independent-censoring.md), the expected event count over a short interval, conditional on the observed past, is

$$
\operatorname E[dN(t)\mid\mathcal F_{t-}]=Y(t)h(t)\,dt=Y(t)\,dH(t).
$$

Here $H(t)=\int_0^t h(u)\,du$ is the [integrated hazard](../../../../../../cumulative-hazard-function.md). Thus an estimating increment for $dH$ is $dN/Y$, on the range where the [risk set](../../../../../../risk-set.md) is nonempty. Accumulating these increments gives the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md)

$$
\boxed{\widehat H(t)=\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dN(u)
=\sum_{t_j\leq t}\frac{\delta_j}{r_j}.}
$$

The observation times $t_j$ include both events and censorings, $r_j=Y(t_j)$, and $\delta_j$ is one for an event and zero for [censoring](../../../../../../censoring-statistics.md). Without ties each event adds $1/r_j$; [censoring](../../../../../../censoring-statistics.md) changes later [risk sets](../../../../../../risk-set.md) but adds nothing immediately. Equivalently, the local event fraction estimates the local hazard increment, and summing those estimates produces the [integrated hazard](../../../../../../cumulative-hazard-function.md). The [counting-process intensity in survival analysis](../../../../../../counting-process-intensity-in-survival-analysis.md) justifies this estimating equation; it does not imply exact finite-sample unbiasedness after the [risk set](../../../../../../risk-set.md) can become empty.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
