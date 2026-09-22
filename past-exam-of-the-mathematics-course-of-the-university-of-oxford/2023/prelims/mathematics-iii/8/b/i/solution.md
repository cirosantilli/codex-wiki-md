<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $D_j=X_j-\overline X$. The supplied linear-transformation result shows that $(\overline X,D_2,\ldots,D_n)$ is jointly [multivariate normal](../../../../../../../multivariate-normal-distribution.md). Its marginal [distributions](../../../../../../../distribution-mathematical-analysis.md) are

$$
\boxed{\overline X\sim N(\mu,\sigma^2/n),\qquad D_j\sim N(0,\sigma^2(1-1/n))\quad(2\leq j\leq n).}
$$

Indeed, $\operatorname{Cov}(X_j,\overline X)=\sigma^2/n$, so

$$
\operatorname{Cov}(\overline X,D_j)=\sigma^2/n-\sigma^2/n=0.
$$

For a jointly [Gaussian vector](../../../../../../../gaussian-random-vector.md), zero cross-covariance between blocks implies their [independence](../../../../../../../independent-random-variables.md). Thus $\overline X$ is independent of the entire vector $(D_2,\ldots,D_n)$, not merely of each coordinate separately. The residual coordinates themselves need not be independent: for $j\ne k$, their [covariance](../../../../../../../covariance.md) is $-\sigma^2/n$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
