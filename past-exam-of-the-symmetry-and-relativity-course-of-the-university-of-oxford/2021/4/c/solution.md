<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The supplied [matrix](../../../../matrix.md) obeys

$$
J_3^2=\operatorname{diag}(1,1,0),\qquad J_3^3=J_3.
$$

Separate the even and odd powers in the [matrix exponential](../../../../matrix-exponential.md) to obtain

$$
\boxed{e^{-i\theta J_3}=I-i\sin\theta J_3+(\cos\theta-1)J_3^2
=\begin{pmatrix}\cos\theta&-\sin\theta&0\\\sin\theta&\cos\theta&0\\0&0&1\end{pmatrix}.}
$$

It fixes the $z$ component and is a counterclockwise active [rotation](../../../../rotation-mathematics.md) viewed from $+z$. This sign differs from the clockwise convention in [b](../b.md), because the source fixes the sign of both $J_3$ and the exponential. Replacing $\theta$ by $-\theta$ yields the clockwise [rotation](../../../../rotation-mathematics.md).

With $(J_k)_{ij}=-i\epsilon_{kij}$, the [generators of rotations](../../../../rotation-generator.md) obey

$$
\boxed{[J_i,J_j]=i\epsilon_{ijk}J_k.}
$$

The [commutator](../../../../commutator.md) measures the leading difference between performing two infinitesimal [rotations](../../../../rotation-mathematics.md) in opposite orders. For example, with $X=-i\alpha J_1$ and $Y=-i\beta J_2$,

$$
e^Xe^Ye^{-X}e^{-Y}=I+[X,Y]+O(\alpha^2\beta,\alpha\beta^2)
=I-i\alpha\beta J_3+O(\alpha^2\beta,\alpha\beta^2).
$$

The failure to commute is itself an infinitesimal [rotation](../../../../rotation-mathematics.md) about the perpendicular axis; the [Lie algebra](../../../../lie-algebra-split.md) closes on the same three [generators of rotations](../../../../rotation-generator.md).

To pass from this local statement to the full [group](../../../../group-split.md) property, put $A_k=-iJ_k$. These are real antisymmetric [matrices](../../../../matrix.md), with $[A_i,A_j]=\epsilon_{ijk}A_k$. The [Baker--Campbell--Hausdorff formula](../../../../baker-campbell-hausdorff-formula.md) shows locally that the logarithm of a product of their exponentials remains a linear combination of the $A_k$, because all nested [commutators](../../../../commutator.md) do. Globally, each exponential has $R^TR=I$ and $\det R=e^{\operatorname{tr}A}=1$. If $R_1,R_2$ have these properties, then

$$
(R_1R_2)^T(R_1R_2)=R_2^TR_2=I,\qquad \det(R_1R_2)=1.
$$

Every real three-dimensional [orthogonal matrix](../../../../orthogonal-matrix.md) of [determinant](../../../../determinant.md) $+1$ has an eigenvector with [eigenvalue](../../../../eigenvalue.md) $+1$: its nonreal [eigenvalues](../../../../eigenvalue.md) come in conjugate pairs, and the product of all three is $+1$. On the perpendicular plane it acts as a two-dimensional [rotation](../../../../rotation-mathematics.md). It therefore has axis-angle form and can be written $e^{-i\theta\hat n^kJ_k}$. Thus the product is again a [rotation](../../../../rotation-mathematics.md). The identity is $\theta=0$, the inverse reverses $\theta$, and associativity comes from [matrix multiplication](../../../../matrix-multiplication.md). This proves that all these [rotations](../../../../rotation-mathematics.md) form the [special orthogonal group](../../../../special-orthogonal-group.md) $SO(3)$. The [commutator](../../../../commutator.md) supplies local closure, while the orthogonality and axis-angle argument supplies the necessary global step.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
