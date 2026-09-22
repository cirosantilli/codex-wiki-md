<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Baire category theorem](../../../../../../baire-category-theorem.md) states that in a complete [metric space](../../../../../../metric-space.md), a [countable](../../../../../../countable-set.md) intersection of open [dense](../../../../../../dense-set.md) sets is [dense](../../../../../../dense-set.md). Equivalently, a nonempty [complete metric space](../../../../../../complete-metric-space.md) cannot be a [countable union](../../../../../../countable-union.md) of [nowhere dense sets](../../../../../../nowhere-dense-set.md), where a set is [nowhere dense](../../../../../../nowhere-dense-set.md) if its closure has empty interior.

Here is the proof. Let $G_1,G_2,\ldots$ be open [dense](../../../../../../dense-set.md) sets and let $U$ be any nonempty [open set](../../../../../../open-set.md). Choose a point $a_1\in U\cap G_1$ and a radius $0<r_1<1/2$ such that the [closed ball](../../../../../../closed-ball.md) $B_1=\overline B(a_1,r_1)$ lies inside $U\cap G_1$. Inductively choose $a_{m+1}$ in the nonempty [open set](../../../../../../open-set.md) $B(a_m,r_m)\cap G_{m+1}$, and then a radius $0<r_{m+1}<2^{-m-1}$ such that

$$
B_{m+1}=\overline B(a_{m+1},r_{m+1})\subseteq B(a_m,r_m)\cap G_{m+1}.
$$

Thus the [closed](../../../../../../closed-set.md) balls are nested and their radii tend to zero. For $j,k\geq m$, both centers lie in $B_m$, so $d(a_j,a_k)\leq2r_m$. They form a [Cauchy sequence](../../../../../../cauchy-sequence.md). [Completeness](../../../../../../completeness.md) gives a limit $a$, and closedness puts it in every $B_m$. Consequently $a\in U\cap\bigcap_mG_m$. As $U$ was arbitrary, **the intersection is [dense](../../../../../../dense-set.md)**.

To obtain the equivalent formulation, take complements of the closures of the [nowhere dense](../../../../../../nowhere-dense-set.md) sets; those complements are open [dense](../../../../../../dense-set.md). Conversely, complements of open [dense](../../../../../../dense-set.md) sets are [closed](../../../../../../closed-set.md) with empty interior. In particular, a [countable](../../../../../../countable-set.md) [closed](../../../../../../closed-set.md) cover of a nonempty [complete metric space](../../../../../../complete-metric-space.md) must contain a set with nonempty interior.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
