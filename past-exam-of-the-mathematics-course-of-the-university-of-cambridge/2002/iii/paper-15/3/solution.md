<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the natural [linearization of a line bundle](../../../../../linearization-of-a-line-bundle.md) on $\mathcal O_X(1)$ induced by the conjugation representation on $M_n\mathbb C$. The notation involving the dual does not change this matrix description: the nondegenerate pairing $(A,B)\mapsto\operatorname{tr}(AB)$ identifies the representation with its dual equivariantly. Let $[A]$ be a projective point, so $A\ne0$.

The [Hilbert-Mumford criterion for projective stability](../../../../../hilbert-mumford-criterion-for-projective-stability.md) says that $[A]$ is not a [semistable projective point in geometric invariant theory](../../../../../semistable-projective-point-in-geometric-invariant-theory.md) precisely when some [algebraic one-parameter subgroup](../../../../../algebraic-one-parameter-subgroup.md) $\lambda:\mathbb G_m\to SL_n$ sends its affine representative to zero:

$$
\lim_{t\to0}\lambda(t)A\lambda(t)^{-1}=0.
$$

Equivalently, all active weights for that subgroup are strictly positive. With the convention $\mu([A],\lambda)=-\min\{\text{active weights}\}$, semistability requires $\mu\ge0$ for every subgroup, including conjugates of diagonal ones.

Suppose such a zero limit exists. The coefficients $c_j(A)$ in

$$
\det(TI-A)=T^n+c_1(A)T^{n-1}+\cdots+c_n(A)
$$

are invariant under conjugation. Continuity along the zero limit gives $c_j(A)=c_j(0)=0$ for every $j$. By the [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md), $A^n=0$: the matrix is [nilpotent](../../../../../nilpotent.md).

Conversely, if $A$ is a nonzero [nilpotent matrix](../../../../../nilpotent-matrix.md), choose a basis in which it is strictly upper triangular, for example a [Jordan normal form](../../../../../jordan-normal-form.md). The change of basis can be chosen in $SL_n$: multiply any invertible change-of-basis matrix by a scalar with the required $n$th power, which does not affect its conjugation. In this basis take

$$
\lambda(t)=\operatorname{diag}(t^{n-1},t^{n-3},\ldots,t^{1-n}).
$$

The exponents sum to zero, so this is an [algebraic one-parameter subgroup](../../../../../algebraic-one-parameter-subgroup.md) of the [special linear group](../../../../../special-linear-group.md). The $(i,j)$ matrix entry has weight

$$
(n+1-2i)-(n+1-2j)=2(j-i).
$$

Every potentially nonzero entry has $i<j$ and therefore positive weight. Thus the conjugated matrix tends to zero. Conjugate this subgroup back to the original basis to obtain the required destabilizing subgroup for $A$.

It follows that the [nilpotent cone for conjugation of matrices](../../../../../nilpotent-cone-for-conjugation-of-matrices.md) is exactly the [affine null cone](../../../../../affine-null-cone.md), and

$$
\boxed{X^{ss}=\{[A]:A\text{ is not nilpotent}\}=\bigcup_{j=1}^n\{[A]:c_j(A)\ne0\}.}
$$

Each $c_j$ is a homogeneous invariant of degree $j$, so the second description also gives invariant open sets witnessing semistability. Equivalently, a representative has at least one nonzero eigenvalue. Nonzero singular matrices can be semistable; invertibility is not the criterion. For example, a diagonal matrix with diagonal entries $1,0,\ldots,0$ is semistable, while a nonzero strictly upper triangular matrix is unstable.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
