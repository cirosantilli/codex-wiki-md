<h1 id="5d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Place the cube's vertices at $(\pm1,\pm1,\pm1)$. Its full [symmetry group of a cube](../../../../../../symmetry-group-of-a-cube.md) consists of [signed permutation matrices](../../../../../../signed-permutation-matrix.md). To see completeness, a cube symmetry fixes its [center of a group](../../../../../../center-of-a-group.md) and permutes the six face normals, so it sends coordinate axes to signed coordinate axes; conversely every such matrix preserves the cube. Coordinate [permutations](../../../../../../permutation.md) and sign changes take any edge to any other edge, so this is a [transitive group action](../../../../../../transitive-group-action.md) on edges.

Choose the edge $e=\{(1,1,z):-1\le z\le1\}$. A symmetry stabilizing it must preserve its axis direction and its midpoint $(1,1,0)$. It can swap the first two coordinates and independently reverse the third coordinate, but cannot change the signs of the two fixed coordinates. Hence

$$
\boxed{\operatorname{Stab}_H(e)=\langle (x,y,z)\mapsto(y,x,z),\ (x,y,z)\mapsto(x,y,-z)\rangle
\cong C_2\times C_2.}
$$

There are twelve edges and four elements of the [stabilizer subgroup](../../../../../../stabilizer-subgroup.md). The [orbit-stabiliser theorem](../../../../../../orbit-stabilizer-theorem.md) therefore gives **$|H|=48$**, including orientation-reversing symmetries, not just the twenty-four rotations.

The action defines a [group homomorphism](../../../../../../group-homomorphism.md) $H\to S_{12}$. If an element fixes every edge as a set, it fixes every vertex, since each vertex is the unique common point of its three incident edges. A cube isometry fixing all vertices is the identity. Thus this is a [faithful group action](../../../../../../faithful-group-action.md), and the [cube symmetry action on edges](../../../../../../cube-symmetry-action-on-edges.md) embeds $H$ as a [subgroup](../../../../../../subgroup.md) with

$$
\boxed{[S_{12}:H]=\frac{12!}{48}=9\,979\,200.}
$$

It is **not a [normal subgroup](../../../../../../normal-subgroup.md)**. Central inversion $\mathbf x\mapsto-\mathbf x$ belongs to $H$ and swaps the twelve edges in six opposite pairs. In $S_{12}$, all [permutations](../../../../../../permutation.md) of cycle type $2^6$ are conjugate, and their number is

$$
\frac{12!}{2^6\,6!}=10\,395>48.
$$

If $H$ were a [normal subgroup](../../../../../../normal-subgroup.md), it would contain this entire [conjugacy class](../../../../../../conjugacy-class.md), impossible for a [group](../../../../../../group-split.md) of order forty-eight. This avoids relying on a classification of normal [subgroups](../../../../../../subgroup.md) of the symmetric [group](../../../../../../group-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
