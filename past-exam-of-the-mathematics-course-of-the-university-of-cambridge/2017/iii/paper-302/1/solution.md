<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The two [Lie groups](../../../../../lie-group.md) have the same local infinitesimal structure, but different global topology. This difference determines which [Lie algebra representations](../../../../../lie-algebra-representation.md) integrate to representations of each group.

An element of the [SU(2) group](../../../../../su-2-group.md) is a [unitary matrix](../../../../../unitary-matrix.md) of [determinant](../../../../../determinant.md) one. Orthogonality of its columns and its [determinant](../../../../../determinant.md) give the unique form

$$
U=\begin{pmatrix}a&b\\-\overline b&\overline a\end{pmatrix},\qquad |a|^2+|b|^2=1.
$$

Thus its [group manifold](../../../../../group-manifold.md) is the unit [three-sphere](../../../../../three-sphere.md) in $\mathbb C^2\simeq\mathbb R^4$: this is [SU(2) as the three-sphere](../../../../../su-2-as-the-three-sphere.md). In particular it is [compact](../../../../../compact-space.md), [connected](../../../../../connected-space.md) and [simply connected](../../../../../simply-connected-space.md). In terms of the [Pauli matrices](../../../../../pauli-matrices.md) one may also write $U=a_0I-i\mathbf a\cdot\boldsymbol\sigma$ with real coefficients satisfying $a_0^2+\mathbf a^2=1$.

Differentiate $U(t)^\dagger U(t)=I$ and $\det U(t)=1$ at $U(0)=I$. The [tangent space](../../../../../tangent-space.md) consists of traceless [skew-Hermitian matrices](../../../../../skew-hermitian-matrix.md):

$$
\mathfrak{su}(2)=\{X\in M_2(\mathbb C):X^\dagger=-X,\ \operatorname{tr}X=0\}.
$$

The [Lie bracket](../../../../../lie-bracket.md) of a [Matrix Lie group](../../../../../matrix-lie-group.md) is the matrix [commutator](../../../../../commutator.md). With $T_a=-i\sigma_a/2$, the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives

$$
[T_a,T_b]=\epsilon_{abc}T_c.
$$

This derives the [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md) as a three-dimensional real [Lie algebra](../../../../../lie-algebra-split.md). The Hermitian physics generators $J_a=\sigma_a/2$ instead obey $[J_a,J_b]=i\epsilon_{abc}J_c$; they are $i$ times the skew-Hermitian tangent generators, so these are consistent conventions.

The [SO(3) group](../../../../../so-3-group.md) consists of real [orthogonal matrices](../../../../../orthogonal-matrix.md) with [determinant](../../../../../determinant.md) one. Differentiating $R(t)^TR(t)=I$ at the identity gives

$$
\mathfrak{so}(3)=\{A\in M_3(\mathbb R):A^T=-A\}.
$$

The [determinant](../../../../../determinant.md) condition gives no additional infinitesimal constraint because a [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md) already has [trace](../../../../../matrix-trace.md) zero. Define $L_a\mathbf v=\mathbf e_a\times\mathbf v$. The [cross product](../../../../../cross-product.md) identity implies

$$
[L_a,L_b]\mathbf v=\mathbf e_a\times(\mathbf e_b\times\mathbf v)-\mathbf e_b\times(\mathbf e_a\times\mathbf v)=\epsilon_{abc}L_c\mathbf v.
$$

Therefore the [SO(3) Lie algebra](../../../../../so-3-lie-algebra.md) has the same [structure constants](../../../../../structure-constant.md) and $T_a\mapsto L_a$ is a [Lie algebra isomorphism](../../../../../lie-algebra-isomorphism.md).

The global relation is the [Adjoint double cover from SU(2) to SO(3)](../../../../../adjoint-double-cover-from-su-2-to-so-3.md). For $V=\mathbf v\cdot\boldsymbol\sigma$, define $R(U)$ by

$$
UVU^{-1}=(R(U)\mathbf v)\cdot\boldsymbol\sigma.
$$

