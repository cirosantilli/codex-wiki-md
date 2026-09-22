<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Y(t)$ be the [at-risk process](../../../../../../at-risk-process.md) and $N(t)$ the [counting process](../../../../../../counting-process.md) for observed events. Over a short interval, the multiplicative-intensity model gives

$$
\mathbb E\{dN(t)\mid\mathcal F_{t-}\}=Y(t)h(t),dt
=Y(t),dH(t),
$$

where $h$ is the [hazard function](../../../../../../hazard-function.md) and $H$ the [cumulative hazard function](../../../../../../cumulative-hazard-function.md). Solving this relation for the infinitesimal hazard increment suggests $d\widehat H(t)=dN(t)/Y(t)$. Summing over distinct event times gives the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md)

$$
\widehat H(t)=\sum_{j:a_j\leq t}\frac{d_j}{r_j},
$$

where $d_j$ events occur among $r_j$ individuals at risk. Here there are no ties, so $d_j=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
