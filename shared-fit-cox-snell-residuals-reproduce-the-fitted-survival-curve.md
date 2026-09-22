<h1 id="shared-fit-cox-snell-residuals-reproduce-the-fitted-survival-curve">Shared-fit Cox–Snell residuals reproduce the fitted survival curve</h1>

↑ **Parent:** [Cox–Snell residual survival diagnostic](cox-snell-residual-survival-diagnostic.md)

If a common [Kaplan–Meier estimator](kaplan-meier-estimator.md) $\widehat S$ is fitted and the same data are transformed to $u_i=-\log\widehat S(x_i)$ with censoring indicators retained, event ordering and risk sets are preserved under compatible tie conventions. At a transformed event time $u_j$, the residual product-limit estimate equals $\widehat S(x_j)=e^{-u_j}$. Consequently agreement of the pooled residual curve with the exponential target is largely built into the construction. Separate group curves or a model fitted with covariates can reveal differences concealed by the pooled fit. Residuals become infinite if the fitted survivor reaches zero.

// Target: survival-analysis.bigb

## ↑ Ancestors (7)

1. [Cox–Snell residual survival diagnostic](cox-snell-residual-survival-diagnostic.md)
2. [Cox–Snell residual](cox-snell-residual.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/c/solution.md)
