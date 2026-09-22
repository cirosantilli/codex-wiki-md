<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Let $T$ be the [isometry](../../../../../isometry.md). Since $T(0)=0$, it preserves [norms](../../../../../norm.md), and the [polarization identity](../../../../../polarization-identity.md) applied to distances gives $\langle T(x),T(y)\rangle=\langle x,y\rangle$. For an [orthonormal basis](../../../../../orthonormal-basis.md) $e_1,e_2,e_3$, the vectors $T(e_i)$ are again an [orthonormal basis](../../../../../orthonormal-basis.md), and

$$
\langle T(x),T(e_i)\rangle=\langle x,e_i\rangle.
$$

Expanding in that [basis](../../../../../basis.md) proves $T(x)=\sum_i\langle x,e_i\rangle T(e_i)$. Hence $T$ is a [linear map](../../../../../linear-map.md) represented by an [orthogonal matrix](../../../../../orthogonal-matrix.md) $Q$.

A [reflection in a hyperplane](../../../../../reflection-in-a-hyperplane.md) with nonzero normal $v$ is $H_v(x)=x-2\langle x,v\rangle v/\langle v,v\rangle$. If $Qe_1\ne e_1$, choose $v=Qe_1-e_1$. Because $\|Qe_1\|=\|e_1\|$, substitution shows $H_vQe_1=e_1$. If they agree, no [reflection](../../../../../reflection-mathematics.md) is needed. The resulting [orthogonal transformation](../../../../../orthogonal-transformation.md) fixes $e_1$ and preserves its [orthogonal complement](../../../../../orthogonal-complement.md). Apply the same construction there to fix $e_2$; the second normal is perpendicular to $e_1$, so the first vector remains fixed. Finally the restriction to the remaining line is either the identity or negation; in the latter case a third [reflection](../../../../../reflection-mathematics.md), normal to $e_3$, fixes it. Reversing these steps writes $Q$ as a product of at most three [reflections](../../../../../reflection-mathematics.md), each in a plane through the origin. This proves the three-dimensional case of the [Cartan–Dieudonné theorem](../../../../../cartan-dieudonne-theorem.md).

**Three reflections are sometimes necessary.** The map $-I$ is the product of the three coordinate-plane [reflections](../../../../../reflection-mathematics.md). Its [determinant](../../../../../determinant.md) is $-1$, excluding zero or two [reflections](../../../../../reflection-mathematics.md). A single plane [reflection](../../../../../reflection-mathematics.md) fixes a two-dimensional [vector subspace](../../../../../vector-subspace.md), whereas $-I$ fixes only zero, excluding one. Thus the bound is sharp.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
