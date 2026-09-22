# Restricted likelihood from orthogonal error contrasts

↑ **Parent:** [Restricted maximum likelihood](restricted-maximum-likelihood.md)

For $Y\sim N(X\beta,V_\theta)$ and a full-column-rank [design matrix](design-matrix.md) $X\in\mathbb R^{n\times p}$, take $A\in\mathbb R^{n\times(n-p)}$ with $A^TA=I$ and $A^TX=0$. Then $A^TY\sim N(0,A^TV_\theta A)$, so [restricted maximum likelihood](restricted-maximum-likelihood.md) maximizes

$$
\ell_R(\theta)=-\frac{n-p}{2}\log(2\pi)-\frac12\log\det(A^TV_\theta A)-\frac12Y^TA(A^TV_\theta A)^{-1}A^TY.
$$

Changing the [orthonormal basis](orthonormal-basis.md) by an orthogonal matrix leaves this expression unchanged.

## ↑ Ancestors (8)

1. [Restricted maximum likelihood](restricted-maximum-likelihood.md)
2. [Normal linear model](normal-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/1/c/solution.md)
