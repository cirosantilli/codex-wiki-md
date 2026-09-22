# Similarity and the coordinate metric

↑ **Parent:** [Similarity transformation](similarity-transformation.md)

For real [matrices](matrix.md), [orthogonal similarity](orthogonal-similarity.md) is the special case $B=Q^{-1}AQ=Q^TAQ$ with $Q$ an [orthogonal matrix](orthogonal-matrix.md). Then a [symmetric matrix](symmetric-matrix.md) remains symmetric, because $B^T=Q^TA^TQ=B$. The expression $QAQ^T$ describes the reverse conversion and has the same property. An [orthonormal basis](orthonormal-basis.md) retains the ordinary [dot product](dot-product.md) formula for its [coordinate vectors](coordinate-vector.md).

An arbitrary [change of basis](change-of-basis.md) need not preserve entrywise symmetry. In the opening example, $A$ is a [symmetric matrix](symmetric-matrix.md) but $B=\begin{pmatrix}2&-3\\0&5\end{pmatrix}$ is not. The geometric [inner product](inner-product-split.md) has not disappeared: in the new [coordinates](coordinate-linear-algebra.md) it is represented by the [Gram matrix](gram-matrix.md)

$$
G=S^TS=\begin{pmatrix}1&1\\1&2\end{pmatrix},\qquad
(Sy)^T(Sz)=y^TGz.
$$

For $p$ with new [coordinate vector](coordinate-vector.md) $y=(1,1)^T$, the squared [Euclidean norm](euclidean-norm.md) is $y^TGy=5$, agreeing with $x^Tx=2^2+1^2$. The naive coordinate sum $y^Ty=2$ would use the wrong [inner product](inner-product-split.md).

If $A^T=A$, direct multiplication gives

$$
B^TG=GB=S^TAS.
$$

This is [self-adjointness](self-adjoint-operator.md) expressed in the new [inner product](inner-product-split.md), rather than entrywise symmetry relative to the [identity matrix](identity-matrix.md). For the example, both products equal $\begin{pmatrix}2&2\\2&7\end{pmatrix}$. Thus arbitrary [matrix similarity](matrix-similarity.md) preserves the [linear operator](linear-operator.md), while its geometric interpretation requires transforming the [Gram matrix](gram-matrix.md) as well. [Matrix congruence](matrix-congruence.md) supplies the corresponding rule for a [bilinear form](bilinear-form-split.md) and should be distinguished from [matrix similarity](matrix-similarity.md).

## ↑ Ancestors (7)

1. [Similarity transformation](similarity-transformation.md)
2. [Matrix similarity](matrix-similarity.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
