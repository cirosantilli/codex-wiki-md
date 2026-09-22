<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N(t)=\sum_iN_i(t)$ and $Y(t)=\sum_iY_i(t)$ be the total observed [counting process](../../../../../../counting-process.md) and size of the [risk set](../../../../../../risk-set.md). When the individual [cumulative hazard functions](../../../../../../cumulative-hazard-function.md) are all $H_0$, summing the conditional intensity equations gives

$$
\mathbb E(dN(t)\mid\mathcal H_{t-})=Y(t)\,dH_0(t).
$$

Replace the expected increment by its observed value and divide by the predictable [risk set](../../../../../../risk-set.md) size. Thus **the Nelson–Aalen estimator in integral form** is

$$
\boxed{\widehat H_{NA}(t)=\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dN(u),}
$$

with the integrand defined as zero when $Y(u)=0$. This is an integral against the step [counting process](../../../../../../counting-process.md), so each event time contributes its event count divided by the [risk set](../../../../../../risk-set.md) just before that time. The [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) estimates integrated hazard over times with observable risk; it does not supply information after observation has ended.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
