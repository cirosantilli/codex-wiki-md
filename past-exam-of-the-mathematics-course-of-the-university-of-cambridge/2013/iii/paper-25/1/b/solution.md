<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For any $r_1,\ldots,r_n\in\mathbb R$, the linearity from part (a) gives

$$
\sum_{j=1}^n r_jX(h_j)=X\left(\sum_{j=1}^n r_jh_j\right)
$$

almost surely, and the right side has a [normal distribution](../../../../../../normal-distribution.md). This is the defining linear-combination criterion for a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md); singular [covariance matrices](../../../../../../covariance-matrix.md) are allowed.

Passing to the limit in the inner products of the partial sums gives

$$
\boxed{\operatorname{Cov}(X(g),X(h))=\mathbb E[X(g)X(h)]=\sum_j\langle g,e_j\rangle\langle h,e_j\rangle=\langle g,h\rangle.}
$$

The passage to the limit is justified by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and $L^2$ convergence. Equivalently, the vector's [characteristic function](../../../../../../characteristic-function.md) is

$$
\mathbb E\exp\left(i\sum_jr_jX(h_j)\right)=\exp\left(-\frac12\sum_{j,k}r_jr_k\langle h_j,h_k\rangle\right).
$$

Thus both joint normality and the complete [covariance matrix](../../../../../../covariance-matrix.md) follow from the Hilbert-space inner product.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
