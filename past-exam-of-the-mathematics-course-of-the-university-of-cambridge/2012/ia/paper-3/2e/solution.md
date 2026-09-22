<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

A [permutation cycle](../../../../../permutation-cycle.md) $(a_1\ a_2\ \cdots\ a_p)$ sends $a_1$ to $a_2$, each successive listed point to the next, and $a_p$ to $a_1$, fixing every unlisted point. Its length is $p$. For any [permutation](../../../../../permutation.md) $h$,

$$
h(a_1\ \cdots\ a_p)h^{-1}=(h(a_1)\ \cdots\ h(a_p)).
$$

Thus [conjugate group elements](../../../../../conjugate-group-elements.md) in the [symmetric group](../../../../../symmetric-group.md) have the same cycle length. Conversely, two cycles of the same length are conjugate: send their entries, in cyclic order, to one another and extend this [bijection](../../../../../bijection.md) arbitrarily to the unused points. Length-one cycles represent the identity and cause no exception to this conclusion.

An odd-length [permutation cycle](../../../../../permutation-cycle.md) is an [even permutation](../../../../../even-permutation.md), since its sign is $(-1)^{p-1}$. Let $c,d$ be such cycles on $p+2$ points and choose $h\in S_{p+2}$ with $hch^{-1}=d$. If $h$ is odd, let $t$ be the [transposition](../../../../../transposition-permutation.md) of the two points unused by the listed cycle $c$. Then $tc=ct$, and $ht$ is even with

$$
(ht)c(ht)^{-1}=hch^{-1}=d.
$$

Hence **all the $p$-cycles are conjugate within $A_{p+2}$**. The two spare letters supply the parity correction; they are the reason the same argument need not work with only one spare letter.

In $A_4$ the answer is **no**. For example, $(1\ 2\ 3)$ and $(1\ 3\ 2)$ are conjugated by the odd [transposition](../../../../../transposition-permutation.md) $(2\ 3)$ in $S_4$. The [centralizer](../../../../../centralizer.md) of $(1\ 2\ 3)$ in $S_4$ is exactly its order-three [cyclic subgroup](../../../../../cyclic-subgroup.md): a commuting [permutation](../../../../../permutation.md) fixes the unique fixed point $4$ and acts as a power of the cycle on the other three points. All these centralizing elements are even. Every other conjugating element differs from $(2\ 3)$ by a centralizing element, so it is also odd. There is no conjugator in $A_4$. Equivalently, the eight three-cycles split into two [conjugacy classes](../../../../../conjugacy-class.md) of size $12/3=4$, illustrating the [alternating conjugacy class splitting criterion](../../../../../alternating-conjugacy-class-splitting-criterion.md).

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
