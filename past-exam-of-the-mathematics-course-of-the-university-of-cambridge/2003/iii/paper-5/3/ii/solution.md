<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a null word $w$, define its area as the least number of conjugates of defining [relators](../../../../../../relator.md) or their inverses whose product is $w$ in the [free group](../../../../../../free-group.md). By the [van Kampen lemma](../../../../../../van-kampen-lemma.md), this is also its minimum number of [relator](../../../../../../relator.md) faces in a [disc diagram](../../../../../../disc-diagram.md). The [Dehn function](../../../../../../dehn-function.md) is

$$
\boxed{\delta_{\mathcal P}(n)=\max\{\operatorname{Area}_{\mathcal P}(w):|w|\le n,\ w=_G1\}}.
$$

The maximum is finite because there are finitely many words of bounded length. An [isoperimetric function of a group presentation](../../../../../../isoperimetric-function-of-a-group-presentation.md) is a nondecreasing upper bound on $\delta_{\mathcal P}$. Here subrecursive means bounded above by a total computable function, not merely recursively enumerable.

Suppose $\delta_{\mathcal P}(n)\le F(n)$ with $F$ computable. Let $\ell$ be the maximum [relator](../../../../../../relator.md) length, taking $\ell\ge1$ even if there are no [relators](../../../../../../relator.md). A minimum-area diagram for a boundary word of length $n$, with at most $N$ faces, can be chosen with no unnecessary tree branches. Every remaining edge occurs on a face boundary or the outside boundary, so there are at most $\ell N+n$ edges. Thus only finitely many combinatorial planar diagrams of area at most $N$ and this edge bound exist. Their finite edge labels and face labels can be enumerated, and the planar contractible diagram topology (allowing boundary spurs and pinched vertices), [relator](../../../../../../relator.md) face boundaries and outside boundary word can be checked by finite combinatorial operations.

For the input $w$, compute $N=F(|w|)$ and inspect all these diagrams. Answer yes if one has boundary $w$, and no otherwise. The diagram bound and [van Kampen lemma](../../../../../../van-kampen-lemma.md) prove correctness, including the negative answer. This finite search avoids the invalid attempt to bound area while allowing unbounded conjugating words.

Conversely, suppose a [word problem](../../../../../../word-problem-for-groups.md) decider is available. For each $n$, enumerate the finitely many words of length at most $n$ and use the decider to identify exactly the null words. For each such word search diagrams in increasing area, with the finite edge bound just given at each area. The search terminates, and the first successful area is its minimum area. Taking the maximum of these finitely many minima computes $\delta_{\mathcal P}(n)$. This proves the [recursive area bounds and the word problem](../../../../../../recursive-area-bounds-and-the-word-problem.md) equivalence:

$$
\boxed{\text{recursive isoperimetric upper bound}\quad\Longleftrightarrow\quad\text{decidable word problem}.}
$$

In fact, for [finite group presentations](../../../../../../finite-group-presentation.md), a word decider computes the minimal [Dehn function](../../../../../../dehn-function.md) itself.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
