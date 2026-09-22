# Discrete hazard

↑ **Parent:** [Hazard function](hazard-function.md)

At ordered possible failure times $t_j$, the [discrete hazard](discrete-hazard.md) is $h_j=\mathbb P(T=t_j\mid T>t_{j-1})$. Its [survival function](survival-function.md) satisfies $S(t_j)=S(t_{j-1})(1-h_j)$, and hence $S(t)=\prod_{t_j\le t}(1-h_j)$. Estimating $h_j$ by the observed number of failures divided by the [risk set](risk-set.md) size under [independent censoring](independent-censoring.md) yields the [Kaplan–Meier estimator](kaplan-meier-estimator.md). Unlike a continuous-time hazard rate, a [discrete hazard](discrete-hazard.md) is a probability between zero and one.

## ↑ Ancestors (7)

1. [Hazard function](hazard-function.md)
2. [Survival function](survival-function.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Constrained Kaplan–Meier estimator](constrained-kaplan-meier-estimator.md)
- [Discrete hazard](discrete-hazard.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37/5/b/solution.md)
