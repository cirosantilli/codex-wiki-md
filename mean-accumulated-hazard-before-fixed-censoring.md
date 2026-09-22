# Mean accumulated hazard before fixed censoring

↑ **Parent:** [Cumulative hazard function](cumulative-hazard-function.md)

For a nonnegative continuous event time with [survival function](survival-function.md) S, [hazard function](hazard-function.md) h and H the [cumulative hazard](cumulative-hazard-function.md), split the expectation at c. The censored contribution is S(c)H(c). The event contribution is $\int_0^cH(t)f(t)dt=1-S(c)-S(c)H(c)$ by [integration by parts](integration-by-parts.md), since $dH=hdt$ and $f=hS$. Adding gives the displayed identity. Linearity extends it to the expected observed event count in a cohort, without requiring independence between subjects.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38/2/b/iii/solution.md)