Conjugation preserves the real space of traceless [Hermitian matrices](../../../../../hermitian-operator.md) and its [inner product](../../../../../inner-product.md) $\tfrac12\operatorname{tr}(VW)=\mathbf v\cdot\mathbf w$. Hence $R(U)$ is orthogonal. Continuity and connectedness, together with $R(I)=I$, put it in $SO(3)$. Composition of conjugations makes $R$ a [group homomorphism](../../../../../group-homomorphism.md). If $R(U)=I$, then $U$ commutes with every [Pauli matrix](../../../../../pauli-matrices.md), hence is scalar; unitarity and [determinant](../../../../../determinant.md) one leave precisely $U=\pm I$. The differential sends $T_a$ to $L_a$, so it is an isomorphism. More concretely,

$$
U(\theta,\mathbf n)=\exp\left(-\frac{i\theta}{2}\mathbf n\cdot\boldsymbol\sigma\right)=\cos\frac\theta2\,I-i\sin\frac\theta2\,\mathbf n\cdot\boldsymbol\sigma
$$

induces rotation through angle $\theta$ about $\mathbf n$, by the [Rodrigues rotation formula](../../../../../rodrigues-rotation-formula.md). Every three-dimensional rotation has such an axis and angle, proving surjectivity. Consequently

$$
\boxed{SO(3)\simeq SU(2)/\{\pm I\},\qquad \mathfrak{so}(3)\simeq\mathfrak{su}(2).}
$$

The matrices $U$ and $-U$ are antipodal points on the three-sphere, so the [SO(3) group manifold](../../../../../so-3-as-real-projective-three-space.md) is [Real projective space](../../../../../real-projective-space.md) $\mathbb{RP}^3$. Equivalently, the closed axis-angle ball $\|\theta\mathbf n\|\le\pi$ has opposite boundary points identified. The [fundamental group](../../../../../fundamental-group.md) is $\pi_1(SO(3))\simeq\mathbb Z_2$, whereas $\pi_1(SU(2))=0$. A $2\pi$ rotation lifts from $I$ to $-I$; a $4\pi$ rotation returns to $I$. Thus the covering is the [universal cover](../../../../../universal-cover.md) and the groups are not globally isomorphic.

For [representation theory](../../../../../representation-theory-split.md), specify finite-dimensional complex continuous representations. Compactness permits an invariant [Hermitian inner product](../../../../../hermitian-form.md), obtained by averaging against [Haar measure](../../../../../haar-measure.md), and therefore complete reducibility. Complexifying either real [Lie algebra](../../../../../lie-algebra-split.md) gives the [sl2 Lie algebra](../../../../../sl2-lie-algebra.md). Its finite-dimensional irreducibles are indexed by $n\in\mathbb Z_{\ge0}$, have [highest weight](../../../../../highest-weight-of-a-representation.md) $n$, and have dimension $n+1$. By [integration of a Lie-algebra representation](../../../../../integration-of-a-lie-algebra-representation.md), since $SU(2)$ is [simply connected](../../../../../simply-connected-space.md), every such [Lie algebra representation](../../../../../lie-algebra-representation.md) integrates uniquely. The resulting [homogeneous polynomial representation of SU2](../../../../../homogeneous-polynomial-representation-of-su2.md) is

$$
V_n=\operatorname{Sym}^n(\mathbb C^2),\qquad \dim V_n=n+1.
$$

In the [spin angular momentum](../../../../../spin.md) notation $j=n/2$, its Hermitian $J_3$ [eigenvalues](../../../../../eigenvalue.md) are $j,j-1,\ldots,-j$. The central matrix $-I$ acts on the [symmetric power](../../../../../symmetric-power.md) by $(-1)^n$, so [descent of an SU(2) representation to SO(3)](../../../../../descent-of-an-su-2-representation-to-so-3.md) occurs exactly when $n$ is even. Hence

$$
\boxed{SU(2):j=0,\tfrac12,1,\tfrac32,\ldots;\qquad SO(3):j=0,1,2,\ldots;\qquad \dim V_j=2j+1.}
$$

For a reducible representation, every summand must satisfy the descent condition. The spin-one-half doublet is a genuine representation of the covering group but does not define a single-valued representation of $SO(3)$; the spin-one triplet does and is its vector representation. The distinction is topological, rather than a difference in their isomorphic [Lie algebras](../../../../../lie-algebra-split.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
