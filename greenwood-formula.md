# Greenwood formula

↑ **Parent:** [Kaplan–Meier estimator](kaplan-meier-estimator.md)

For the [Kaplan–Meier estimator](kaplan-meier-estimator.md), the estimated [variance](variance-split.md) is

$$
\widehat{\operatorname{Var}}(\widehat S(t))=\widehat S(t)^2\sum_{t_j\le t}\frac{d_j}{r_j(r_j-d_j)}.
$$

The formula follows by summing approximate variances of the logarithms of the conditional survival factors and applying the [delta method](delta-method.md) to their product. Its square root is the estimated [standard error](standard-error.md). The same expression uses the actual delayed-entry [risk sets](risk-set.md) for the [Kaplan–Meier estimator with delayed entry](kaplan-meier-estimator-with-delayed-entry.md). When $0<\widehat S(t)<1$ and every contributing $r_j>d_j$, an approximate log-scale [confidence interval](confidence-interval.md) is $\exp\{\log\widehat S(t)\pm z_{1-\alpha/2}\widehat{\operatorname{se}}(\widehat S(t))/\widehat S(t)\}$, with the upper endpoint capped at one. This interval can be inaccurate with very small [risk sets](risk-set.md).

## ↑ Ancestors (6)

1. [Kaplan–Meier estimator](kaplan-meier-estimator.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/5/b/i/solution.md)
