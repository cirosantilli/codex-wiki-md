<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [decidable object in a topos](../../../../../../decidable-object-in-a-topos.md) has a decomposition $A\times A=\Delta_A\amalg D_A$, with $D_A$ representing inequality. In the [internal logic of a topos](../../../../../../internal-logic-of-a-topos.md), equality on $A$ is decidable. These categorical complements behave well under [pullback](../../../../../../pullback-category-theory.md).

For a [subobject](../../../../../../subobject.md) $B\hookrightarrow A$, pull back the displayed decomposition along $B\times B\hookrightarrow A\times A$. The diagonal pulls back to $\Delta_B$, while $D_A$ pulls back to its complement. Hence **every [subobject](../../../../../../subobject.md) of a decidable object is decidable**; the [subobject](../../../../../../subobject.md) itself need not be complemented in $A$.

For two decidable objects, the diagonals of $A$ and $B$ give four disjoint summands of $(A\times B)^2$, according as each coordinate pair is equal or unequal. The both-equal summand is $\Delta_{A\times B}$, and the other three give its complement. The [terminal object](../../../../../../terminal-object.md) is decidable, so induction gives **closure under finite products**, including the empty product.

For a family $(A_i)_{i\in I}$ of decidable objects with an existing [coproduct](../../../../../../coproduct.md) $A=\coprod_iA_i$, products distribute over this [coproduct](../../../../../../coproduct.md), giving

$$
A\times A\cong\coprod_{i,j\in I}(A_i\times A_j).
$$

The [coproduct](../../../../../../coproduct.md) injections in a topos are disjoint. The diagonal consists of $\Delta_{A_i}$ in each $i=j$ summand, and has complement

$$
\boxed{\left(\coprod_iD_{A_i}\right)\amalg\left(\coprod_{i\ne j}A_i\times A_j\right).}
$$

Consequently **every existing [coproduct](../../../../../../coproduct.md) of decidable objects is decidable**, including the [initial object](../../../../../../initial-object.md). In a [Grothendieck topos](../../../../../../grothendieck-topos.md) all small [coproducts](../../../../../../coproduct.md) exist. No assertion that arbitrary products preserve decidability is used.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
