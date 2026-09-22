# Orbit-stabilizer theorem

↑ **Parent:** [Group action](group-action-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbit-stabilizer_theorem)

For a [group action](group-action-split.md) of any [group](group-split.md) $G$ on a [set](set-split.md) $X$, the [cardinality](cardinality.md) of the [orbit of a group action](orbit-group-theory.md) through $x$ is the [index of a subgroup](index-of-a-subgroup.md) of its [stabilizer subgroup](stabilizer-subgroup.md):

$$
|Gx|=[G:G_x],\qquad G_x=\{g\in G:g\cdot x=x\}.
$$

In particular, if $G$ is a [finite group](finite-group.md),

$$
|G|=|Gx|\,|G_x|,\qquad |Gx|=\frac{|G|}{|G_x|}.
$$

For a fixed [finite group](finite-group.md), a larger [stabilizer subgroup](stabilizer-subgroup.md) means a smaller [group orbit](orbit-group-theory.md): more transformations repeat the same image of $x$. The [set](set-split.md) $X$ itself need not be finite.

The underlying [bijection](bijection.md) uses left [cosets](coset.md), without requiring $G_x$ to be a [normal subgroup](normal-subgroup.md):

$$
\Phi:\{gG_x:g\in G\}\longrightarrow Gx,\qquad gG_x\longmapsto g\cdot x.
$$

