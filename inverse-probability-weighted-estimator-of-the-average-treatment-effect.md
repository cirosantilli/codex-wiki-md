# Inverse-probability-weighted estimator of the average treatment effect

↑ **Parent:** [Inverse probability weighting](inverse-probability-weighting.md)

For binary treatment, outcomes $Y_i$, and estimated [propensity score](propensity-score.md) $\widehat e(X_i)$, the inverse-probability-weighted estimator is

$$
\widehat{\operatorname{ATE}}_{\rm IPW}
=\frac1n\sum_{i=1}^n\left\{
\frac{A_iY_i}{\widehat e(X_i)}-
\frac{(1-A_i)Y_i}{1-\widehat e(X_i)}
\right\}.
$$

It is consistent under [conditional exchangeability](conditional-exchangeability.md), [consistency of potential outcomes](consistency-in-causal-inference.md), [positivity in causal inference](positivity-assumption.md), and a consistent propensity-score estimator.

## ↑ Ancestors (6)

1. [Inverse probability weighting](inverse-probability-weighting.md)
2. [Causal inference](causal-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-221/4/b/iii/solution.md)
