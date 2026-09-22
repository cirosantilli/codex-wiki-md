# Adjoint in weighted coordinates

↑ **Parent:** [Adjoint operator](adjoint-operator.md)

Suppose a [linear map](linear-map.md) between finite-dimensional [Hilbert spaces](hilbert-space-split.md) has [matrix](matrix.md) $A$, and their [inner products](inner-product-split.md) in the chosen [bases](basis.md) are $\langle x,z\rangle_H=z^*G_Hx$ and $\langle u,v\rangle_K=v^*G_Ku$. The [Gram matrices](gram-matrix.md) $G_H,G_K$ are [positive-definite matrices](positive-definite-matrix.md). Writing $A^*=\overline A^{\mathrm T}$ for the ordinary [conjugate transpose](conjugate-transpose.md), the coordinate [matrix](matrix.md) of the [adjoint operator](adjoint-operator.md) is

$$
[T^*]=G_H^{-1}A^*G_K.
$$

Indeed, the defining [inner product](inner-product-split.md) identity says $y^*G_KAx=y^*[T^*]^*G_Hx$ for all $x,y$. Thus simply transposing and conjugating is valid in [orthonormal bases](orthonormal-basis.md), where both [Gram matrices](gram-matrix.md) are the [identity matrix](identity-matrix.md).

For the [weighted inner product](weighted-inner-product.md) $\langle x,y\rangle_G=\overline{y_1}x_1+4\overline{y_2}x_2$ and the coordinate swap $A=\begin{pmatrix}0&1\\1&0\end{pmatrix}$, the [adjoint operator](adjoint-operator.md) has [matrix](matrix.md) $\begin{pmatrix}0&4\\1/4&0\end{pmatrix}$. With $x=(1,0)^{\mathrm T}$ and $y=(0,1)^{\mathrm T}$, both [inner products](inner-product-split.md) equal $4$. The coordinate swap is its own ordinary [transpose](transpose.md), but is not [self-adjoint](self-adjoint-operator.md) in this [weighted inner product](weighted-inner-product.md).

## ↑ Ancestors (8)

1. [Adjoint operator](adjoint-operator.md)
2. [Riesz representation theorem](riesz-representation-theorem.md)
3. [Hilbert space](hilbert-space-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
