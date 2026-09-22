<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since every $u_{jj}>0$, the [diagonal matrix](../../../../diagonal-matrix.md) $D$ is invertible. Set

$$
\widehat U=D^{-1}U,\qquad
\widehat u_{ij}=\frac{u_{ij}}{u_{ii}}.
$$

The division is by the diagonal entry of row $i$. Thus $\widehat U$ is an [upper triangular matrix](../../../../upper-triangular-matrix.md) with diagonal entries one and $A=LD\widehat U$.

To use symmetry without assuming the conclusion, multiply by the [matrix inverse](../../../../matrix-inverse-split.md) of $L$ and its [transpose](../../../../transpose.md):

$$
M=L^{-1}AL^{-T}=D\widehat U L^{-T}.
$$

The [matrix](../../../../matrix.md) $M$ is symmetric because $A$ is a [symmetric matrix](../../../../symmetric-matrix.md). It is also an [upper triangular matrix](../../../../upper-triangular-matrix.md), since every factor on the right is an [upper triangular matrix](../../../../upper-triangular-matrix.md). A symmetric [upper triangular matrix](../../../../upper-triangular-matrix.md) is diagonal. Its diagonal is exactly $D$, because $\widehat U$ and $L^{-T}$ have diagonal entries one. Hence $M=D$, giving

$$
\boxed{A=LDL^T,\qquad \widehat U=L^T.}
$$

This is the [LDL decomposition](../../../../ldl-decomposition.md).

Take the positive [square roots](../../../../square-root.md) of the diagonal entries:

$$
D^{1/2}=\operatorname{diag}(\sqrt{u_{11}},\ldots,\sqrt{u_{nn}}),\qquad
\widehat L=LD^{1/2}.
$$

The [matrix](../../../../matrix.md) $\widehat L$ is a [lower triangular matrix](../../../../lower-triangular-matrix.md) with positive diagonal, and

$$
\boxed{A=\widehat L\widehat L^T.}
$$

This is a [Cholesky decomposition](../../../../cholesky-decomposition.md). For a nonzero [vector](../../../../vector.md) $x$, the [vector](../../../../vector.md) $\widehat L^Tx$ is nonzero because $\widehat L^T$ is invertible. Therefore

$$
\boxed{x^TAx=(\widehat L^Tx)^T(\widehat L^Tx)=\|\widehat L^Tx\|_2^2>0.}
$$

Here $\|\cdot\|_2$ is the [Euclidean norm](../../../../euclidean-norm.md). Thus $A$ is a [positive-definite matrix](../../../../positive-definite-matrix.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
