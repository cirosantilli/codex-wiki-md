<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

A [plane crystallographic group](../../../../../wallpaper-group.md) is a discrete [subgroup](../../../../../subgroup.md) of the [Euclidean plane](../../../../../euclidean-plane.md)'s [isometry group](../../../../../isometry-group.md) with compact quotient; equivalently a [compact set](../../../../../compact-space.md) has translates covering the plane. We prove the [crystallographic restriction theorem](../../../../../crystallographic-restriction-theorem.md) without assuming its conclusion. The orientation-preserving [subgroup](../../../../../subgroup.md) $G^+$ has index at most two and still has a [cocompact group action](../../../../../cocompact-group-action.md). Its [subgroup](../../../../../subgroup.md) $T$ of [translations](../../../../../translation-geometry.md) is discrete as an additive [subgroup](../../../../../subgroup.md) of $\mathbb R^2$.

Suppose $T$ were trivial. Linear parts of orientation-preserving plane isometries commute, so every [group commutator](../../../../../group-commutator.md) in $G^+$ is a translation. Thus $G^+$ would be an [abelian group](../../../../../abelian-group.md). Every member would then commute with the given nontrivial rotation $g$ and preserve its unique [fixed point](../../../../../fixed-point.md). A discrete [subgroup](../../../../../subgroup.md) of the compact rotation group about that point is finite. Then $G$ would be finite, contradicting cocompactness on the unbounded plane. Hence $T$ contains a nonzero vector $v$.

If $g$ is a half-turn its order is already two. Otherwise its linear part $R$ rotates $v$ to a linearly independent vector $Rv$, and conjugating [translations](../../../../../translation-geometry.md) shows that $Rv\in T$. Thus $T$ spans the plane and is a [euclidean lattice](../../../../../euclidean-lattice.md). A discrete additive [subgroup](../../../../../subgroup.md) meets every bounded closed set in finitely many points: an accumulating sequence would give nonzero differences tending to zero, contradicting isolation of the identity. To see the [euclidean lattice](../../../../../euclidean-lattice.md) assertion directly, choose a shortest nonzero translation $v$. [Translations](../../../../../translation-geometry.md) on its line are integer multiples of $v$. Reducing all parallel components modulo $v$ shows that nonzero perpendicular components are bounded away from zero, since otherwise infinitely many translation vectors would accumulate in a compact rectangle. Choose a vector $w$ with the smallest positive perpendicular component; reducing by $w$ and then $v$ proves $T=\mathbb Zv+\mathbb Zw$.

Conjugation by $g$ preserves this [euclidean lattice](../../../../../euclidean-lattice.md). In its [euclidean lattice](../../../../../euclidean-lattice.md) basis, $R$ is therefore an invertible integer matrix with [determinant](../../../../../determinant.md) one. Its [trace](../../../../../matrix-trace.md) is an integer and is also $2\cos\theta$, where $\theta$ is the rotation angle. Since $g$ is nontrivial,

$$
2\cos\theta\in\{-2,-1,0,1\}.
$$

These values give angles of order $2,3,4,6$ respectively. Hence

$$
\boxed{\operatorname{ord}(g)\in\{2,3,4,6\}}.
$$

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
