<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the six-point matching geometry. A [duad](../../../../../../duad.md) is an edge of the [complete graph](../../../../../../complete-graph.md) on six points, a [syntheme](../../../../../../syntheme.md) is a [perfect matching](../../../../../../perfect-matching.md) of its three pairs, and a [pentad](../../../../../../total-of-synthemes.md) is a one-factorization: five pairwise edge-disjoint [synthemes](../../../../../../syntheme.md) covering all fifteen [duads](../../../../../../duad.md).

First count the [pentads](../../../../../../total-of-synthemes.md) without assuming their number. There are fifteen [synthemes](../../../../../../syntheme.md): the partner of the first point has five choices, the least remaining point then has three possible partners, and the last pair is forced. For a fixed [syntheme](../../../../../../syntheme.md) $M$, eight others share no edge with it: [inclusion-exclusion](../../../../../../inclusion-exclusion-principle.md) gives $15-3\cdot3+3\cdot1-1=8$. Two edge-disjoint [synthemes](../../../../../../syntheme.md) $M,M'$ have union a six-cycle. The complement of that cycle is a triangular prism, consisting of two triangles with three corresponding cross edges. It has precisely four [perfect matchings](../../../../../../perfect-matching.md): the all-cross matching and three matchings using one cross edge plus one edge from each triangle. The all-cross matching leaves two odd triangles and therefore cannot be completed by two matchings. The other three matchings are pairwise edge-disjoint and partition the prism. Hence $M,M'$ extend to exactly one [pentad](../../../../../../total-of-synthemes.md).

Each [pentad](../../../../../../total-of-synthemes.md) through $M$ uses four of its eight disjoint partners, and every partner gives exactly one completion. Thus $M$ lies in two [pentads](../../../../../../total-of-synthemes.md). Counting incidences gives $15\cdot2/5=6$ [pentads](../../../../../../total-of-synthemes.md) in total. Distinct [pentads](../../../../../../total-of-synthemes.md) cannot share two [synthemes](../../../../../../syntheme.md) because two disjoint [synthemes](../../../../../../syntheme.md) determine their unique completion. Every [syntheme](../../../../../../syntheme.md) therefore identifies a distinct pair of [pentads](../../../../../../total-of-synthemes.md); there are fifteen such pairs, so this incidence map is a bijection.

Permuting the six original points permutes the six [pentads](../../../../../../total-of-synthemes.md), defining a [group homomorphism](../../../../../../group-homomorphism.md) $\Phi:S_6\to\operatorname{Sym}(\text{pentads})$. It is faithful. If an element fixes every [pentad](../../../../../../total-of-synthemes.md), it fixes every [syntheme](../../../../../../syntheme.md) by the pair-incidence bijection. A [duad](../../../../../../duad.md) is the unique common edge of two distinct [synthemes](../../../../../../syntheme.md) containing it, so every [duad](../../../../../../duad.md) is fixed as well. A [permutation](../../../../../../permutation.md) fixing all two-element subsets fixes every point, by intersecting $\{i,j\}$ and $\{i,k\}$ for distinct $i,j,k$. The [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is therefore trivial. Both [groups](../../../../../../group-split.md) have order $6!$, so labeling the [pentads](../../../../../../total-of-synthemes.md) produces an [group automorphism](../../../../../../group-automorphism.md) of $S_6$.

It remains to prove this [group automorphism](../../../../../../group-automorphism.md) is outer. A [transposition](../../../../../../transposition-permutation.md), say $(1\ 2)$, fixes no [pentad](../../../../../../total-of-synthemes.md). If it fixed one, the unique [syntheme](../../../../../../syntheme.md) in that [pentad](../../../../../../total-of-synthemes.md) containing the [duad](../../../../../../duad.md) $\{1,2\}$ would be fixed. Every other [syntheme](../../../../../../syntheme.md) $M'$ in the [pentad](../../../../../../total-of-synthemes.md) contains 1 and 2 in separate edges. Swapping them changes those two edges but leaves the third edge unchanged. Hence $(1\ 2)M'$ is a distinct [syntheme](../../../../../../syntheme.md) sharing an edge with $M'$, impossible for two members of the same [pentad](../../../../../../total-of-synthemes.md). Thus $(1\ 2)$ acts without fixed points on the six [pentads](../../../../../../total-of-synthemes.md) and becomes a product of three disjoint [transpositions](../../../../../../transposition-permutation.md).

[Inner automorphisms](../../../../../../inner-automorphism.md) preserve [cycle type](../../../../../../cycle-type.md), whereas $\Phi$ sends a single [transposition](../../../../../../transposition-permutation.md) to a triple [transposition](../../../../../../transposition-permutation.md). Consequently

$$
\boxed{\Phi\text{ is an outer automorphism of }S_6.}
$$

This realizes the exceptional class-size coincidence from part (a). It is the full symmetric-group version of the [pentad construction of the exceptional alternating-group automorphism](../../../../../../pentad-construction-of-the-exceptional-alternating-group-automorphism.md), with faithfulness proved directly from incidence rather than borrowed from a simplicity theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
