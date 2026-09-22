<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

For a [group action](../../../../../group-action.md) of a [finite group](../../../../../finite-group.md) $G$ on a set $X$, let $G_x=\{g:gx=x\}$ be the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) and $Gx=\{gx:g\in G\}$ the [orbit](../../../../../orbit-dynamical-system.md). The [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) is

$$
\boxed{|Gx|=[G:G_x],\qquad |G|=|Gx|\,|G_x|.}
$$

To prove it, the map from left [cosets](../../../../../coset.md) to the orbit, $gG_x\mapsto gx$, is well-defined because multiplying $g$ on the right by an element fixing $x$ does not change $gx$. It is surjective by the definition of the orbit. If $gx=hx$, then $h^{-1}g\in G_x$, so $gG_x=hG_x$; hence it is injective. The cardinality identity now follows from [Lagrange's theorem](../../../../../lagrange-s-theorem.md).

Place the octahedron's vertices at $\pm e_1,\pm e_2,\pm e_3$. A symmetry fixes their centre, so it is an orthogonal map and must take an opposite pair of vertices to another opposite pair. Its matrix is thus a [signed permutation matrix](../../../../../signed-permutation-matrix.md). Conversely every signed [permutation](../../../../../permutation.md) of these coordinate directions preserves the vertices, edges and faces. Therefore the [full octahedral symmetry group](../../../../../symmetry-group-of-a-cube.md) has

$$
\boxed{|G|=3!\,2^3=48.}
$$

These same signed [permutation](../../../../../permutation.md) matrices preserve the cube with vertices $(\pm1,\pm1,\pm1)$, so the [group](../../../../../group-split.md) is also the [symmetry group of a cube](../../../../../symmetry-group-of-a-cube.md). The opposite-vertex lines are the three coordinate axes, so **$|D|=3$**. The action on them is transitive, giving a line stabilizer of order $48/3=16$.

For the line $\mathbb Re_3$, the precise [axis stabilizer in the full octahedral symmetry group](../../../../../axis-stabilizer-in-the-full-octahedral-symmetry-group.md) consists of the block matrices

$$
\begin{pmatrix}A&0\\0&\varepsilon\end{pmatrix},\qquad
A\text{ a signed }2\times2\text{ permutation matrix},\quad\varepsilon\in\{1,-1\}.
$$

The eight possible $A$ are the symmetries of a square in the perpendicular plane, a [dihedral group](../../../../../dihedral-group.md) of order eight; the independent sign $\varepsilon$ reverses the selected axis. Thus

$$
\boxed{G_{\mathbb Re_3}\cong D_8\times C_2.}
$$

Here $D_8$ denotes the order-eight square-symmetry [group](../../../../../group-split.md). The selected line is unoriented: its two endpoints may be exchanged. Fixing an individual endpoint instead would give only the order-eight [subgroup](../../../../../subgroup.md) with $\varepsilon=1$.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
