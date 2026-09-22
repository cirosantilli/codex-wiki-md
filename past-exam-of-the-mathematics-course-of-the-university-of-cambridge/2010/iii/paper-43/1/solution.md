<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) acts on the algebra itself by $\operatorname{ad}_X(Y)=[X,Y]$. The [Jacobi identity](../../../../../jacobi-identity.md) gives $[\operatorname{ad}_X,\operatorname{ad}_Y]=\operatorname{ad}_{[X,Y]}$, so this is a [Lie algebra representation](../../../../../lie-algebra-representation.md). In the generator basis, the column labelled $b$ records the coefficients of $[T_a,T_b]$, giving

$$
\boxed{(t_a^{\mathrm{Ad}})^c{}_b=i f_{abc}.}
$$

In the orthonormal compact-algebra convention, the [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md) are totally antisymmetric. With the row index written first this is $(t_a^{\mathrm{Ad}})_{bc}=-if_{abc}$.

Applying the representation to the generator [commutator](../../../../../commutator.md) and taking a [trace](../../../../../matrix-trace.md) against $t_c^R$ gives

$$
\operatorname{tr}([t_a^R,t_b^R]t_c^R)
=i f_{abd}\operatorname{tr}(t_d^Rt_c^R)
=i C(R)f_{abc}.
$$

Consequently, for a nonzero [trace](../../../../../matrix-trace.md) normalization,

$$
\boxed{f_{abc}=-\frac{i}{C(R)}\operatorname{tr}([t_a^R,t_b^R]t_c^R).}
$$

The [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md) also shows that this expression is antisymmetric in every pair of indices, justifying the orthonormal convention used for the adjoint matrices.

The summed [quadratic Casimir operator](../../../../../quadratic-casimir-operator.md) has scalar value $C_2(R)$ on the representation under consideration. Taking its [trace](../../../../../matrix-trace.md) in two ways yields

$$
\sum_{a=1}^{d(G)}\operatorname{tr}(t_a^Rt_a^R)=C(R)d(G)=C_2(R)d(R),
$$

and hence

$$
\boxed{C(R)=\frac{d(R)C_2(R)}{d(G)}.}
$$

The constant $C(R)$ is the representation's [Dynkin index](../../../../../dynkin-index.md) in this normalization.

Differentiating the [tensor product of group representations](../../../../../tensor-product-of-group-representations.md) gives

$$
\boxed{t_a^{R_1\otimes R_2}=t_a^{R_1}\otimes I_{d(R_2)}+I_{d(R_1)}\otimes t_a^{R_2}.}
$$

The generators acting on the two factors commute, so the sum of their squares is

$$
\sum_a(t_a^{R_1\otimes R_2})^2
=[C_2(R_1)+C_2(R_2)]I+2\sum_at_a^{R_1}\otimes t_a^{R_2}.
$$

For a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), every element is a sum of [commutators](../../../../../commutator.md). Since the [trace](../../../../../matrix-trace.md) of each represented [commutator](../../../../../commutator.md) vanishes, all represented generators are [traceless matrices](../../../../../traceless-matrix.md). The [trace](../../../../../matrix-trace.md) of the cross term is therefore zero. Taking the [trace](../../../../../matrix-trace.md) after decomposition into [irreducible representations](../../../../../irreducible-representation.md) instead gives the [tensor-product Casimir trace identity](../../../../../tensor-product-casimir-trace-identity.md)

$$
\boxed{[C_2(R_1)+C_2(R_2)]d(R_1)d(R_2)=\sum_i C_2(R_i)d(R_i),}
$$

where repeated irreducible constituents occur repeatedly in the sum.

This step requires tracelessness, as holds for the special unitary groups used below. For an arbitrary algebra with an abelian factor, the general [trace](../../../../../matrix-trace.md) formula has the extra term $2\sum_a\operatorname{tr}(t_a^{R_1})\operatorname{tr}(t_a^{R_2})$. For example, one-dimensional representations of an abelian generator with charges one and one have individual Casimirs one, while the product generator has charge two and Casimir four. Thus the identity without the cross term is not a theorem for every [Lie algebra](../../../../../lie-algebra-split.md) as the unrestricted opening wording might suggest.

For the [fundamental-antifundamental decomposition for SU(N)](../../../../../fundamental-antifundamental-decomposition-for-su-n.md), write a product [tensor](../../../../../tensor.md) as a [matrix](../../../../../matrix.md) $M^i{}_j$. It transforms as $M\mapsto UMU^{-1}$, and decomposes uniquely as

$$
M=\frac{\operatorname{tr}M}{N}I+\left(M-\frac{\operatorname{tr}M}{N}I\right).
$$

The first term is a [trivial representation](../../../../../trivial-representation.md), and the second is the invariant traceless subspace, of [dimension](../../../../../dimension-vector-space.md) $N^2-1$. Its infinitesimal transformation is a [commutator](../../../../../commutator.md), so it is the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). This representation is irreducible for $N\ge2$: an [invariant subspace](../../../../../invariant-subspace.md) is an ideal of $\mathfrak{sl}_N$; commuting a nonzero ideal element with diagonal and elementary matrices produces off-diagonal elementary matrices, whose further [commutators](../../../../../commutator.md) generate all off-diagonal matrices and traceless diagonal matrices. A purely diagonal nonzero element also produces an off-diagonal element unless it is scalar, and a traceless scalar in characteristic zero is zero. Therefore

$$
\boxed{\mathbf N\otimes\overline{\mathbf N}=\mathbf1\oplus\mathbf{Adj},\qquad d(\mathbf{Adj})=N^2-1.}
$$

For the conjugate defining representation the generators are $-t_a^T$, so its [trace](../../../../../matrix-trace.md) index and Casimir equal those of the defining representation. With $C(\mathbf N)=1/2$, the [trace](../../../../../matrix-trace.md) formula gives $C_2(\mathbf N)=(N^2-1)/(2N)$. The product [trace](../../../../../matrix-trace.md) identity, with the zero Casimir of the singlet, then reads

$$
2\frac{N^2-1}{2N}N^2=C_2(\mathbf{Adj})(N^2-1).
$$

Cancelling the nonzero factor yields

$$
\boxed{C_2(\mathbf{Adj})=N.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
