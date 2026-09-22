<h1 id="30k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Condition on the information available before time $n$. The current wealth is then fixed, while $\xi_n\sim N(b,\Sigma)$ is independent of that information. Put

$$
B=b^T\Sigma^{-1}b>0.
$$

For any portfolio $\theta$, use the [inner product](../../../../../../inner-product.md) induced by the [positive-definite matrix](../../../../../../positive-definite-matrix.md) $\Sigma$ to write

$$
\theta=\lambda\Sigma^{-1}b+\eta,
\qquad
\lambda=\frac{\theta^Tb}{B},
\qquad
\eta^Tb=0.
$$

The [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md) shows that the two portfolio returns are jointly normal, and

$$
\operatorname{cov}\left((\lambda\Sigma^{-1}b)^T\xi_n,\eta^T\xi_n\right)
=\lambda\eta^T\Sigma\Sigma^{-1}b
=\lambda\eta^Tb=0.
$$

Thus [independence of uncorrelated jointly normal variables](../../../../../../independence-of-uncorrelated-jointly-normal-variables.md) makes the residual return $\eta^T\xi_n$ independent of the aligned return; it also has [expected value](../../../../../../expected-value.md) zero.

The continuation value $V(n,\cdot)$ is concave by part (c). Conditional [Jensen inequality](../../../../../../jensen-s-inequality.md) therefore shows that adding the independent centered residual cannot improve the objective:

$$
\mathbb E\left[V\left(n,m+(\lambda\Sigma^{-1}b)^T\xi_n+\eta^T\xi_n\right)\right]
\leq
\mathbb E\left[V\left(n,m+(\lambda\Sigma^{-1}b)^T\xi_n\right)\right],
$$

where $m=(1+r)X_{n-1}$. Since the optimal portfolio is unique, its residual must be zero.

It remains to determine the sign. If $\lambda<0$, the portfolios $\lambda\Sigma^{-1}b$ and $-\lambda\Sigma^{-1}b$ have the same return [variance](../../../../../../variance-split.md), namely $\lambda^2B$, while their means are $\lambda B$ and $-\lambda B$. The latter return has the distribution of the former plus the positive constant $-2\lambda B$. Since $V(n,\cdot)$ is increasing, replacing $\lambda$ by $-\lambda$ cannot reduce the objective, contradicting uniqueness. Hence $\lambda\geq0$.

Applying this conditional argument at every time gives nonnegative, past-measurable random variables $\lambda_n$ such that

$$
\boxed{\theta_n^*=\lambda_n\Sigma^{-1}b},
\qquad 1\leq n\leq N.
$$

This is the [Gaussian one-fund theorem](../../../../../../gaussian-one-fund-theorem.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
