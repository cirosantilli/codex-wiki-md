# Risk-set-adjusted relative survivor estimator

↑ **Parent:** [Relative survivor function](relative-survivor-function.md)

With a common [excess hazard](excess-hazard.md), let $\overline h_B=\sum_iY_i h_B^{(i)}/\sum_iY_i$ be the known [background hazard](background-hazard.md) averaged over the current [risk set](risk-set.md). Estimate the excess [cumulative hazard](cumulative-hazard-function.md) by subtracting $\int\overline h_B$ from the [Nelson–Aalen estimator](nelson-aalen-estimator.md). Applying the product-limit construction gives the displayed estimator: the continuous background correction multiplies the ordinary [Kaplan–Meier estimator](kaplan-meier-estimator.md). Its event jump is $1-d_j/r_j$, while between events it grows at rate $\overline h_B\widehat F_E$. Hence the unconstrained curve can increase, even if the true [excess hazard](excess-hazard.md) is nonnegative. Replacing its jump factor by $\exp(-d_j/r_j)$ gives the alternative exponential cumulative-hazard estimator; these versions are close for small event fractions but are not identical.

## ↑ Ancestors (7)

1. [Relative survivor function](relative-survivor-function.md)
2. [Relative survival](relative-survival.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41/5/b/solution.md)
