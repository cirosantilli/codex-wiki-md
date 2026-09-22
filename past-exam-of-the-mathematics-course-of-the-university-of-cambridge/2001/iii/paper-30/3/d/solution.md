<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Multivariate analysis of variance](../../../../../../multivariate-analysis-of-variance.md) tests differences between group mean vectors when each experimental unit has several correlated responses. For independent $p$-dimensional observations in $g$ groups, use a common positive-definite [covariance matrix](../../../../../../covariance-matrix.md) $\Sigma$ and the [multivariate normal](../../../../../../multivariate-normal-distribution.md) model $Y_{ri}\sim N_p(\mu_r,\Sigma)$. The null hypothesis is equality of all $g$ means.

Write $n=\sum_rn_r$, group means $\bar y_r$, and the size-weighted grand mean $\bar y$. The within-group and between-group scatter matrices are

$$
E=\sum_{r,i}(y_{ri}-\bar y_r)(y_{ri}-\bar y_r)^T,
\qquad H=\sum_rn_r(\bar y_r-\bar y)(\bar y_r-\bar y)^T.
$$

Expanding deviations about the group means yields total scatter $T=E+H$, with zero cross terms. Under the null, orthogonal normal projections give independent [Wishart distributions](../../../../../../wishart-distribution.md) $E\sim W_p(\Sigma,n-g)$ and $H\sim W_p(\Sigma,g-1)$.

With nonsingular $E$, the [Wilks lambda statistic](../../../../../../wilks-lambda-statistic.md) is

$$
\boxed{\Lambda=\frac{\det E}{\det(E+H)}=\prod_j(1+\theta_j)^{-1},}
$$

where the nonnegative $\theta_j$ are [eigenvalues](../../../../../../eigenvalue.md) of $E^{-1/2}HE^{-1/2}$. Maximizing the common covariance under the two mean models gives the likelihood ratio $\Lambda^{n/2}$, so small $\Lambda$ indicates large group separation relative to within-group spread. For fixed $p,g$ and large group sizes, the [Wilks theorem](../../../../../../wilks-theorem.md) gives $-n\log\Lambda\Rightarrow\chi^2_{p(g-1)}$ under the null; a finite-sample reference distribution can also be used.

The lower-right sketch shows two elongated groups whose centroid difference lies nearly across, rather than along, their long axes. Their correlation makes this multivariate separation much clearer than either marginal mean shift alone. Nonsingular linear rescaling changes $E$ and $H$ by congruence, leaving the determinant ratio unchanged. **MANOVA measures mean separation against the full within-group covariance geometry.** Its interpretation requires independent observations and an adequate common-covariance model; separate coordinatewise tests discard that geometry and raise multiple-testing issues.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
