<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use a [generalized estimating equation](../../../../../../generalized-estimating-equation.md) with any well-behaved positive-definite [working correlation matrix](../../../../../../working-correlation-matrix.md). Let $\gamma$ collect the marginal intercept and slopes, let $m_i(\gamma)$ be the vector of three correct marginal means, and put $D_i=\partial m_i/\partial\gamma^{\mathsf T}$. Write the working [covariance](../../../../../../covariance.md) as $V_i=A_i^{1/2}R_i(\alpha)A_i^{1/2}$, where the proposed Poisson [variance](../../../../../../variance-split.md) gives $A_i=\operatorname{diag}(m_i)$; working [independence](../../../../../../independent-random-variables.md) is also allowed. Solve

$$
\boxed{\sum_{i=1}^mD_i^{\mathsf T}V_i^{-1}(Y_i-m_i)=0}.
$$

At the true mean, each cluster residual has [expectation](../../../../../../expected-value.md) zero, so the estimating equation is unbiased regardless of whether $V_i$ equals the actual [covariance](../../../../../../covariance.md). With [independent](../../../../../../independent-random-variables.md) students, sufficient covariate variation and regularity as $m\to\infty$, this gives consistent mean coefficients.

Replace the model-based [covariance](../../../../../../covariance.md) by the cluster-level [sandwich covariance matrix](../../../../../../sandwich-covariance-matrix.md). Evaluated at the fitted values, define

$$
\widehat A=\sum_iD_i^{\mathsf T}V_i^{-1}D_i,\qquad
\widehat B=\sum_iD_i^{\mathsf T}V_i^{-1}r_ir_i^{\mathsf T}V_i^{-1}D_i,
\qquad r_i=Y_i-\widehat m_i.
$$

Then

$$
\boxed{\widehat{\operatorname{Cov}}(\widehat\gamma)
=\widehat A^{-1}\widehat B\widehat A^{-1}}.
$$

The residual outer products estimate the actual within-student variability, including correlations and extra-Poisson [variance](../../../../../../variance-split.md) absent from the working model. Use these [standard errors](../../../../../../standard-error.md) for asymptotic [Wald tests](../../../../../../wald-test.md) and [confidence intervals](../../../../../../confidence-interval.md); exponentiating the treatment coefficient and its interval gives the mean-count [rate ratio](../../../../../../rate-ratio.md) and interval. Treating the $3m$ observations as [independent](../../../../../../independent-random-variables.md) when forming the sandwich meat would miss the within-student dependence. The effective asymptotic replication is the number of students, so a small number of clusters requires further finite-sample care rather than assuming that three measurements per student repair the large-sample approximation.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
