<h1 id="5d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [permutation](../../../../../../permutation.md) $g$, start with a letter $i$ and follow $i,g(i),g^2(i),\ldots$. Finiteness gives a repetition; since $g$ is invertible, the first return is to $i$. The visited letters form a [permutation cycle](../../../../../../permutation-cycle.md) on which $g$ acts by moving to the next letter. If there are letters left, repeat the construction starting with one of them. Its trajectory cannot meet an earlier one, because applying a suitable inverse power of $g$ would put its starting letter in that earlier trajectory. Continuing partitions the letters into disjoint cycles, including fixed points as cycles of length one.

The resulting [disjoint permutation cycles](../../../../../../disjoint-permutation-cycles.md) have disjoint supports, and their product agrees with $g$ on every letter. This proves the [cycle decomposition of a permutation](../../../../../../cycle-decomposition-of-a-permutation.md). A power $g^m$ fixes a cycle of length $l$ exactly when $l\mid m$, so if the cycle lengths are $l_1,\ldots,l_t$,

$$
\boxed{\operatorname{ord}(g)=\operatorname{lcm}(l_1,\ldots,l_t).}
$$

The [least common multiple](../../../../../../least-common-multiple.md) is essential: multiplying the lengths would overcount whenever cycles share a factor.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
