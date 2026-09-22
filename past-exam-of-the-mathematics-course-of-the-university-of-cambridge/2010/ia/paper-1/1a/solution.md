<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

Define the [change-of-basis matrices](../../../../../change-of-basis-matrix.md) by expressing each new [basis vector](../../../../../basis-vector.md) in the corresponding old [basis](../../../../../basis.md):

$$
\mathbf b'_i=\sum_{k=1}^n B_{ki}\mathbf b_k,
\qquad
\mathbf c'_j=\sum_{\ell=1}^m C_{\ell j}\mathbf c_\ell.
$$

Thus $B$ is $n\times n$, $C$ is $m\times m$, and both are [invertible matrices](../../../../../invertible-matrix.md): a [linear combination](../../../../../linear-combination.md) of their columns is zero exactly when the same combination of the new [basis vectors](../../../../../basis-vector.md) is zero. For any vector $v$, its coordinate columns therefore satisfy $[v]_{\mathbf b}=B[v]_{\mathbf b'}$; likewise $[w]_{\mathbf c}=C[w]_{\mathbf c'}$.

The [matrix representation of a linear map](../../../../../matrix-representation-of-a-linear-map.md) gives

$$
C[\Phi(v)]_{\mathbf c'}=[\Phi(v)]_{\mathbf c}
=A[v]_{\mathbf b}=AB[v]_{\mathbf b'}.
$$

Multiplying by the [matrix inverse](../../../../../matrix-inverse.md) of $C$ and comparing with $[\Phi(v)]_{\mathbf c'}=A'[v]_{\mathbf b'}$ for every $v$ proves

$$
\boxed{A'=C^{-1}AB.}
$$

The domain [change of basis](../../../../../change-of-basis.md) acts on the right, while the codomain [change of basis](../../../../../change-of-basis.md) acts on the left through its inverse.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
