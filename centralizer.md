# Centralizer

↑ **Parent:** [Centralizer and normalizer](centralizer-and-normalizer.md)

The [centralizer](centralizer.md) of an element $x$ of a [group](group-split.md) $G$ consists of all elements that commute with $x$:

$$
C_G(x)=\{g\in G:gx=xg\}=\{g\in G:gxg^{-1}=x\}.
$$

It is the [stabilizer subgroup](stabilizer-subgroup.md) of $x$ under the [conjugation action](conjugation-action.md), hence a [subgroup](subgroup.md) of $G$. In [conjugacy classes of the symmetric group on three letters](conjugacy-classes-of-the-symmetric-group-on-three-letters.md), the three representative computations are

$$
C_{S_3}(e)=S_3,\qquad C_{S_3}((12))=\{e,(12)\},\qquad C_{S_3}((123))=\{e,(123),(132)\}.
$$

For the [transposition](transposition-permutation.md) $(12)$, a commuting [permutation](permutation.md) must preserve the exchanged pair $\{1,2\}$ and fix $3$; only $e$ and $(12)$ do so. For $r=(123)$, a commuting [permutation](permutation.md) is determined by where it sends $1$: the equation $g(r(i))=r(g(i))$ forces the images of $2$ and $3$, leaving exactly $e,r,r^2$. For $e$, every [permutation](permutation.md) commutes. These [centralizer](centralizer.md) sizes $6,2,3$ give [conjugacy class](conjugacy-class.md) sizes $1,3,2$.

The [centralizer](centralizer.md) is useful because it measures how much freedom remains after fixing one operation. Its [index of a subgroup](index-of-a-subgroup.md) counts the distinct results of [conjugation](conjugation.md), and the intersection of all element [centralizers](centralizer.md) is the [center of a group](center-of-a-group.md). A [centralizer](centralizer.md) need not be an [abelian group](abelian-group.md): $C_G(e)=G$ even when $G$ is a [nonabelian group](non-abelian-group.md). In an [abelian group](abelian-group.md), all element [centralizers](centralizer.md) equal $G$. These observations also explain why the surrounding [group](group-split.md) matters: the [centralizer](centralizer.md) of $(123)$ inside the [alternating group](alternating-group.md) $A_3$ is the whole $A_3$, whereas its [centralizer](centralizer.md) inside $S_3$ is a proper [subgroup](subgroup.md). See [McKernan, the centralizer definition preceding lemma 23.6](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/96221ce2d5b1077b3e5d3c5e08c88afe_MIT18_703S13_pra_l_23.pdf).

For an arbitrary [subset](subset.md) $A\subseteq G$, the [centralizer of a subset](centralizer-of-a-subset.md) fixes every element of $A$ individually under the [conjugation action](conjugation-action.md):

$$
C_G(A)=\{g\in G:ga=ag\text{ for all }a\in A\}=\bigcap_{a\in A}C_G(a).
$$

This is a [pointwise stabilizer](pointwise-stabilizer.md) of the elements of $A$, not of the [vertices of a polygon](vertex-of-a-polygon.md) in a geometric realization. In particular, $r=(123)$ belongs to $C_{S_3}(r)$ although its [rotation](rotation-mathematics.md) moves every [vertex of a polygon](vertex-of-a-polygon.md) of the [equilateral triangle](equilateral-triangle.md). If $A$ generates a [subgroup](subgroup.md) $H$, commuting with every element of $A$ implies commuting with every product of those elements and their [inverse elements](inverse-element.md); hence $C_G(A)=C_G(H)$. For the triangle [rotation](rotation-mathematics.md) [subgroup](subgroup.md) $H=\langle r\rangle$, this gives $C_{S_3}(H)=C_{S_3}(r)=H$.

To see the commutation test directly on the [equilateral triangle](equilateral-triangle.md), compare a [rotation](rotation-mathematics.md) $r$ with the [reflection](reflection-mathematics.md) $s=(12)$. Their [permutations](permutation.md) satisfy

