<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

An [eigenvalue](../../../../../eigenvalue.md) of a [matrix](../../../../../matrix.md) $A$ is a [scalar](../../../../../scalar.md) $\lambda$ for which $Av=\lambda v$ for some nonzero [eigenvector](../../../../../eigenvector.md) $v$. Its corresponding [eigenspace](../../../../../eigenspace.md) is

$$
E_\lambda=\ker(A-\lambda I).
$$

Write $v=(a,b,c,d)^T$. The displayed matrix is the [outer product](../../../../../outer-product.md) $A=vv^T$, so

$$
Ax=v(v^Tx)=v(v\mathbin{\cdot}x).
$$

Its [column space](../../../../../column-space.md) is contained in $\operatorname{span}\{v\}$ and is nonzero because $Av=\lVert v\rVert^2v\ne0$. Hence $A$ is a [rank-one matrix](../../../../../rank-one-matrix.md).

The vector $v$ is an eigenvector with eigenvalue $\lVert v\rVert^2=a^2+b^2+c^2+d^2$, and every vector in the [orthogonal complement](../../../../../orthogonal-complement.md) $v^\perp$ has eigenvalue $0$. Thus

$$
E_{\lVert v\rVert^2}=\operatorname{span}\{v\},
\qquad E_0=v^\perp.
$$

Since $\mathbb R^4=\operatorname{span}\{v\}\oplus v^\perp$ is a [direct sum](../../../../../direct-sum.md) of these eigenspaces, $A$ has an [eigenbasis](../../../../../eigenbasis.md) and is therefore a [diagonalizable](../../../../../diagonalizable-matrix.md).

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
