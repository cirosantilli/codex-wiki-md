<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $x_r,x_t$ for two rows of the data matrix and $\delta=x_r-x_t$. Three possible dissimilarities for continuous variables are the following.

The [Euclidean distance](../../../../../../euclidean-distance.md) is

$$
\boxed{d_E(x_r,x_t)=\sqrt{\sum_{j=1}^p\delta_j^2}.}
$$

It is simple and has the usual geometric interpretation when coordinates have comparable units. Its disadvantage is sensitivity to the numerical scales: a change of units or a high-variance variable can dominate it. Strongly correlated coordinates can also give repeated weight to essentially the same information. Squared [Euclidean distance](../../../../../../euclidean-distance.md) is useful in some methods, but is not itself a metric because it need not satisfy the triangle inequality.

The [standardized Euclidean distance](../../../../../../standardized-euclidean-distance.md) is

$$
\boxed{d_S(x_r,x_t)=\sqrt{\sum_{j=1}^p\frac{\delta_j^2}{s_j^2}},}
$$

where $s_j^2$ is the [sample variance](../../../../../../sample-variance.md) of coordinate $j$ across individuals. It measures differences in standard-deviation units and is invariant under positive coordinate rescalings when the scales are estimated consistently. It is useful for differently measured variables, but requires nonzero [sample variances](../../../../../../sample-variance.md), ignores correlations between coordinates and can give excessive influence to a low-variance noisy variable. With fixed positive scales it is a [Euclidean distance](../../../../../../euclidean-distance.md) after a diagonal change of coordinates, so it is a metric.

The [Mahalanobis distance](../../../../../../mahalanobis-distance.md) is

$$
\boxed{d_M(x_r,x_t)=\sqrt{\delta^TS^{-1}\delta},}
$$

where $S$ is the pooled [sample covariance matrix](../../../../../../sample-covariance-matrix.md) of all individuals. If $S=CC^T$ is its [Cholesky decomposition](../../../../../../cholesky-decomposition.md), then $d_M=\|C^{-1}\delta\|_2$: it is [Euclidean distance](../../../../../../euclidean-distance.md) in whitened coordinates. It adjusts for both scales and correlations, avoiding duplicate weight for highly correlated variables, and is invariant under nonsingular affine transformations when the [sample covariance matrix](../../../../../../sample-covariance-matrix.md) is transformed accordingly. No [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) assumption is required merely to define the distance. However, $S$ must be a [positive-definite matrix](../../../../../../positive-definite-matrix.md); when there are too few observations or dependent coordinates, its inverse is unavailable. Estimation of $S^{-1}$ can also be unstable and sensitive to outliers. These trade-offs determine whether covariance adjustment is preferable to the simpler distances.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
