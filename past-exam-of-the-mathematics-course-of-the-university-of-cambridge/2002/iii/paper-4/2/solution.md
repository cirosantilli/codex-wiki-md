<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Ohnishi orderability criterion](../../../../../ohnishi-orderability-criterion.md) states that, for each finite list $g_1,\ldots,g_n\ne1$, there are signs $\varepsilon_i\in\{-1,1\}$ such that the [semigroup](../../../../../semigroup.md) of nonempty products of conjugates of $g_i^{\varepsilon_i}$ does not contain $1$. The conjugates are essential for a two-sided invariant [total order](../../../../../total-order.md). Necessity follows by choosing all signed elements positive: their conjugates and nonempty products are still positive.

For sufficiency, consider the compact product $\{+,-\}^{G\setminus\{1\}}$. Impose the closed conditions that an inverse has the opposite sign, that conjugation preserves sign, and that a product of two positive elements is positive whenever it is nonidentity. A positive pair cannot multiply to the identity because of the inverse condition. Each condition uses finitely many coordinates. Given finitely many conditions, collect every nonidentity element appearing in them into a finite list and choose signs using the criterion. These signs satisfy the conditions: an incorrectly negative product would contribute its positive inverse to the generated [semigroup](../../../../../semigroup.md), producing identity with the positive factors; an incorrect conjugate or inverse gives the same contradiction. Extend the signs arbitrarily to the remaining coordinates. Thus the finite intersection property and compactness give a global sign assignment. Its positive elements form a conjugation-invariant [semigroup](../../../../../semigroup.md) $S$ with $S\cap S^{-1}=\varnothing$ and $S\cup S^{-1}=G\setminus\{1\}$. Defining $a<b$ by $a^{-1}b\in S$ gives the required [linearly ordered group](../../../../../linearly-ordered-group.md).

Restriction shows that every [finitely generated subgroup](../../../../../finitely-generated-subgroup.md) of an orderable [group](../../../../../group-split.md) is orderable. Conversely, suppose every such subgroup is orderable. If the criterion failed on $g_1,\ldots,g_n$, each of the finitely many sign choices would have an identity witness made of finitely many conjugates. Collect all $g_i$ and all conjugating elements in these witnesses into one [finitely generated subgroup](../../../../../finitely-generated-subgroup.md) $H$. An order on $H$ supplies one positive sign choice, but its corresponding witness is a nonempty product of positive elements in $H$, a contradiction. Hence the criterion holds in $G$.

Finally, a [finitely generated subgroup](../../../../../finitely-generated-subgroup.md) of a [torsion-free abelian group](../../../../../torsion-free-abelian-group.md) is $\mathbb Z^r$ by the [Fundamental theorem of finitely generated abelian groups](../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md). Its [lexicographic order](../../../../../lexicographic-order.md) is two-sided invariant. Applying the local-to-global conclusion proves that every [torsion-free abelian group](../../../../../torsion-free-abelian-group.md) admits the required order.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