$$
rs=(13),\qquad sr=(23),\qquad srs^{-1}=r^{-1}.
$$

The two orders send [vertex of a polygon](vertex-of-a-polygon.md) $1$ to different places: $rs(1)=3$, but $sr(1)=1$. Thus $s\notin C_{S_3}(r)$. By contrast $r$ and $r^2$ commute, with $rr^2=r^2r=e$. The [reflection](reflection-mathematics.md) reverses the chosen [rotation](rotation-mathematics.md) while preserving the [subgroup](subgroup.md) of all triangle [rotations](rotation-mathematics.md), so $s\in N_{S_3}(H)$. The distinction is visible before any counting: commuting preserves an operation itself; membership in the [normalizer](normalizer.md) permits exchanging it with another operation in the same [subgroup](subgroup.md).

<a id="image-commuting-triangle-rotations-and-noncommuting-rotation-reflection-products"></a>
![](triangle-permutation-operation-order.png)

**[Figure 11](#image-commuting-triangle-rotations-and-noncommuting-rotation-reflection-products). Commuting triangle rotations and noncommuting rotation–reflection products**. Colored labels track the original [vertices of a polygon](vertex-of-a-polygon.md). Products act from right to left. The top row gives the same labeled triangle for $rr^2$ and $r^2r$; the bottom row gives different labeled triangles for $rs$ and $sr$. All six [permutations](permutation.md) in $S_3$ are included in the [centralizer](centralizer.md) and [normalizer](normalizer.md) membership table.

**Table of contents**

- [Centralizer of a subset](centralizer-of-a-subset.md)
- [Centraliser of a fixed-point-free involution](centraliser-of-a-fixed-point-free-involution.md)
- [Centraliser of a transposition](centraliser-of-a-transposition.md)

## ↑ Ancestors (8)

1. [Centralizer and normalizer](centralizer-and-normalizer.md)
2. [Conjugation action](conjugation-action.md)
3. [Group action](group-action.md)
4. [Group theory](group-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (60)

- [Abelian subgroup cannot have prime-power index in a nonabelian simple group](abelian-subgroup-cannot-have-prime-power-index-in-a-nonabelian-simple-group.md)
- [Adjoint-Higgs breaking of SU(3) to SU(2) and U(1)](adjoint-higgs-breaking-of-su-3-to-su-2-and-u-1.md)
- [Automorphisms of alternating groups from triple supports](automorphisms-of-alternating-groups-from-triple-supports.md)
- [Center of a group](center-of-a-group.md)
- [Centralizer](centralizer.md)
- [Centralizer and normalizer](centralizer-and-normalizer.md)
- [Centralizer of a regular permutation subgroup](centralizer-of-a-regular-permutation-subgroup.md)
- [Centralizer of a subset](centralizer-of-a-subset.md)
- [Class equation](class-equation.md)
- [Conjugacy class](conjugacy-class.md)
- [Conjugacy classes of the symmetric group on three letters](conjugacy-classes-of-the-symmetric-group-on-three-letters.md)
- [Least-prime divisibility constraint for a finite simple group](least-prime-divisibility-constraint-for-a-finite-simple-group.md)
- [Normalizer](normalizer.md)
- [P-radical subgroup](p-radical-subgroup.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-3/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-3/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-5/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/1c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-3/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-3/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/10g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/10g/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-4/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-4/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-4/3/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/7d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/8d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/8d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-103/1/c/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-3/1d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-102/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-138/6/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-138/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-151/1/solution.md)
- [Principal nilpotent element](principal-nilpotent-element.md)
- [Regular element of a semisimple Lie algebra](regular-element-of-a-semisimple-lie-algebra.md)
- [Rotational symmetry group of a regular dodecahedron](rotational-symmetry-group-of-a-regular-dodecahedron.md)
