# Bias correction after an inverse transformation

↑ **Parent:** [Box–Cox transformation](box-cox-transformation.md)

A transformed-response regression estimates the conditional mean $m$ on the transformed scale. Inverting that mean does not generally estimate the original-scale mean, because nonlinear transformations do not commute with [expected values](expected-value.md). For a smooth inverse $g$ and centered transformed error of variance $\sigma^2$, a second-order [Taylor expansion](taylor-expansion.md) gives the displayed local correction. For $g(z)=z^q$ at positive $m$, it is $m^q+\tfrac12q(q-1)m^{q-2}\sigma^2$. The variance is the response's residual variance, not the sampling variance of the estimated mean. This approximation requires errors small enough that the inverse is meaningful over the relevant range; it is not an exact moment formula for arbitrary transformed noise.

## ↑ Ancestors (8)

1. [Box–Cox transformation](box-cox-transformation.md)
2. [Power transform](power-transform.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-102/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/1/solution.md)
