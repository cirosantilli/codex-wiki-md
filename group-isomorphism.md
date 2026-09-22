# Group isomorphism

↑ **Parent:** [Isomorphism](isomorphism.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_isomorphism)

A [group isomorphism](group-isomorphism.md) is a [bijective](bijection.md) [group homomorphism](group-homomorphism.md) $\varphi:G\to H$. It matches the entire [group operation](group-operation.md): $\varphi(ab)=\varphi(a)\varphi(b)$, with each product taken in its own [group](group-split.md). Its inverse is automatically a [group homomorphism](group-homomorphism.md). A [group automorphism](group-automorphism.md) is the special case $H=G$.[Definition 1.20](group-theory-v4-01-by-james-s-milne.md)

The target is part of the claim. The doubling example under [isomorphism](isomorphism.md) is a [group isomorphism](group-isomorphism.md) $d:\mathbb Z\to2\mathbb Z$, between the additive [integers](integer-split.md) and the additive [even integers](even-number.md). Exactly the same rule $d(k)=2k$, declared as $d:\mathbb Z\to\mathbb Z$, is an [injective](injective-function.md) [endomorphism](endomorphism.md) that misses $1$ and every other [odd integer](odd-integer.md), so is not a [group automorphism](group-automorphism.md). Changing the declared target changes [surjectivity](surjective-function.md), even though it does not change the formula or its compatibility with [addition](addition.md).

An [isomorphism](isomorphism.md) lets a calculation in one model solve the same problem in another. The example under [group](group-split.md) identifies [addition](addition.md) modulo four with [function composition](function-composition.md) of [rotations](rotation-mathematics.md) of a [square](square.md) via $k\mapsto r^k$. Through this [group isomorphism](group-isomorphism.md), adding exponents corresponds exactly to composing motions. More generally, a [group isomorphism](group-isomorphism.md) preserves [order of a group element](order-of-a-group-element.md), carries [subgroups](subgroup.md) to [subgroups](subgroup.md), and carries a [generating set of a group](generating-set-of-a-group.md) to a [generating set of a group](generating-set-of-a-group.md). Having equally many elements is insufficient: the [permutation](permutation.md) in [group automorphism](group-automorphism.md) already fails compatibility on two inputs.

Why does the inverse preserve the [group operation](group-operation.md)? Write $u=\varphi(a)$ and $v=\varphi(b)$, possible because of [surjectivity](surjective-function.md). Then

$$
\varphi^{-1}(uv)=\varphi^{-1}(\varphi(a)\varphi(b))=\varphi^{-1}(\varphi(ab))=ab=\varphi^{-1}(u)\varphi^{-1}(v).
$$

This proves the inverse condition directly. Analogous calculations work for each operation of a [ring](ring.md) and for [addition](addition.md) and [scalar multiplication](scalar-multiplication.md) in a [vector space](vector-space-split.md). The argument relies on preserving those operations; it supplies no general continuity claim for the inverse of a [continuous](continuous-function.md) [bijection](bijection.md) between [topological spaces](topological-space.md).

## ↑ Ancestors (6)

1. [Isomorphism](isomorphism.md)
2. [Morphism](morphism.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (57)

- [Abelian plane subgroup of a finite Heisenberg group](abelian-plane-subgroup-of-a-finite-heisenberg-group.md)
- [Conjugate subgroup](conjugate-subgroup.md)
- [Cyclic group of order four and Klein four-group](cyclic-group-of-order-four-and-klein-four-group.md)
- [Cyclicity of a product of two finite cyclic groups](cyclicity-of-a-product-of-two-finite-cyclic-groups.md)
- [Endomorphism](endomorphism.md)
- [Finite cyclic group](finite-cyclic-group.md)
- [First isomorphism theorem](first-isomorphism-theorem.md)
- [Group](group-split.md)
- [Group automorphism](group-automorphism.md)
- [Group isomorphism](group-isomorphism.md)
- [Group of order eight](group-of-order-eight.md)
- [Integer shear group](integer-shear-group.md)
- [Internal direct product theorem](internal-direct-product-theorem.md)
- [Isomorphism](isomorphism.md)
- [Lie group isomorphism](lie-group-isomorphism.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3/8d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-23/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-3/5d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-18/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-14/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-29/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-3/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/10g/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-1/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-26/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/20i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-151/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/8/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/8/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/8/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/8/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/8/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2/10/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/8/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/9/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/9/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/9/a/solution.md)
- [Schreier refinement theorem](schreier-refinement-theorem.md)
- [Shifted addition on odd integers](shifted-addition-on-odd-integers.md)
- [Special orthogonal group in two dimensions](special-orthogonal-group-in-two-dimensions.md)
- [Subgroup of an infinite cyclic group](subgroup-of-an-infinite-cyclic-group.md)
- [Symmetry depends on preserved structure](symmetry-depends-on-preserved-structure.md)
- [Topological invariant](topological-invariant.md)
