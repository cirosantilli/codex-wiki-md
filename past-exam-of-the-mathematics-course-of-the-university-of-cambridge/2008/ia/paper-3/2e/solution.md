<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

The real [orthogonal group](../../../../../orthogonal-group.md) and [special orthogonal group](../../../../../special-orthogonal-group.md) are, under [matrix](../../../../../matrix.md) multiplication,

$$
\boxed{O(n)=\{Q\in M_n(\mathbb R):Q^TQ=I\},\qquad
SO(n)=\{Q\in O(n):\det Q=1\}.}
$$

An [orthogonal matrix](../../../../../orthogonal-matrix.md) preserves Euclidean [inner products](../../../../../inner-product.md); taking [determinants](../../../../../determinant.md) of $Q^TQ=I$ shows that its [determinant](../../../../../determinant.md) is $1$ or $-1$. Its inverse is $Q^T$, so $QQ^T=I$ as well.

For $Q\in SO(3)$, use $Q-I=Q(I-Q^T)$. The [determinant](../../../../../determinant.md) then satisfies

$$
\det(Q-I)=\det Q\det(I-Q^T)=\det(I-Q)=(-1)^3\det(Q-I).
$$

It follows that $\det(Q-I)=0$. Thus the real [matrix](../../../../../matrix.md) $Q-I$ has a nonzero [vector](../../../../../vector.md) in its [kernel of a linear map](../../../../../kernel-of-a-linear-map.md), yielding

$$
\boxed{Qv=v\quad\text{for some }v\ne0.}
$$

This is the three-dimensional case of [odd-dimensional special orthogonal transformation has a fixed vector](../../../../../odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector.md); geometrically it supplies the fixed [rotation](../../../../../rotation-mathematics.md) axis, unless the transformation is the identity and every direction is fixed.

The claim is **false for $O(3)$**. The [matrix](../../../../../matrix.md) $Q=-I_3$ is orthogonal with [determinant](../../../../../determinant.md) $-1$ and has only the [eigenvalue](../../../../../eigenvalue.md) $-1$. It therefore has no nonzero [eigenvector](../../../../../eigenvector.md) with [eigenvalue](../../../../../eigenvalue.md) $1$.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
