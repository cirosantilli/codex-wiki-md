<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the divisor-$n$ [sample covariance matrix](../../../../../../sample-covariance-matrix.md), since this is the normalization that enters the [multivariate normal](../../../../../../multivariate-normal-distribution.md) [likelihood function](../../../../../../likelihood-function.md):

$$
\bar x=\frac1n\sum_{j=1}^n x_j,\qquad
S=\frac1n\sum_{j=1}^n(x_j-\bar x)(x_j-\bar x)^T.
$$

For a [covariance matrix](../../../../../../covariance-matrix.md) that is a [positive-definite matrix](../../../../../../positive-definite-matrix.md) $V$, the product of the [multivariate normal densities](../../../../../../multivariate-normal-density.md) gives

$$
-2\ell(\mu,V)=np\log(2\pi)+n\log|V|+
\sum_{j=1}^n(x_j-\mu)^TV^{-1}(x_j-\mu).
$$

To separate the [sample mean](../../../../../../sample-mean.md) from the [sample covariance matrix](../../../../../../sample-covariance-matrix.md), expand $x_j-\mu=(x_j-\bar x)+(\bar x-\mu)$. The cross terms sum to zero because $\sum_j(x_j-\bar x)=0$. Also $u^TV^{-1}u=\operatorname{tr}(V^{-1}uu^T)$ by the [trace](../../../../../../matrix-trace.md) identity. Therefore

$$
\boxed{-2\ell(\mu,V)=np\log(2\pi)+n\log|V|+
 n\operatorname{tr}(V^{-1}S)+n(\bar x-\mu)^TV^{-1}(\bar x-\mu).}
$$

The printed expression suppresses the parameter-independent constant $np\log(2\pi)$; dropping this constant has no effect on [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) or the [likelihood-ratio test](../../../../../../likelihood-ratio-test.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
