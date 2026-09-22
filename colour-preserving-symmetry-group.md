# Colour-preserving symmetry group

↑ **Parent:** [Symmetry group](symmetry-group.md)

Let a [group action](group-action-split.md) of $G$ on a [set](set-split.md) $X$ be given, and let a [function](function-split.md) $c:X\to C$ attach a colour label to each point. The colour-preserving subgroup of $G$ is

$$
G_c=\{g\in G:c(gx)=c(x)\text{ for every }x\in X\}.
$$

It is a [subgroup](subgroup.md): the [identity map](identity-function.md) preserves all labels, compositions of two preserving maps preserve them, and replacing $x$ by $g^{-1}x$ shows that [inverse maps](inverse-function.md) preserve them too. Extra object data restrict the allowable transformations; the labels are now part of the object rather than bookkeeping for a drawing.

For a geometric [square](square.md), take $G=D_4$, of [group order](order-of-a-finite-group.md) eight. If all four vertices have the same colour, all eight maps remain. If two adjacent vertices are red and the others blue, only the identity and one [reflection](reflection-mathematics.md) remain. Putting the two red vertices opposite one another instead leaves four maps: the identity, a half-turn [rotation](rotation-mathematics.md), and the two diagonal [reflections](reflection-mathematics.md). Giving all four vertices distinct colours leaves only the identity.

<a id="image-fixed-vertex-colours-restrict-the-geometric-symmetry-group"></a>
![](square-colours-restrict-symmetry-groups.png)

**[Figure 3](#image-fixed-vertex-colours-restrict-the-geometric-symmetry-group). Fixed vertex colours restrict the geometric symmetry group**. Original computed examples. Counts refer to Euclidean motions of the square that preserve each vertex colour. Two adjacent red vertices and two opposite red vertices have the same colour counts but different symmetry groups. Dashed lines show surviving reflection axes; the rotation labels count surviving rotations including the identity.

The count alone does not specify the pattern. Both two-red examples have the same number of red and blue vertices, but their [stabilizer subgroups](stabilizer-subgroup.md) differ. For a single red vertex, the [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) gives a [group orbit](orbit-group-theory.md) of size four and a [stabilizer subgroup](stabilizer-subgroup.md) of [group order](order-of-a-finite-group.md) two, agreeing with the existing [group action](group-action-split.md) illustration. Such counts identify equivalent placements without treating each placement as a new geometric case.

## ↑ Ancestors (7)

1. [Symmetry group](symmetry-group.md)
2. [Group action](group-action-split.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
