<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

Partition the [design matrix](../../../../../design-matrix.md) accordingly as $X=(X_1\ \cdots\ X_k)$. The blocks $\beta_i,\beta_j$ are [orthogonal](../../../../../orthogonal-vectors.md) when $X_i^{\mathsf T}X_j=0$, meaning that their column spaces are [orthogonal vectors](../../../../../orthogonal-vectors.md). Mutual [orthogonality](../../../../../orthogonal-vectors.md) means that this holds for every pair of distinct blocks, so $X^{\mathsf T}X$ is block diagonal.

For the three scalar coefficients, the corresponding columns are $\mathbf1,x_1,x_2$. The necessary and sufficient conditions are

$$
\boxed{\sum_{i=1}^n x_{i1}=0,\qquad\sum_{i=1}^n x_{i2}=0,\qquad\sum_{i=1}^n x_{i1}x_{i2}=0.}
$$

Under the assumed full rank, neither explanatory column is zero. The [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is $\widehat\beta=(X^{\mathsf T}X)^{-1}X^{\mathsf T}Y$, and the [normal distribution](../../../../../normal-distribution.md) of $Y$ implies

$$
\widehat\beta\sim N_3\!\left(\beta,\sigma^2\operatorname{diag}\left(\frac1n,\frac1{\sum_i x_{i1}^2},\frac1{\sum_i x_{i2}^2}\right)\right).
$$

Thus **the three coefficient estimators are independent normal random variables**, not merely uncorrelated. This is a sampling-distribution statement with the true $\sigma^2$ fixed.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