To check it briefly, replacing $g$ by $gh$ with $h\in G_x$ preserves $g\cdot x$, so $\Phi$ is well-defined. Every member of the [group orbit](orbit-group-theory.md) has this form. Finally, $g\cdot x=k\cdot x$ implies $k^{-1}g\in G_x$, hence $gG_x=kG_x$, proving the [bijection](bijection.md). This is the construction in [MIT's group-action notes, lemma 23.5](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/96221ce2d5b1077b3e5d3c5e08c88afe_MIT18_703S13_pra_l_23.pdf). For infinite [groups](group-split.md), the [bijection](bijection.md) and the [cardinality](cardinality.md) statement $|Gx|=[G:G_x]$ still hold; division of infinite [cardinalities](cardinality.md) does not supply the finite formula.

For the eight-element [dihedral group](dihedral-group.md) $D_4$ acting on the [square](square.md) described under [group action](group-action-split.md), moving a marked [vertex of a polygon](vertex-of-a-polygon.md) gives $8=4\cdot2$. Moving a marked [side of a polygon](side-of-a-polygon.md) also gives $8=4\cdot2$; moving one unoriented [diagonal of a polygon](diagonal-of-a-polygon.md) gives $8=2\cdot4$; moving the [centroid](centroid.md) gives $8=1\cdot8$. These are four different [group actions](group-action-split.md), each with one [group orbit](orbit-group-theory.md). In the first [group action](group-action-split.md), the four left [cosets](coset.md) of $H=G_A=\{e,s\}$ are

$$
H=\{e,s\},\quad rH=\{r,rs\},\quad r^2H=\{r^2,r^2s\},\quad r^3H=\{r^3,r^3s\}.
$$

They correspond respectively to $A,B,C,D$. Counting all eight transformations would count each position of the marked [vertex of a polygon](vertex-of-a-polygon.md) twice.

<a id="image-cosets-explain-the-orbit-stabilizer-theorem-for-a-square"></a>
![](orbit-stabilizer-cosets.png)

**[Figure 9](#image-cosets-explain-the-orbit-stabilizer-theorem-for-a-square). Cosets explain the orbit-stabilizer theorem for a square**. The left panel matches four left [cosets](coset.md) of a [stabilizer subgroup](stabilizer-subgroup.md) to four images of a [vertex of a polygon](vertex-of-a-polygon.md). The right panel compares the [group orbits](orbit-group-theory.md) for separate [group actions](group-action-split.md) on [vertices of a polygon](vertex-of-a-polygon.md), [sides of a polygon](side-of-a-polygon.md), [diagonals of a polygon](diagonal-of-a-polygon.md), and the [centroid](centroid.md); each [group orbit](orbit-group-theory.md) size times the corresponding [stabilizer subgroup](stabilizer-subgroup.md) [group order](order-of-a-finite-group.md) equals eight.

For a second computed example, let the [symmetric group](symmetric-group.md) $S_3$ act on the [Cartesian product](cartesian-product.md) $X=\{1,2,3\}^2$ by $\sigma\cdot(i,j)=(\sigma(i),\sigma(j))$. There are two [orbits of a group action](orbit-group-theory.md):

$$
S_3\cdot(1,1)=\{(1,1),(2,2),(3,3)\},\qquad (S_3)_{(1,1)}=\{e,(23)\},
$$

and

$$
S_3\cdot(1,2)=\{(1,2),(1,3),(2,1),(2,3),(3,1),(3,2)\},\qquad (S_3)_{(1,2)}=\{e\}.
$$

The first [stabilizer subgroup](stabilizer-subgroup.md) can exchange $2$ and $3$ while fixing $1$; the second must fix both $1$ and $2$, so also fixes $3$. The [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) gives $6=3\cdot2$ and $6=6\cdot1$, and the two [group orbit](orbit-group-theory.md) sizes account for all nine [ordered pairs](ordered-pair.md). The general reason for exactly these two [group orbits](orbit-group-theory.md) is [equality-pattern orbits of ordered pairs](equality-pattern-orbits-of-ordered-pairs.md).

**Table of contents**

- [Orbit dimension formula](orbit-dimension-formula.md)

## ↑ Ancestors (6)

1. [Group action](group-action-split.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (89)

- [Central intersection property of normal subgroups of finite p-groups](central-intersection-property-of-normal-subgroups-of-finite-p-groups.md)
- [Class equation](class-equation.md)
- [Colour-preserving symmetry group](colour-preserving-symmetry-group.md)
- [Conjugacy class](conjugacy-class.md)
- [Conjugacy class splitting in a prime-index normal subgroup](conjugacy-class-splitting-in-a-prime-index-normal-subgroup.md)
- [Cube symmetry action on edges](cube-symmetry-action-on-edges.md)
- [Double coset](double-coset.md)
- [Faithful coset action of the symmetric group on three letters](faithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Fano point-line stabilizer intersection](fano-point-line-stabilizer-intersection.md)
- [Free group action](free-group-action.md)
- [Group action](group-action-split.md)
- [Lagrange's theorem](lagrange-s-theorem.md)
- [Minimal faithful permutation degree of the quaternion group](minimal-faithful-permutation-degree-of-the-quaternion-group.md)
- [Nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Normalizer](normalizer.md)
- [Orbit (group theory)](orbit-group-theory.md)
- [Orbit-stabilizer theorem](orbit-stabilizer-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-77/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/1b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/1b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/7b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/7b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/1c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/19g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-31/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/11e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/11g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/11g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-7/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-7/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/10g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/19f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/5d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-26/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/1d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/7d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/7d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/8d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/5e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/5e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-81/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-81/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-3/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-3/3/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/7d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/5d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/7d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/8d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2/11e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-119/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/7e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/17g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-3/1d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-138/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-2/6e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/19f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-3/6d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/9g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/9e/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-3/8d/a/solution.md)
- [Regular icosahedron](regular-icosahedron.md)
- [Simply transitive group action](simply-transitive-group-action.md)
- [Skyrmion stabilizer and collective-coordinate orbit](skyrmion-stabilizer-and-collective-coordinate-orbit.md)
- [SL2 action on a finite projective line](sl2-action-on-a-finite-projective-line.md)
- [Stabilizer subgroup](stabilizer-subgroup.md)
- [Tetrahedron stabilizer in the cube rotation group](tetrahedron-stabilizer-in-the-cube-rotation-group.md)
- [Transitive group action](transitive-group-action.md)
