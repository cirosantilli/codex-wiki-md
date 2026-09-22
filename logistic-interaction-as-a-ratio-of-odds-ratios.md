# Logistic interaction as a ratio of odds ratios

↑ **Parent:** [Interaction contrast](interaction-contrast.md)

For binary predictors $A,B$, a [logistic regression](logistic-regression.md) with [linear predictor](linear-predictor.md) $a+bA+cB+\delta AB$ has conditional [odds ratios](odds-ratio.md) $e^b$ at $B=0$ and $e^{b+\delta}$ at $B=1$. Their ratio is $e^\delta$. The same interaction can be computed from the four cell [logit link](logit.md) values as $\delta=\eta_{11}-\eta_{10}-\eta_{01}+\eta_{00}$. Independent positive event and nonevent counts in each cell give an estimated [variance](variance-split.md) for this contrast equal to the sum of all eight reciprocal counts. An interaction on the [odds ratio](odds-ratio.md) scale is not an interaction on the absolute-risk scale.

## ↑ Ancestors (12)

1. [Interaction contrast](interaction-contrast.md)
2. [Treatment contrast](treatment-contrast.md)
3. [Linear contrast of cell means](linear-contrast-of-cell-means.md)
4. [Cell-means parametrization](cell-means-parametrization.md)
5. [One-way normal linear model](one-way-normal-linear-model.md)
6. [Normal linear model](normal-linear-model.md)
7. [Statistical modelling](statistical-modelling-split.md)
8. [Statistical model](statistical-model-split.md)
9. [Probability and statistics](probability-and-statistics-split.md)
10. [Area of mathematics](area-of-mathematics.md)
11. [Mathematics](mathematics-split.md)
12. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/4/solution.md)
