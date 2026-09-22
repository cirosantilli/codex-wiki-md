# Symmetry depends on preserved structure

↑ **Parent:** [Symmetry group](symmetry-group.md)

Take the four-point [set](set-split.md)

$$
R=\{(2,1),(-2,1),(-2,-1),(2,-1)\},
$$

the [vertices of a polygon](vertex-of-a-polygon.md) of a [rectangle](rectangle.md) whose side lengths are four and two. Three choices of structure give three different [symmetry groups](symmetry-group.md) on these same points.

As an unstructured [set](set-split.md), $R$ has all $4!=24$ [permutations](permutation.md) as symmetries, forming the [symmetric group](symmetric-group.md) $S_4$. If [Euclidean distance](euclidean-distance.md) is part of the data, the allowed maps are only the identity, a half-turn [rotation](rotation-mathematics.md), and the [reflections](reflection-mathematics.md) across the two coordinate axes. They form a [Klein four-group](klein-four-group.md) of [group order](order-of-a-finite-group.md) four. To see that nothing is missing, fix the image of one [vertex of a polygon](vertex-of-a-polygon.md): its three other distances, $2$, $4$, and $\sqrt{20}$, are distinct, so they uniquely determine the images of the remaining vertices.

Preserving affine structure permits more. The [affine map](affine-map.md)

$$
T(x,y)=(-2y,x/2),\qquad
T=\begin{pmatrix}0&-2\\1/2&0\end{pmatrix}
$$

cycles all four points of $R$. It sends a horizontal side of length four to a vertical side of length two, so it is not an [isometry](isometry.md). Yet it preserves the [rectangle](rectangle.md)'s vertex [set](set-split.md) and all [affine combinations](affine-combination.md) among those points.

<a id="image-an-affine-symmetry-preserves-these-four-points-while-changing-a-side-s-euclidean-length"></a>
![](rectangle-metric-versus-affine-symmetry.png)

**[Figure 2](#image-an-affine-symmetry-preserves-these-four-points-while-changing-a-side-s-euclidean-length). An affine symmetry preserves these four points while changing a side's Euclidean length**. Original example $T(x,y)=(-2y,x/2)$. The orange side of length four on the left is sent to the orange side of length two on the right. The point labels track the map for this illustration; they are not additional fixed labels imposed on the underlying four-point object.

Let $A=\operatorname{diag}(2,1)$ and let $r(x,y)=(-y,x)$ be the [square](square.md)'s quarter-turn [rotation](rotation-mathematics.md). Then

$$
T=ArA^{-1}.
$$

Conjugating every [square](square.md) symmetry by $A$ gives eight [affine maps](affine-map.md) preserving $R$. This [group isomorphism](group-isomorphism.md) makes the affine [symmetry group](symmetry-group.md) a [dihedral group](dihedral-group.md), although some of its maps do not preserve the original [Euclidean distances](euclidean-distance.md). There are no further affine symmetries: an [affine map](affine-map.md) preserves the common midpoint of the diagonals, so it must preserve opposite pairs. The image of one vertex has four choices and the image of an adjacent vertex has two; those choices determine the map through three noncollinear points.

Thus

$$
\boxed{G_{\rm metric}\subsetneq G_{\rm affine}\subsetneq G_{\rm set},\qquad
4<8<24.}
$$

An arbitrary [permutation](permutation.md) need not be an [affine map](affine-map.md). For example, exchanging the two top vertices while fixing the two bottom vertices sends the common diagonal midpoint to two different points, which no single [affine map](affine-map.md) can do. The phrase "the symmetry of these points" becomes unambiguous only after stating which structure matters.

## ↑ Ancestors (7)

1. [Symmetry group](symmetry-group.md)
2. [Group action](group-action-split.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
