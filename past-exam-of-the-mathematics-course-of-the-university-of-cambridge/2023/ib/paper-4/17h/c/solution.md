<h1 id="17h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put

$$
S_r=\sum_{i=1}^n x_i^r.
$$

Independence and $\operatorname{var}(Y_i)=\theta x_i$ give

$$
\boxed{\operatorname{var}(\widehat\theta_{LS})
=\frac{\theta S_3}{S_2^2}},
$$

whereas $\sum_iY_i\sim\operatorname{Poisson}(\theta S_1)$ gives

$$
\boxed{\operatorname{var}(\widehat\theta_{MLE})
=\frac{\theta}{S_1}}.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), applied to $(x_i^{1/2})$ and $(x_i^{3/2})$, yields

$$
S_2^2=\left(\sum_i x_i^{1/2}x_i^{3/2}\right)^2
\leq S_1S_3.
$$

Consequently

$$
\boxed{\operatorname{var}(\widehat\theta_{MLE})
\leq\operatorname{var}(\widehat\theta_{LS})}.
$$

Equality holds exactly when all positive exposures $x_i$ are equal. This is the [variance comparison for Poisson exposure estimators](../../../../../../variance-comparison-for-poisson-exposure-estimators.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
