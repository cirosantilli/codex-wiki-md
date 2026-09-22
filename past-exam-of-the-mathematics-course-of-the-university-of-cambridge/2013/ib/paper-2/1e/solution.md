<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

Write $U^*=\overline U^T$ for the [conjugate transpose](../../../../../conjugate-transpose.md). Taking [determinants](../../../../../determinant.md) in $U^*AU=A$ gives $|\det U|^2\det A=\det A$. Since the [Hermitian matrix](../../../../../hermitian-operator.md) $A$ is invertible, **every such $U$ is invertible and $|\det U|=1$.** The identity belongs to $U_A$; if $U,V\in U_A$, then $(UV)^*A(UV)=V^*AV=A$; and multiplying $U^*AU=A$ by $(U^*)^{-1}$ and $U^{-1}$ gives $(U^{-1})^*AU^{-1}=A$. Associativity comes from [matrix multiplication](../../../../../matrix-multiplication.md), so this is a [group](../../../../../group-split.md).

The [Hermitian form](../../../../../hermitian-form.md) $h_A(v,w)=v^*Aw$ obeys $h_A(Uv,Uw)=h_A(v,w)$ precisely when $U\in U_A$. Thus **$U_A$ is the group of linear isometries of this nondegenerate [Hermitian form](../../../../../hermitian-form.md)**; positivity of $A$ is unnecessary.

For $A=I$, $U$ is a [unitary matrix](../../../../../unitary-matrix.md). Here is a direct [diagonalization of a matrix](../../../../../diagonalization-of-a-matrix.md) proof. Over $\mathbb C$, its [characteristic polynomial](../../../../../characteristic-polynomial.md) has a root, giving a unit [eigenvector](../../../../../eigenvector.md) $v$ with $Uv=\lambda v$. Preservation of the [inner product](../../../../../inner-product.md) gives $|\lambda|=1$. If $w\perp v$, then $\langle Uw,Uv\rangle=\langle w,v\rangle=0$, so $v^\perp$ is invariant. The restriction is again a [unitary matrix](../../../../../unitary-matrix.md). Induction on the [dimension](../../../../../dimension-vector-space.md) supplies an [orthonormal basis](../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../eigenvector.md). In that [basis](../../../../../basis.md), **$U$ is diagonal, with diagonal entries on the unit [circle](../../../../../circle.md)**.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
