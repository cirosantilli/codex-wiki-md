# Mean accumulated hazard under independent censoring

↑ **Parent:** [Cumulative hazard function](cumulative-hazard-function.md)

Let $X=\min(T,C)$, $V=\mathbf1_{\{T\leq C\}}$, and suppose $T$ and $C$ are independent, with continuous failure density $f=hS$. Then the [Tonelli theorem](tonelli-theorem.md) gives

$$
\mathbb E H(X)=\int_0^\infty h(t)S(t)\mathbb P(C\geq t)dt=\mathbb P(T\leq C)=\mathbb EV.
$$

Thus $V-H(X)$ has mean zero. The identity also holds conditionally on covariates when censoring is independent conditionally on them. For an estimated hazard, the mean error is controlled by $\mathbb E|\widehat H(X)-H(X)|$, not by pointwise fit alone.

// Target: survival-analysis.bigb

## ↑ Ancestors (8)

1. [Cumulative hazard function](cumulative-hazard-function.md)
2. [Hazard function](hazard-function.md)
3. [Survival function](survival-function.md)
4. [Survival analysis](survival-analysis-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/d/solution.md)
