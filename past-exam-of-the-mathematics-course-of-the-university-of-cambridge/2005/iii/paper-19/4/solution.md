<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Loop theorem](../../../../../loop-theorem.md) converts a nonzero kernel of $\pi_1(F)\to\pi_1(M)$, for a boundary [surface](../../../../../topological-surface.md) $F$, into a properly embedded [compression disk](../../../../../compression-disk.md). It is stronger than simply producing a singular nullhomotopy, and does not assert that every original self-intersecting loop is the boundary of the final disk.

The proof outline uses a strengthened version: keep the boundary class outside a prescribed [normal subgroup](../../../../../normal-subgroup.md) $N\triangleleft\pi_1(F)$. Begin with a singular disk in general position. Local cut-and-paste removes branch points; when a disk splits, at least one boundary stays outside $N$, since otherwise their product would lie in $N$. Take a regular neighborhood of its image and lift the disk through connected double covers of successive neighborhoods. Each lift decreases a finite lexicographic singularity complexity, so the tower terminates. At the top no double cover remains; mod-two duality forces its boundary components to be spheres. A boundary curve of the disk neighborhood lying outside the pulled-back $N$ then bounds an embedded disk on such a sphere, pushed inward. Project down one stage at a time. Exchange disk sectors along double curves, retaining a boundary outside $N$, to remove the projection's double intersections. Repeating yields an embedded disk downstairs. Taking $N=1$ proves the [Loop theorem](../../../../../loop-theorem.md); controlling a prescribed simple boundary gives [Dehn's lemma](../../../../../dehn-s-lemma.md). The key points are termination of the covering tower and preservation of an essential boundary during surgery, not an unjustified removal of all intersections by general position alone.

Two classification applications are particularly useful. First, a two-sided embedded [surface](../../../../../topological-surface.md) is incompressible precisely when its inclusion is fundamental-group injective, with the usual exclusion of inessential sphere components. A [compression disk](../../../../../compression-disk.md) immediately supplies a nontrivial kernel element. In the other direction, cut along the [surface](../../../../../topological-surface.md) and use the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md): if both boundary-copy maps were injective, the amalgamated-product or HNN normal-form theorem would make the original inclusion injective. Hence a nontrivial kernel appears on one cut side, and the [Loop theorem](../../../../../loop-theorem.md) produces a [compression disk](../../../../../compression-disk.md). This is what makes algebraically detected essential [surfaces](../../../../../topological-surface.md) usable in three-manifold splitting and incompressible hierarchies.

Second, consider a compact orientable [irreducible three-manifold](../../../../../irreducible-three-manifold.md) with one [torus](../../../../../torus.md) boundary. If that boundary is not fundamental-group injective, the [Loop theorem](../../../../../loop-theorem.md) supplies a [compression disk](../../../../../compression-disk.md). An essential simple curve on a [torus](../../../../../torus.md) is nonseparating, so compression changes the [torus](../../../../../torus.md) into a sphere. Pushing this sphere into the manifold, irreducibility gives a ball on the side away from the original [torus](../../../../../torus.md) boundary; the region between the sphere and the [torus](../../../../../torus.md) is the compression neighborhood. Undoing compression therefore attaches one one-handle to a ball. This proves the [solid-torus recognition by a compression disk](../../../../../solid-torus-recognition-by-a-compression-disk.md) criterion:

$$
\boxed{\text{irreducible compact orientable manifold with compressible torus boundary}\ \cong D^2\times S^1.}
$$

As a concrete consequence, a knot with [knot group](../../../../../knot-group.md) $\mathbb Z$ is the unknot. Its exterior is irreducible: a sphere disjoint from a connected knot bounds a ball on the side not containing the knot. The map from its boundary [group](../../../../../group-split.md) $\mathbb Z^2$ to $\mathbb Z$ cannot be injective, so its exterior is a solid [torus](../../../../../torus.md). The boundary of a meridian disk of this exterior lies in the kernel of the linking-number map; it is therefore the primitive preferred longitude. Joining that longitude to the knot through its tubular neighborhood makes an embedded spanning disk for the knot. This proves **the cyclic-knot-group unknot criterion**, rather than merely identifying a familiar consequence by name.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
