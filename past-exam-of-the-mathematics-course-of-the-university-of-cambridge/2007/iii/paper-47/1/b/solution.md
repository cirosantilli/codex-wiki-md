<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Transform each observation to $Y_j=A^TX_j$. If $A^T$ has full row [rank](../../../../../../rank-one-quadratic-form.md) $m$, the transformed sample is [multivariate normal](../../../../../../multivariate-normal-distribution.md) with mean $A^T\mu$ and [positive-definite](../../../../../../positive-definite-bilinear-form.md) [covariance matrix](../../../../../../covariance-matrix.md) $A^T\Sigma A$. Its [sample mean](../../../../../../sample-mean.md) is $A^T\bar X$ and its unbiased [sample covariance matrix](../../../../../../sample-covariance-matrix.md) is $A^TSA$. The [Hotelling test of linear hypotheses](../../../../../../hotelling-test-of-linear-hypotheses.md) therefore uses

$$
\boxed{T_A^2=n(A^T\bar X)^T(A^TSA)^{-1}(A^T\bar X),\qquad
\frac{n-m}{m(n-1)}T_A^2\sim F_{m,n-m}\text{ under }H_0.}
$$

Here $n>m$ is required. Reject for a large scaled statistic using the relevant upper [F-distribution](../../../../../../f-distribution.md) quantile. If the rows of $A^T$ are dependent, choose a basis for their row space, use that basis as the contrast matrix, and replace $m$ by its [rank](../../../../../../rank-one-quadratic-form.md) $r$. The null hypothesis is unchanged, but redundant contrasts must not be treated as independent dimensions. [Rank](../../../../../../rank-one-quadratic-form.md) zero gives no restrictions and hence no nontrivial test.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
