<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Acting separately on disjoint sets of four and eight symbols embeds the [direct product of groups](../../../../../../direct-product-of-groups.md) $S_4\times S_8$ into $S_{12}$. The action is injective since fixing all twelve symbols forces both factors to be identities.

For the lower bound, $S_4$ contains a cycle of order four and $S_8$ contains disjoint cycles of lengths five and three, whose product has order fifteen. The corresponding element of $S_4\times S_8$ has [order of a group element](../../../../../../order-of-a-group-element.md) $\operatorname{lcm}(4,15)=60$. Every isomorphic subgroup of $S_n$ must therefore contain a [permutation](../../../../../../permutation.md) of order sixty. We can bound the [minimum number of symbols for a permutation of prescribed order](../../../../../../minimum-number-of-symbols-for-a-permutation-of-prescribed-order.md) directly here.

In the [disjoint cycle decomposition](../../../../../../disjoint-cycle-decomposition.md) of such a [permutation](../../../../../../permutation.md), all cycle lengths divide $60$, and their [least common multiple](../../../../../../least-common-multiple.md) must contain the factors $4$, $3$, and $5$. If these factors occur in three distinct cycles, those cycles use at least $4+3+5=12$ symbols. If two occur in the same cycle, that cycle has length at least their product: combining $4,3$ costs at least $12$, combining $4,5$ costs at least $20$, and combining $3,5$ costs at least $15$. Each possibility already requires at least twelve symbols. Thus $n\geq12$, and

$$
\boxed{n_{\min}=12.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
