<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Proper orthochronous Lorentz group](../../../../../../proper-orthochronous-lorentz-group.md) is the connected Lorentz group in the question. Its double cover is $SL(2,\mathbb C)$, viewed as a real [Lie group](../../../../../../lie-group.md). Identify a spacetime vector with the Hermitian matrix

$$
X=x^0I+x^a\sigma_a=\begin{pmatrix}x^0+x^3&x^1-ix^2\\x^1+ix^2&x^0-x^3\end{pmatrix},\qquad\det X=(x^0)^2-|\mathbf x|^2.
$$

The action $X\mapsto SXS^\dagger$ for $S\in SL(2,\mathbb C)$ preserves this determinant and hence the Minkowski metric. The group is connected, so its image is proper and orthochronous. Its kernel consists of $\pm I$: a matrix in the kernel first preserves $I$, hence is unitary, and then commutes with every Hermitian matrix, so is scalar; determinant one forces the two signs. Matrices in $SU(2)$ generate spatial rotations, and positive Hermitian determinant-one matrices generate boosts. Rotations and boosts generate the connected Lorentz group, so the action is onto. Polar decomposition also gives $SL(2,\mathbb C)\cong SU(2)\times\mathbb R^3$ as a manifold, proving that it is simply connected. This establishes the [Lorentz spinor double cover](../../../../../../lorentz-spinor-double-cover.md).

In an anti-Hermitian rotation-generator convention, the [Lorentz algebra](../../../../../../lorentz-algebra.md) brackets are

$$
[J_i,J_j]=\epsilon_{ijk}J_k,\qquad[J_i,K_j]=\epsilon_{ijk}K_k,\qquad[K_i,K_j]=-\epsilon_{ijk}J_k.
$$

The negative sign in the last bracket distinguishes boosts from Euclidean four-dimensional rotations. After complexification, set

$$
A_i=\frac{J_i+iK_i}{2},\qquad B_i=\frac{J_i-iK_i}{2}.
$$

A direct bracket calculation gives $[A_i,A_j]=\epsilon_{ijk}A_k$, $[B_i,B_j]=\epsilon_{ijk}B_k$ and $[A_i,B_j]=0$. Thus the [chiral decomposition of the complex Lorentz algebra](../../../../../../chiral-decomposition-of-the-complex-lorentz-algebra.md) is

$$
\mathfrak{so}(1,3)\otimes_{\mathbb R}\mathbb C\cong\mathfrak{sl}_2(\mathbb C)\oplus\mathfrak{sl}_2(\mathbb C).
$$

Complexification matters: the real Lorentz algebra is not the compact real algebra $\mathfrak{su}(2)\oplus\mathfrak{su}(2)$.

Each spin-$j$ [homogeneous polynomial representation of SU2](../../../../../../homogeneous-polynomial-representation-of-su2.md) extends from $SU(2)$ to $SL(2,\mathbb C)$ as $D_j(S)=\operatorname{Sym}^{2j}S$. Its complex-conjugate extension uses $\overline S$. The finite-dimensional irreducible complex [group representations](../../../../../../group-representation.md) of the covering group are therefore

$$
D^{(j_L,j_R)}(S)=D_{j_L}(S)\otimes D_{j_R}(\overline S),\qquad j_L,j_R\in\{0,\tfrac12,1,\ldots\}.
$$

The two separate complexified Lie-algebra factors act irreducibly on the two spin spaces, so their tensor product is irreducible. Conversely an invariant complex subspace for the real group is invariant under its complexified [Lie algebra](../../../../../../lie-algebra-split.md); the highest-weight classification for the two $\mathfrak{sl}_2$ factors gives exactly these tensor products. This constructs all [finite-dimensional complex Lorentz representations](../../../../../../finite-dimensional-complex-lorentz-representations.md).

Again $-I\in SL(2,\mathbb C)$ acts by $(-1)^{2j_L+2j_R}$. Therefore the [irreducible representations](../../../../../../irreducible-representation.md) of the connected Lorentz group itself, in this finite-dimensional complex category, are

$$
\boxed{(j_L,j_R),\quad j_L+j_R\in\mathbb Z,\quad\dim=(2j_L+1)(2j_R+1).}
$$

If the sum is a half-integer, the [group representation](../../../../../../group-representation.md) is a [group representation](../../../../../../group-representation.md) of the spin cover, or a projective [group representation](../../../../../../group-representation.md) of the Lorentz group, and is not an ordinary single-valued [group representation](../../../../../../group-representation.md) of the group named in the question.

The scalar $(0,0)$ and four-vector $(1/2,1/2)$ descend. The left and right [Weyl spinors](../../../../../../weyl-spinor.md), $(1/2,0)$ and $(0,1/2)$, do not. Their direct sum is a [Dirac spinor](../../../../../../dirac-spinor.md), reducible under the connected group; parity exchanges its two chiral summands. The [group representations](../../../../../../group-representation.md) $(1,0)$ and $(0,1)$ describe the two complex chiral parts of an antisymmetric tensor. On the rotation subgroup, self-duality of $SU(2)$ irreducibles identifies the conjugate spin space with the usual spin space, so the [Clebsch-Gordan decomposition for SU2](../../../../../../clebsch-gordan-decomposition-for-su2.md) gives the same spin range $|j_L-j_R|,\ldots,j_L+j_R$ as in part (i).

These are [group representations](../../../../../../group-representation.md) used for fields, and they need not be unitary for a positive-definite inner product. Indeed no nontrivial finite-dimensional [group representation](../../../../../../group-representation.md) of this group is unitary: if it were, its differential would embed the simple real Lorentz algebra into an algebra of skew-Hermitian matrices. The trace form $-\operatorname{tr}(XY)$ would give an invariant positive-definite form $b$ on that algebra. Invariance and the boost brackets would then force $-b(J_3,J_3)=b([K_1,K_2],J_3)=b(K_1,[K_2,J_3])=b(K_1,K_1)$, impossible for positive-definite $b$. Equivalently nontrivial boosts in these polynomial [group representations](../../../../../../group-representation.md) have real exponential rather than phase eigenvalues.

The qualification about dimension is necessary because a noncompact group also has infinite-dimensional unitary [group representations](../../../../../../group-representation.md). They too can be built using $SU(2)$ spin spaces, but not by a single finite pair. For example, the [rotation content of induced Lorentz representations](../../../../../../rotation-content-of-induced-lorentz-representations.md) is obtained from normalized [induced representations](../../../../../../induced-representation.md) of the upper triangular subgroup of $SL(2,\mathbb C)$, with $n\in\mathbb Z$, $\rho\in\mathbb R$ and unitary characters $(a/|a|)^n|a|^{2i\rho}$ on its diagonal $(a,a^{-1})$, trivial on its unipotent part. In the compact picture this uses functions on $SU(2)$ satisfying

$$
f\bigl(k\operatorname{diag}(e^{i\vartheta},e^{-i\vartheta})\bigr)=e^{-in\vartheta}f(k).
$$

Expanding functions into $SU(2)$ matrix coefficients selects a single right-torus weight from each spin space, giving the rotation content

$$
\bigoplus_{j=|n|/2,\ |n|/2+1,\ldots}V_j.
$$

Normalized induction supplies the boost action, coupling these infinitely many rotation spaces. The central sign is $(-1)^n$, so the even-$n$ family descends to the connected Lorentz group and has integer rotation spins. This explains both the finite-dimensional field construction and why a classification of unitary [group representations](../../../../../../group-representation.md) cannot simply be identified with the finite two-spin labels.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
