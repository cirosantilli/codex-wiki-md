# Population-averaged logistic model for repeated binary outcomes

↑ **Parent:** [Generalized estimating equation](generalized-estimating-equation.md)

For independent subjects with repeated [Bernoulli](bernoulli-distribution.md) observations, specify marginal means $m_{ij}=\operatorname{logit}^{-1}(w_{ij}^T\gamma)$. A [generalized estimating equation](generalized-estimating-equation.md) uses their derivative matrix $D_i$ and working [covariance matrix](covariance-matrix.md) $V_i$ to solve $\sum_iD_i^TV_i^{-1}(Y_i-m_i)=0$. Subject-level [sandwich covariance matrices](sandwich-covariance-matrix.md) give robust uncertainty when the mean is correctly specified but the working correlation is not. The coefficients describe population [odds ratios](odds-ratio.md); this mean specification does not prescribe a complete joint distribution within a subject.

**Table of contents**

- [Inverse-observation-weighted estimating equations for longitudinal dropout](inverse-observation-weighted-estimating-equations-for-longitudinal-dropout.md)

## ↑ Ancestors (7)

1. [Generalized estimating equation](generalized-estimating-equation.md)
2. [Estimating equation](estimating-equation.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38/5/ii/a/solution.md)
