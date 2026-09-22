# Quasi-complete separation

↑ **Parent:** [Separation (statistics)](separation-statistics.md)

In a binary [logistic regression](logistic-regression.md), write the signed directional margin of observation $i$ as $(2y_i-1)x_i^Td$. Quasi-complete separation occurs when a nonzero direction $d$ makes all these margins nonnegative, with some zero and some strictly positive. Along coefficients $\beta+td$, $t\to\infty$, each observation's [log-likelihood](log-likelihood.md) contribution is nondecreasing, and those with positive margins strictly increase toward their limiting value. Hence the unpenalized fit cannot have a finite maximum in that direction. A group containing only outcome zeros is a simple example: sending its indicator coefficient to $-\infty$ improves that group's likelihood while leaving all other observations unchanged. Zero fitted risk is then a boundary limit, and ordinary finite-coefficient [Wald confidence intervals](wald-confidence-interval.md) are unavailable.

## ↑ Ancestors (9)

1. [Separation (statistics)](separation-statistics.md)
2. [Logistic regression](logistic-regression.md)
3. [Generalized linear model](generalized-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34/1/b/solution.md)
