# Direct product of groups

↑ **Parent:** [Group theory](group-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Direct_product_of_groups)

A direct product combines two [groups](group-split.md) into one while keeping their operations in separate coordinates. Its underlying [set](set-split.md) is the [Cartesian product](cartesian-product.md) $G\times H$, and its [group operation](group-operation.md) is

$$
(g_1,h_1)(g_2,h_2)=(g_1g_2,h_1h_2).
$$

The [identity element](identity-element.md) is $(e_G,e_H)$, and the [inverse element](inverse-element.md) of $(g,h)$ is $(g^{-1},h^{-1})$. [Associativity](associative-property.md) follows coordinate by coordinate. For finite [groups](group-split.md), the [multiplication principle](rule-of-product.md) gives $|G\times H|=|G||H|$.

For example, write the [cyclic group](cyclic-group.md) $C_m$ as the additive [group](group-split.md) of [residue classes](residue-class.md) modulo $m$. In $C_2\times C_3$,

$$
(1,2)+(1,2)=(0,1),
$$

since each coordinate reduces with its own [integer modulus](modulus-in-modular-arithmetic.md). A pair can track two cyclic counters that advance independently. Updating the first coordinate does not alter the second, and vice versa.

This independence has an algebraic form. The embedded factor elements always [commute](commuting-elements.md):

$$
(g,e_H)(e_G,h)=(g,h)=(e_G,h)(g,e_H).
$$

The coordinate maps $(g,h)\mapsto g$ and $(g,h)\mapsto h$ are [group homomorphisms](group-homomorphism.md), so one can analyze either component separately. This does not make the full product an [abelian group](abelian-group.md) when one of its factors is nonabelian: two arbitrary pairs need not [commute](commuting-elements.md).

The construction is useful in both directions. It builds a larger [group](group-split.md) from familiar pieces, while the [internal direct product theorem](internal-direct-product-theorem.md) recognizes when an existing [group](group-split.md) can be separated into such pieces. A [cyclic group](cyclic-group.md) can sometimes be split this way; whether two finite cyclic factors combine into one [cyclic group](cyclic-group.md) is decided by the [cyclicity of a product of two finite cyclic groups](cyclicity-of-a-product-of-two-finite-cyclic-groups.md). Definitions and the basic recognition theorems are developed in [Thomas Judson, Abstract Algebra: Theory and Applications, §9.2, Direct Products](https://judsonbooks.org/aata-files/aata-html/isomorph-section-direct-products.html).

**Table of contents**

- [Direct product of cyclic groups of orders four and two](direct-product-of-cyclic-groups-of-orders-four-and-two.md)
  - [Subgroups of C4 times C2](subgroups-of-c4-times-c2.md)
- [Cyclicity of a product of two finite cyclic groups](cyclicity-of-a-product-of-two-finite-cyclic-groups.md)
- [Order of a direct-product element](order-of-a-direct-product-element.md)
- [Restricted direct sum of groups](restricted-direct-sum-of-groups.md)
- [Internal direct product theorem](internal-direct-product-theorem.md)

## ↑ Ancestors (5)

1. [Group theory](group-theory-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (58)

- [Abelian plane subgroup of the Heisenberg group modulo four](abelian-plane-subgroup-of-the-heisenberg-group-modulo-four.md)
- [Body-diagonal stabilizer in the cube symmetry group](body-diagonal-stabilizer-in-the-cube-symmetry-group.md)
- [Canonical Coleman decomposition of power-series units](canonical-coleman-decomposition-of-power-series-units.md)
- [Carmichael function](carmichael-function.md)
- [Category of groups](category-of-groups.md)
- [Category theory](category-theory-split.md)
- [Classification of groups of order p squared](classification-of-groups-of-order-p-squared.md)
- [Dihedral splitting when the half-rotation order is odd](dihedral-splitting-when-the-half-rotation-order-is-odd.md)
- [Direct-product decomposition of the cube symmetry group](direct-product-decomposition-of-the-cube-symmetry-group.md)
- [Direct product of cyclic groups of orders four and two](direct-product-of-cyclic-groups-of-orders-four-and-two.md)
- [Exact factorization of a group](exact-factorization-of-a-group.md)
- [Finite abelian group](finite-abelian-group.md)
- [Finite nilpotent group decomposition](finite-nilpotent-group-decomposition.md)
- [Internal direct product theorem](internal-direct-product-theorem.md)
- [Nilpotency class of a direct product](nilpotency-class-of-a-direct-product.md)
- [Normal subgroups of coprime order commute](normal-subgroups-of-coprime-order-commute.md)
- [Odd-dimensional orthogonal determinant splitting](odd-dimensional-orthogonal-determinant-splitting.md)
- [P-elementary group](p-elementary-group.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3/8d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-3/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-7/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-1/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-1/6/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-7/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/1d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/5d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/6d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/8d/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/8d/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-104/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-104/6/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-3/5d/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/9g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/8/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/9/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/8/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/9/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/8/f/solution.md)
- [Permutation wreath product](permutation-wreath-product.md)
- [Prime-set decomposition of elementary groups](prime-set-decomposition-of-elementary-groups.md)
- [Restricted direct sum of groups](restricted-direct-sum-of-groups.md)
- [Section normal form for a split group extension](section-normal-form-for-a-split-group-extension.md)
