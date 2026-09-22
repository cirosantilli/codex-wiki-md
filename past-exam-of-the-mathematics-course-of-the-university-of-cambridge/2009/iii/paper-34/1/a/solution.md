<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For every nonzero $v\in\mathbb R^{n-p}$, full column rank of $L$ gives $Lv\ne0$, and hence

$$
v^TL^TLv=\|Lv\|^2>0.
$$

Thus the [Gram matrix](../../../../../../gram-matrix.md) $L^TL$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md) and is invertible. Using $BA=0$ and $A=LL^T$,

$$
0=BLL^TL(L^TL)^{-1}=BL,
$$

so

$$
\boxed{L^TL\text{ is positive definite},\qquad BL=0.}
$$

A [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md) is again multivariate normal. Therefore the stacked vector has mean $(B\mu,L^T\mu)^T$ and [covariance](../../../../../../covariance.md)

$$
\sigma^2\begin{pmatrix}BB^T&BL\\L^TB^T&L^TL\end{pmatrix}=\sigma^2\begin{pmatrix}BB^T&0\\0&L^TL\end{pmatrix}.
$$

In particular,

$$
\boxed{Z\sim N_n\!\left(\begin{pmatrix}B\mu\\L^T\mu\end{pmatrix},\ \sigma^2\begin{pmatrix}BB^T&0\\0&L^TL\end{pmatrix}\right).}
$$

The two diagonal blocks are [positive-definite](../../../../../../positive-definite-bilinear-form.md) by the rank assumptions. The two blocks are jointly Gaussian and have zero cross [covariance](../../../../../../covariance.md). The fact that [uncorrelated jointly Gaussian variables are independent](../../../../../../uncorrelated-jointly-normal-variables-are-independent.md) makes $BY$ and $L^TY$ independent. Since

$$
Y^TAY=Y^TLL^TY=\|L^TY\|^2
$$

is a measurable function of the second block, independence is preserved under this transformation. This proves [Gaussian independence of linear and quadratic statistics](../../../../../../gaussian-independence-of-linear-and-quadratic-statistics.md):

$$
\boxed{BY\text{ and }Y^TAY\text{ are independent}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
