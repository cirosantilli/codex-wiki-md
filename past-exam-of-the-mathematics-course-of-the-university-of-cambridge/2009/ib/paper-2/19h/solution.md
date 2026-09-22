<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

A random [vector](../../../../../vector.md) $X$ has [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) $N_d(\mu,\Sigma)$ if every real linear combination $t^TX$ is normally distributed, with mean $t^T\mu$ and variance $t^T\Sigma t$. The [covariance matrix](../../../../../covariance-matrix.md) is symmetric positive semidefinite; zero variances permit degenerate normals. Its [moment-generating function](../../../../../moment-generating-function.md) is $M_X(t)=\exp(t^T\mu+t^T\Sigma t/2)$, including the degenerate cases.

For the given $X$, let $t_j\in\mathbb R^{d_j}$. The joint [moment-generating function](../../../../../moment-generating-function.md) of the $Y_j=A_jX$ is

$$
\begin{aligned}
\mathbb E\exp\left(\sum_jt_j^TY_j\right)
&=M_X\left(\sum_jA_j^Tt_j\right)\\
&=\exp\left[\frac{\sigma^2}{2}\sum_{i,j}t_j^TA_jA_i^Tt_i\right]\\
&=\prod_j\exp\left[\frac{\sigma^2}{2}t_j^TA_jA_j^Tt_j\right].
\end{aligned}
$$

The last equality uses the assumed orthogonality of the row spaces. Its factors are exactly the individual [moment-generating functions](../../../../../moment-generating-function.md), so the hint implies **the random [vectors](../../../../../vector.md) $Y_j$ are independent**. Also every linear combination of the stacked [vector](../../../../../vector.md) $Y$ is a linear combination of $X$, hence normally distributed. Consequently

$$
\boxed{Y\sim N_{\sum_jd_j}\left(0,\operatorname{diag}(\sigma^2A_1A_1^T,\ldots,\sigma^2A_JA_J^T)\right).}
$$

This establishes both claims without excluding singular block covariances.

For the [sample mean](../../../../../sample-mean.md) and [sample variance](../../../../../sample-variance.md) result, assume $n\ge2$ and set $W=(Z_1-\mu,\ldots,Z_n-\mu)^T$. Independence of the observations gives $W\sim N_n(0,\sigma^2I)$. Let $u=(1,\ldots,1)^T$, $A_1=u^T/n$, and $A_2=I-uu^T/n$. Then $A_1A_2^T=0$. The first transformed [vector](../../../../../vector.md) is the scalar $\overline Z-\mu$, and the second is the residual [vector](../../../../../vector.md) $(Z_i-\overline Z)_i$. They are independent by the just-proved result. Applying the measurable function $v\mapsto\|v\|^2/(n-1)$ to the residual [vector](../../../../../vector.md) preserves independence from the [sample mean](../../../../../sample-mean.md). Thus

$$
\boxed{\overline Z\ \text{and}\ S_{ZZ}\ \text{are independent}.}
$$

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
