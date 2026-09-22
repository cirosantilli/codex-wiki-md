<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Write the affine modes as $J_n^a=T_n^a$, and put $Q=Q^{\mathfrak g}$. The [Sugawara construction](../../../../../sugawara-construction.md) requires a restricted module, meaning that sufficiently large positive current modes annihilate each fixed vector, and a noncritical level $2k+Q\ne0$. A positive-energy [highest-weight representation](../../../../../highest-weight-representation.md) has the required restriction. Define

$$
S_m=\sum_{a,p\in\mathbb Z}:J^a_{m-p}J^a_p:,
\qquad \boxed{L_m^{\mathfrak g}=\frac{S_m}{2k+Q}}.
$$

[Normal ordering](../../../../../normal-ordering.md) puts positive modes to the right, making each sum finite on a fixed finite-energy vector. The invariant sum over the current index $a$ is the quadratic [Casimir operator](../../../../../casimir-element.md) construction for the [affine current algebra](../../../../../affine-current-algebra.md).

Here is the [normal ordering](../../../../../normal-ordering.md) calculation responsible for its denominator. In commuting $S_m$ with $J_n^b$, the two affine central terms supply $-2knJ_{m+n}^b$. The remaining terms contain $if^{abc}$ times the two ways to replace a current by $J_{p+n}^c$. Relabeling the summation index and using antisymmetry of $f^{abc}$ cancels the un-reordered terms. Reordering the modes that cross the creation/annihilation boundary leaves $n$ signed terms, whose two [structure constants](../../../../../structure-constant.md) contract by $f^{abc}f^{abd}=Q\delta^{cd}$. Their sum is $-QnJ_{m+n}^b$. Thus

$$
[S_m,J_n^b]=-(2k+Q)nJ_{m+n}^b,
\qquad \boxed{[L_m^{\mathfrak g},J_n^b]=-nJ_{m+n}^b}.
$$

The adjoint-Casimir contribution is genuinely quantum. For an explicit check of its coefficient, let $|0\rangle$ be the affine vacuum, with all $J_n^a|0\rangle=0$ for $n\ge0$. Then

$$
S_0=\sum_a(J_0^a)^2+2\sum_{a,p>0}J_{-p}^aJ_p^a,
\qquad S_0J_{-1}^b|0\rangle=(Q+2k)J_{-1}^b|0\rangle.
$$

The first term acts by the adjoint [Casimir operator](../../../../../casimir-element.md) $Q$, and only $p=1$ contributes $2k$ to the second. This also verifies that a current has conformal weight one under the displayed normalization.

Now commute the quadratic generators with one another. Acting on either current factor produces $(m-n)L_{m+n}^{\mathfrak g}$; the residual full contractions are scalar and vanish unless $m+n=0$. The [Jacobi identity](../../../../../jacobi-identity.md) fixes their cubic dependence on $m$, and the plane vacuum convention $L_{-1}|0\rangle=L_0|0\rangle=L_1|0\rangle=0$ fixes the combination $m^3-m$. To determine its coefficient explicitly, note

$$
L_{-2}^{\mathfrak g}|0\rangle=\frac1{2k+Q}\sum_a J_{-1}^aJ_{-1}^a|0\rangle.
$$

Commuting a single $J_1^a$ through the numerator gives $(2k+Q)J_{-1}^a|0\rangle$: the two central contractions give $2kJ_{-1}^a$, and the zero-mode commutator in the structure-constant term gives $QJ_{-1}^a$. The remaining $J_1^a$ contraction gives $k$ for each adjoint index. Therefore

$$
\|L_{-2}^{\mathfrak g}|0\rangle\|^2
=\frac{k(2k+Q)\dim\mathfrak g}{(2k+Q)^2}
=\frac{k\dim\mathfrak g}{2k+Q}=\frac{c^{\mathfrak g}}2.
$$

For an algebraic module without a positive [inner product](../../../../../inner-product.md), the same calculation is its vacuum matrix element and fixes the universal central term. Consequently

$$
\boxed{[L_m^{\mathfrak g},L_n^{\mathfrak g}]=(m-n)L_{m+n}^{\mathfrak g}+\frac{c^{\mathfrak g}}{12}(m^3-m)\delta_{m+n,0}},\qquad
\boxed{c^{\mathfrak g}=\frac{2k\dim\mathfrak g}{2k+Q}}.
$$

This is a representation of the [Virasoro algebra](../../../../../virasoro-algebra.md), not merely its centerless part.

For a complex semisimple [Lie algebra](../../../../../lie-algebra-split.md), a [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathfrak h$ is a maximal abelian subalgebra of semisimple elements; equivalently it is the complexification of a maximal torus algebra in the compact real form. Its dimension is the [rank of a semisimple Lie algebra](../../../../../rank-of-a-semisimple-lie-algebra.md), $r$. Choose an orthonormal Cartan basis with currents $H_n^i$. They have no structure-constant term:

$$
[H_m^i,H_n^j]=km\delta^{ij}\delta_{m+n,0}.
$$

For $k\ne0$, their abelian [Sugawara construction](../../../../../sugawara-construction.md) is

$$
L_m^{\mathfrak h}=\frac1{2k}\sum_{i=1}^{r}\sum_p:H_{m-p}^iH_p^i:,
\qquad c^{\mathfrak h}=r.
$$

Each Cartan current has weight one under both $L^{\mathfrak g}$ and $L^{\mathfrak h}$, so $K_m=L_m^{\mathfrak g}-L_m^{\mathfrak h}$ commutes with all $H_n^i$, hence also with $L_n^{\mathfrak h}$. Subtracting the two commuting stress tensors yields the [Coset construction](../../../../../coset-construction.md)

$$
[K_m,K_n]=(m-n)K_{m+n}+\frac{c^{\mathfrak g}-r}{12}(m^3-m)\delta_{m+n,0}.
$$

In the intended nontrivial compact unitary theory at positive admissible level, this coset acts on a positive inner-product space, with $K_m^\dagger=K_{-m}$. Its vacuum satisfies $K_n|0\rangle=0$ for $n\ge-1$, so

$$
0\le\|K_{-2}|0\rangle\|^2=\langle0|[K_2,K_{-2}]|0\rangle=\frac{c^{\mathfrak g}-r}{2}.
$$

Thus $c^{\mathfrak g}\ge r$. Also $Q>0$ for a compact [simple Lie algebra](../../../../../simple-lie-algebra.md) and $k>0$, so $2k/(2k+Q)<1$, which proves the upper bound directly. Hence, under these physical representation hypotheses,

$$
\boxed{\operatorname{rank}\mathfrak g\le c^{\mathfrak g}\le\dim\mathfrak g}.
$$

The upper inequality is strict at finite positive level; $c^{\mathfrak g}$ tends to $\dim\mathfrak g$ as the level grows.

The positivity hypothesis is necessary and is not implied by the bare affine commutation relation. For example, at $k=0$ its trivial representation has all currents zero and gives $c^{\mathfrak g}=0<\operatorname{rank}\mathfrak g$. Even positive arbitrary levels need not satisfy the bound: with $\mathfrak g=\mathfrak{su}(2)$, $f^{abc}=\epsilon^{abc}$, $Q=2$ and $k=1/4$, the formula gives $c^{\mathfrak g}=3/5<1$. Such a level does not give the intended compact unitary positive-energy theory. Thus the last bound is a statement about nontrivial unitary admissible-level representations; it cannot hold for every representation in the unrestricted algebraic formulation. At $2k+Q=0$ the displayed [Sugawara construction](../../../../../sugawara-construction.md) itself is undefined.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
