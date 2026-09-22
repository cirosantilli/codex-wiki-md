# Independence log-linear model for a two-way contingency table

↑ **Parent:** [Log-linear model](log-linear-model.md)

For cell counts $Y_{ij}$ in a two-way [contingency table](contingency-table.md), the independence model is

$$
Y_{ij}\sim\operatorname{Pois}(\mu_{ij}),
\qquad
\log\mu_{ij}=\lambda+\lambda_i^{(1)}+\lambda_j^{(2)}.
$$

The absence of an interaction makes $\mu_{ij}$ factor as a row effect times a column effect. Its [maximum-likelihood fitted values](maximum-likelihood-fitted-value.md) are

$$
\widehat\mu_{ij}=\frac{y_{i+}y_{+j}}{y_{++}}.
$$

## ↑ Ancestors (7)

1. [Log-linear model](log-linear-model.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/5j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/13j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/13j/c/solution.md)
