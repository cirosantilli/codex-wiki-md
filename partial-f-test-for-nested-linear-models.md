# Partial F-test for nested linear models

↑ **Parent:** [F-test](f-test.md)

Let $M_0\subset M_1$ be nested [normal linear models](normal-linear-model.md) with $p_0,p_1$ independent coefficients and $n$ observations. Under the reduced model,

$$
F=\frac{(\operatorname{RSS}_0-\operatorname{RSS}_1)/(p_1-p_0)}{\operatorname{RSS}_1/(n-p_1)}\sim F_{p_1-p_0,n-p_1}.
$$

The difference of the orthogonal projection matrices onto the two model spaces is an orthogonal projection of rank $p_1-p_0$, orthogonal to the full-model residual projection. Independent [normal distribution](normal-distribution.md) projections therefore give independent chi-squared numerators and denominators after division by $\sigma^2$. This proves the ratio law. The test evaluates the extra terms conditional on all reduced-model terms, and estimates the unknown common variance from the full model.

## ↑ Ancestors (5)

1. [F-test](f-test.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/1/i/solution.md)
