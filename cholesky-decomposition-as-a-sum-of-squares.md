# Cholesky decomposition as a sum of squares

↑ **Parent:** [Cholesky decomposition](cholesky-decomposition.md)

For any real [vector](vector.md) $u$, a [Cholesky decomposition](cholesky-decomposition.md) gives the [quadratic form](quadratic-form-split.md) identity

$$
u^TAu=u^TLL^Tu=(L^Tu)^T(L^Tu)=\|L^Tu\|_2^2.
$$

Since $L$ is an [invertible matrix](invertible-matrix.md), this [squared Euclidean norm](squared-euclidean-norm.md) is positive whenever $u\ne0$. The factorization thus certifies [positive definiteness](positive-definiteness.md) and gives coordinates in which the [quadratic form](quadratic-form-split.md) is a sum of ordinary squares. For the matrix above,

$$
4u_1^2+4u_1u_2+5u_2^2=(2u_1+u_2)^2+(2u_2)^2.
$$

The [level set](level-set.md) $u^TAu=1$ is an [ellipse](ellipse.md); the [linear map](linear-map.md) $z=L^Tu$ sends it to the [unit circle](complex-unit-circle.md). The points $u=(1/2,0)^T$ and $u=(-1/4,1/2)^T$ go to $(1,0)^T$ and $(0,1)^T$, respectively.

<a id="image-a-cholesky-decomposition-turns-a-positive-quadratic-form-into-a-squared-euclidean-norm"></a>
![](cholesky-quadratic-ellipse-to-circle.png)

**[Figure 2](#image-a-cholesky-decomposition-turns-a-positive-quadratic-form-into-a-squared-euclidean-norm). A Cholesky decomposition turns a positive quadratic form into a squared Euclidean norm**. Original exact [ellipse](ellipse.md) and its image under $z=L^Tu$. Matching point colors show two mapped points; the axes use their own coordinates. This transformation need not be a [rotation](rotation-mathematics.md) or a uniform scaling.

The same factor works in the reverse direction for [Gaussian random vectors](gaussian-random-vector.md). If $Z$ has [independent](independent-random-variables.md) unit-[variance](variance-split.md), zero-[mean](expected-value-split.md) [Gaussian random variables](gaussian-random-variable.md) as coordinates, $X=LZ$ has [covariance matrix](covariance-matrix.md) $LL^T=A$. In this example $X_1=2Z_1$ and $X_2=Z_1+2Z_2$: their [variances](variance-split.md) are $4$ and $5$, while their [covariance](covariance.md) is $2$. This is a concrete way to generate specified correlations from independent draws.

A triangular factor is not generally a [square root of a matrix](square-root-of-a-matrix.md) in the sense $B^2=A$. Here $L^2=\begin{pmatrix}4&0\\4&4\end{pmatrix}\ne A$. The [Cholesky decomposition](cholesky-decomposition.md) uses the product with the [transpose](transpose.md), which is also what makes the [quadratic form](quadratic-form-split.md) a [squared Euclidean norm](squared-euclidean-norm.md).

## ↑ Ancestors (9)

1. [Cholesky decomposition](cholesky-decomposition.md)
2. [Positive-definite matrix](positive-definite-matrix.md)
3. [Definite matrix](definite-matrix.md)
4. [Quadratic form](quadratic-form-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
