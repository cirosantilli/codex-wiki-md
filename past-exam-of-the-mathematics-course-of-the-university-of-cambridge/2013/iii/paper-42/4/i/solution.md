<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Start with the [classification of finite-dimensional representations of SU2](../../../../../../classification-of-finite-dimensional-representations-of-su2.md). Its irreducible complex [group representations](../../../../../../group-representation.md) are the spin-$j$ spaces

$$
V_j=\operatorname{Sym}^{2j}\mathbb C^2,\qquad j=0,\tfrac12,1,\ldots,\qquad\dim V_j=2j+1.
$$

The central element $-I$ acts on $V_j$ as $(-1)^{2j}$. These facts follow also by realizing $V_j$ as homogeneous polynomials of degree $2j$ in two variables: the raising and lowering operators connect all of their one-dimensional weight spaces, and the highest-weight classification supplies every irreducible.

Identify Euclidean four-space with the [quaternions](../../../../../../quaternion.md). The [unit quaternions](../../../../../../unit-quaternion.md), each a copy of $SU(2)$, act by

$$
(a,b):q\longmapsto aqb^{-1}.
$$

The norm is multiplicative, so this is an orthogonal action. It preserves orientation because the acting group is connected. If it fixes every $q$, setting $q=1$ first gives $a=b$, and then this [quaternion](../../../../../../quaternion.md) must commute with every [quaternion](../../../../../../quaternion.md); a real unit [quaternion](../../../../../../quaternion.md) is $\pm1$. The kernel is therefore $\{(1,1),(-1,-1)\}$.

For completeness, the differential is injective: if imaginary [quaternions](../../../../../../quaternion.md) $u,v$ satisfy $uq-qv=0$ for every $q$, then $u=v$ is central and imaginary, hence zero. Both [Lie algebras](../../../../../../lie-algebra-split.md) have dimension six. Thus the image contains a neighbourhood of the identity and is an open subgroup of the connected [SO(4) group](../../../../../../so-4-group.md), so it is the whole group. This proves the [Spin(4) double cover](../../../../../../spin-4-double-cover.md)

$$
\boxed{SO(4)\cong\bigl(SU(2)_L\times SU(2)_R\bigr)/\{(I,I),(-I,-I)\}.}
$$

The covering group is simply connected since each $SU(2)$ is a three-sphere.

The [irreducible representations](../../../../../../irreducible-representation.md) of a product of compact groups are tensor products of irreducibles of its two factors. One way to see this is to decompose an irreducible space into isotypic components for the first factor; the second commutes with the first, so only one isotypic component can occur. The multiplicity space must then be irreducible for the second factor. Hence the covering-group irreducibles are $V_{j_L}\otimes V_{j_R}$. By [central parity on SU2 tensor products](../../../../../../central-parity-on-su2-tensor-products.md), the kernel element acts as $(-1)^{2j_L+2j_R}$. The [group representation](../../../../../../group-representation.md) descends to $SO(4)$ precisely when that sign is positive. The [representations of SO(4) from two SU2 spins](../../../../../../representations-of-so-4-from-two-su2-spins.md) are therefore

$$
\boxed{(j_L,j_R),\quad j_L+j_R\in\mathbb Z,\quad\dim=(2j_L+1)(2j_R+1).}
$$

Every finite-dimensional irreducible complex [group representation](../../../../../../group-representation.md) of $SO(4)$ is obtained this way. Since the group is compact, these are also all its continuous irreducible unitary [group representations](../../../../../../group-representation.md), up to equivalence.

The Lie-algebra version makes the two spin labels visible locally. Choose rotation generators $J_i$ and generators $K_i$ mixing the fourth direction with the first three, normalized so that

$$
[J_i,J_j]=\epsilon_{ijk}J_k,\qquad[J_i,K_j]=\epsilon_{ijk}K_k,\qquad[K_i,K_j]=\epsilon_{ijk}J_k.
$$

Then $A_i=(J_i+K_i)/2$ and $B_i=(J_i-K_i)/2$ obey two commuting copies of $\mathfrak{su}(2)$. The [quaternion](../../../../../../quaternion.md) quotient determines which [Lie algebra representations](../../../../../../lie-algebra-representation.md) integrate to the actual group, rather than only to its cover.

For example, $(0,0)$ is the scalar, $(1/2,1/2)$ is the four-vector, and $(1,0)$ and $(0,1)$ are the three-dimensional self-dual and anti-self-dual two-form [group representations](../../../../../../group-representation.md). The half-spin spaces $(1/2,0)$ and $(0,1/2)$ belong to the cover and do not descend to $SO(4)$. Restricting to rotations fixing the real [quaternion](../../../../../../quaternion.md) axis gives the diagonal $SU(2)$, and the [Clebsch-Gordan decomposition for SU2](../../../../../../clebsch-gordan-decomposition-for-su2.md) yields

$$
V_{j_L}\otimes V_{j_R}\big|_{\mathrm{diag}\,SU(2)}\cong\bigoplus_{j=|j_L-j_R|}^{j_L+j_R}V_j,
$$

with steps of one. For a descended [group representation](../../../../../../group-representation.md) these diagonal spins are integers, as required for the spatial $SO(3)$ subgroup.

## ↑ Ancestors (11)

1. [I](../i.md)
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
