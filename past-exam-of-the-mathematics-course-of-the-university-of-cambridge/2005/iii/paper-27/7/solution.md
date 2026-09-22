<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [well-quasi-ordering](../../../../../well-quasi-ordering.md) is a [preorder](../../../../../preorder.md) $\le$ for which every infinite sequence has $i<j$ with $x_i\le x_j$. Such a comparable pair is good; a sequence without one is a [bad sequence](../../../../../bad-sequence.md). Equivalently there is no infinite strictly descending chain in the quotient order and no infinite antichain.

A [better-quasi-ordering](../../../../../better-quasi-ordering.md) strengthens this by requiring every barrier array to be good. A [barrier in better-quasi-order theory](../../../../../barrier-in-better-quasi-order-theory.md) on an infinite $A\subseteq\omega$ is a family $B$ of nonempty finite increasing sequences, no one properly contained in another, such that every infinite subset of $A$ has an initial segment in $B$. Write $s\triangleleft t$ when $s$ is an initial segment of a finite increasing sequence $u$ and $t$ is an initial segment of $u$ with its first entry deleted. A map $f:B\to Q$ is good if some $s\triangleleft t$ satisfy $f(s)\le f(t)$. Requiring this for all barriers defines a [better-quasi-ordering](../../../../../better-quasi-ordering.md). Singleton barriers recover [well-quasi-ordering](../../../../../well-quasi-ordering.md); the stronger property supports infinitary closure operations that can fail for a mere well-quasi-ordering.

The [labelled version of Kruskal's tree theorem](../../../../../labelled-version-of-kruskal-s-tree-theorem.md) states that finite rooted trees labelled in a well-quasi-order $Q$ are well-quasi-ordered under label-monotone [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md). An embedding sends edges to nonempty downward paths, separates different child branches, and increases labels. Initially allow the source root to land at any vertex of the target. We prove this version; forcing roots to match follows at the end.

Suppose there is a bad sequence $T_0,T_1,\ldots$. Choose it as a [minimal bad sequence](../../../../../minimal-bad-sequence.md): at each stage choose a tree with the fewest vertices among those admitting a bad continuation of the already fixed prefix. Let $U$ contain all proper rooted descendant subtrees of these trees. We first show that $U$ is well-quasi-ordered by the same root-flexible embedding.

Otherwise choose a bad sequence $S_0,S_1,\ldots$ from $U$. Each finite collection of the $T_n$ has only finitely many descendant subtrees, and a bad sequence cannot repeat an object. Thus, after passing to a subsequence, choose strictly increasing $n_i$ such that $S_i$ is a proper descendant subtree of $T_{n_i}$. The sequence

$$
T_0,\ldots,T_{n_0-1},S_0,S_1,\ldots
$$

is bad: an embedding of a prefix tree $T_k$ into $S_i$ would compose with the subtree inclusion to embed $T_k$ into $T_{n_i}$, contradicting the original badness. But $S_0$ is smaller than $T_{n_0}$, contradicting minimality. Hence $U$ is well-quasi-ordered.

Give the children of each root any fixed linear order, and describe a tree by its root label and the word of its child subtrees. The [Higman lemma](../../../../../higman-s-lemma.md) makes $U^*$ well-quasi-ordered, and [finite product closure of well-quasi-orderings](../../../../../finite-product-closure-of-well-quasi-orderings.md) makes $Q\times U^*$ well-quasi-ordered. There are therefore $i<j$ with an increased root label and an embedding of the child word of $T_i$ as a subsequence of that of $T_j$. Embed the root into the root, use the chosen subtree embeddings inside the corresponding distinct target branches, and join their root images to the target root by downward paths. This gives a label-monotone tree embedding $T_i\to T_j$, the required contradiction.

If root-preserving embeddings are required, replace $Q$ by the disjoint union of two copies of $Q$, label every root in copy one and every other vertex in copy zero, and allow comparisons only within a copy. This is again a well-quasi-order. The unique copy-one vertex of a tree forces an embedding to send root to root. Taking $Q$ to be a singleton gives [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md) for unlabelled trees. The [Higman lemma](../../../../../higman-s-lemma.md) used above follows from the same minimal-bad-sequence argument for words: delete the last letters along an infinite nondecreasing subsequence of those letters; a good pair among the shortened words would extend to a good pair of original words, contradicting minimality. Empty shortened words cause an immediate good pair. This supplies the word lemma needed in the tree proof.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
