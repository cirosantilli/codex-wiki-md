# Bivariate probit model for endogenous treatment

↑ **Parent:** [Sensitivity analysis for unmeasured confounding](sensitivity-analysis-for-unmeasured-confounding.md)

A bivariate probit model for a binary treatment and outcome uses latent equations

$$
A=\mathbf1_{\{X^T\alpha+U>0\}},\qquad
Y=\mathbf1_{\{A\beta+X^T\gamma+V>0\}},
$$

where $(U,V)$ has a [bivariate normal distribution](bivariate-normal-distribution.md). Its correlation parameter represents dependence between the two latent disturbances; when nonzero, treatment is endogenous in the outcome equation.

## ↑ Ancestors (6)

1. [Sensitivity analysis for unmeasured confounding](sensitivity-analysis-for-unmeasured-confounding.md)
2. [Causal inference](causal-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-221/4/c/i/solution.md)
