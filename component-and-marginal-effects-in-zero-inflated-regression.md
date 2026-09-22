# Component and marginal effects in zero-inflated regression

↑ **Parent:** [Zero-inflated Poisson regression](zero-inflated-poisson-regression.md)

A logarithmic count-component contrast $b$ multiplies the susceptible mean by $e^b$, while a zero-logit contrast $g$ multiplies the structural-zero odds by $e^g$. If the baseline zero predictor is $\eta$, the marginal mean ratio is

$$
e^b\frac{1+e^{\eta}}{1+e^{\eta+g}}.
$$

Thus the count ratio alone is not a population-average effect when a covariate changes both components. With [interaction terms](interaction-term.md), the relevant count contrast must first include the interactions for the stated reference group.

## ↑ Ancestors (10)

1. [Zero-inflated Poisson regression](zero-inflated-poisson-regression.md)
2. [Zero-inflated Poisson distribution](zero-inflated-poisson-distribution.md)
3. [Poisson distribution](poisson-distribution.md)
4. [Discrete probability distribution](discrete-probability-distribution-split.md)
5. [Probability distribution](probability-distribution.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/6/b/i/solution.md)
