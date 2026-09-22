<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each symbol $a$, iterate the [permutation](../../../../../../../permutation.md) $\sigma$. Since the symbol set is finite, some iterate repeats. Applying an inverse power of $\sigma$ shows that the first return is to $a$ itself, giving

$$
a,\sigma(a),\ldots,\sigma^{k-1}(a),\qquad\sigma^k(a)=a,
$$

with the displayed symbols distinct. This is a [permutation cycle](../../../../../../../permutation-cycle.md). If two such lists share a symbol, applying powers of $\sigma$ shows that they contain exactly the same symbols. Hence these [group orbits](../../../../../../../orbit-group-theory.md) form a [partition of a set](../../../../../../../partition-of-a-set.md) $\{1,\ldots,n\}$. On each [group orbit](../../../../../../../orbit-group-theory.md), $\sigma$ acts as the corresponding [permutation cycle](../../../../../../../permutation-cycle.md), and these [disjoint permutation cycles](../../../../../../../disjoint-permutation-cycles.md) multiply to $\sigma$.

The [disjoint cycle decomposition](../../../../../../../disjoint-cycle-decomposition.md) is **unique up to reordering the cycles and cyclically rotating the entries within each cycle**, with fixed points optionally omitted. Indeed, each cycle must consist of one of the uniquely determined [group orbits](../../../../../../../orbit-group-theory.md), and its successive entries must follow the action of $\sigma$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
