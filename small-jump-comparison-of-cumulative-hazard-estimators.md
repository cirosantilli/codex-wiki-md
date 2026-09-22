# Small-jump comparison of cumulative hazard estimators

↑ **Parent:** [Nelson–Aalen estimator](nelson-aalen-estimator.md)

At a failure time with $d$ events among $r$ at risk, the [Nelson–Aalen estimator](nelson-aalen-estimator.md) adds $u=d/r$, whereas minus the logarithm of the [Kaplan–Meier estimator](kaplan-meier-estimator.md) adds $-\log(1-u)$. For $0\le u<1$,

$$
0\le-\log(1-u)-u=\sum_{m=2}^{\infty}\frac{u^m}{m}\le\frac{u^2}{2(1-u)}.
$$

Thus small event fractions give close [cumulative hazard](cumulative-hazard-function.md) estimates. Large [risk sets](risk-set.md) alone do not suffice when a large fraction fail together. If all remaining individuals fail, the logarithmic estimate becomes infinite while the Nelson–Aalen jump is one.

## ↑ Ancestors (6)

1. [Nelson–Aalen estimator](nelson-aalen-estimator.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-40/2/iv/solution.md)
