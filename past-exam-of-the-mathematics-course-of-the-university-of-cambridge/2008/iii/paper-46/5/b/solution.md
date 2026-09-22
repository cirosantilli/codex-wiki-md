<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At event time $t_j$, the vector [Schoenfeld residual](../../../../../../schoenfeld-residual.md) is

$$
\boxed{r_j=z_{i_j}-\bar z_j(\widehat\beta),}
$$

where $\widehat\beta$ is the fitted partial-likelihood coefficient. It compares the [covariate](../../../../../../covariate.md) of the person who actually failed with the [covariate](../../../../../../covariate.md) [mean](../../../../../../expected-value.md) predicted for the failing person, using the fitted [hazard](../../../../../../hazard-function.md) weights over the [risk set](../../../../../../risk-set.md). Under the model at the true coefficient, the conditional expected failing [covariate](../../../../../../covariate.md) is precisely that weighted [mean](../../../../../../expected-value.md), so the corresponding [Schoenfeld function](../../../../../../schoenfeld-function.md) is conditionally centered at zero. Residuals are defined at observed events, not at censoring times.

The score equation from part (a) is exactly

$$
U(\beta)=\sum_j[z_{i_j}-\bar z_j(\beta)].
$$

At a finite interior unpenalized maximum, $U(\widehat\beta)=0$, so

$$
\boxed{\sum_j r_j=0.}
$$

This is the intended fitted-residual identity. For an arbitrary trial coefficient it is a score, not generally zero; a single event with [covariates](../../../../../../covariate.md) zero and one in its [risk set](../../../../../../risk-set.md) can have Schoenfeld function $1/2$ at $\beta=0$. Penalized estimates or a boundary maximum also need their own score conditions rather than this unqualified zero-sum assertion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
