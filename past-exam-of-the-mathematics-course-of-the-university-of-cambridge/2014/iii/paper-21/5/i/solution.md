<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [well-quasi-ordering](../../../../../../well-quasi-ordering.md) is a reflexive transitive relation for which every infinite [sequence](../../../../../../sequence.md) has $i<j$ with $x_i\le x_j$. A [bad sequence](../../../../../../bad-sequence.md) has no such pair. **The [labelled version of Kruskal's tree theorem](../../../../../../labelled-version-of-kruskal-s-tree-theorem.md) says that finite [rooted trees](../../../../../../rooted-tree.md) labelled in any [well-quasi-ordering](../../../../../../well-quasi-ordering.md) are themselves [well-quasi-ordered](../../../../../../well-quasi-ordering.md) by [label-monotone tree embedding](../../../../../../label-monotone-tree-embedding.md).**

More explicitly, an embedding is an injective map of vertices preserving [lowest common ancestors](../../../../../../lowest-common-ancestor.md), and satisfying $\ell_T(v)\le\ell_S(h(v))$ at every vertex. The root need not map to the host root. This is a [homeomorphic embedding of a rooted tree](../../../../../../homeomorphic-embedding-of-a-rooted-tree.md): an edge can map to a longer path, but distinct branches must separate at the image of their common ancestor. We shall prove the stronger version in which every vertex's children are linearly ordered and embeddings respect that ordering. Forgetting the child order gives the stated result for unordered [rooted trees](../../../../../../rooted-tree.md).

We first establish the two [well-quasi-ordering](../../../../../../well-quasi-ordering.md) facts used in the proof. Every infinite [sequence](../../../../../../sequence.md) in a [well-quasi-ordering](../../../../../../well-quasi-ordering.md) has an infinite nondecreasing [subsequence](../../../../../../subsequence.md). Indeed, color an index pair $i<j$ according to whether $x_i\le x_j$. The infinite two-color [Ramsey theorem](../../../../../../ramsey-theorem.md) gives a homogeneous infinite set; the negative color would be a [bad sequence](../../../../../../bad-sequence.md), so the positive color gives the required [subsequence](../../../../../../subsequence.md). It follows that the componentwise product of two [well-quasi-orderings](../../../../../../well-quasi-ordering.md) is a [well-quasi-ordering](../../../../../../well-quasi-ordering.md): first extract a nondecreasing [subsequence](../../../../../../subsequence.md) in one coordinate, then find a good pair in the other.

Next prove [Higman lemma](../../../../../../higman-s-lemma.md): finite [words](../../../../../../string.md) over a [well-quasi-ordering](../../../../../../well-quasi-ordering.md) $Q$, ordered by subsequence embedding with coordinatewise increase of letters, are a [well-quasi-ordering](../../../../../../well-quasi-ordering.md). Suppose not, and choose a [minimal bad sequence](../../../../../../minimal-bad-sequence.md) $w_0,w_1,\ldots$ by making the length of $w_n$ minimal among all choices admitting an infinite bad continuation of the already fixed prefix. No [word](../../../../../../string.md) is the [empty word](../../../../../../empty-word.md), since that embeds in every later [word](../../../../../../string.md). Write $w_n=v_na_n$ with $a_n\in Q$. Extract indices $i_0<i_1<\cdots$ for which $a_{i_0}\le a_{i_1}\le\cdots$. Consider

$$
w_0,\ldots,w_{i_0-1},v_{i_0},v_{i_1},\ldots.
$$

It cannot be a [bad sequence](../../../../../../bad-sequence.md), since its first replacement is shorter than the minimal choice $w_{i_0}$. But a good pair within the original prefix is impossible. A prefix [word](../../../../../../string.md) embedding into $v_{i_j}$ would embed into $w_{i_j}$, contradicting the original [bad sequence](../../../../../../bad-sequence.md). And $v_{i_j}$ embedding into $v_{i_k}$ would, after appending the ordered last letters, embed $w_{i_j}$ into $w_{i_k}$, also impossible. This contradiction proves [Higman lemma](../../../../../../higman-s-lemma.md), including [words](../../../../../../string.md) of arbitrary finite length.

Now suppose there is a [bad sequence](../../../../../../bad-sequence.md) of finite ordered labelled [rooted trees](../../../../../../rooted-tree.md). Choose a [minimal bad sequence](../../../../../../minimal-bad-sequence.md) $T_0,T_1,\ldots$ by minimizing the number of vertices of $T_n$, subject to the fixed prefix having an infinite bad continuation. Existence of a least possible size uses ordinary well-ordering of the natural numbers; after selecting such a tree retain a bad continuation to make the next choice.

Let $\mathcal S$ be the collection of all proper rooted subtrees of all $T_n$, with inherited labels and child ordering. These are the subtrees rooted at vertices other than the root, and each embeds into its containing tree. We claim $\mathcal S$ is a [well-quasi-ordering](../../../../../../well-quasi-ordering.md) under the same [label-monotone tree embedding](../../../../../../label-monotone-tree-embedding.md).

Otherwise choose a [bad sequence](../../../../../../bad-sequence.md) $U_0,U_1,\ldots$ from $\mathcal S$, and choose for each a containing tree $T_{n_j}$. The indices $n_j$ are unbounded in every tail: finitely many containing trees have only finitely many rooted subtrees, and an infinite [bad sequence](../../../../../../bad-sequence.md) cannot repeatedly use one of these, since it embeds into itself. Passing to a [subsequence](../../../../../../subsequence.md), arrange $n_0<n_1<\cdots$. The spliced [sequence](../../../../../../sequence.md)

$$
T_0,\ldots,T_{n_0-1},U_0,U_1,\ldots
$$

is bad. A good pair within either piece is already excluded. A comparison $T_k\preceq U_j$, where $k<n_0\le n_j$, would compose with $U_j\preceq T_{n_j}$ to give $T_k\preceq T_{n_j}$, contradicting the original [bad sequence](../../../../../../bad-sequence.md). But $U_0$ is smaller than $T_{n_0}$, contradicting the minimal choice at that position. This proves the claim about $\mathcal S$.

Describe $T_n$ by its root label $q_n\in Q$ and its finite ordered list $C_n$ of child subtrees. Every entry of $C_n$ lies in $\mathcal S$. By [Higman lemma](../../../../../../higman-s-lemma.md), $\mathcal S^*$ is a [well-quasi-ordering](../../../../../../well-quasi-ordering.md); hence so is $Q\times\mathcal S^*$. There exist $i<j$ with $q_i\le q_j$ and an increasing injection matching the child subtrees in $C_i$ to child subtrees in $C_j$, each by an embedding. Map root to root and combine these child embeddings. Different matched children lie in different target branches, so their paths meet exactly at the target root; within each branch the chosen embedding already preserves [lowest common ancestors](../../../../../../lowest-common-ancestor.md). The resulting map is a [label-monotone tree embedding](../../../../../../label-monotone-tree-embedding.md) $T_i\preceq T_j$, a contradiction. Therefore

$$
\boxed{Q\text{ wqo}\quad\Longrightarrow\quad\mathcal T(Q)\text{ wqo under labelled homeomorphic embedding}.}
$$

The empty labelled tree, if included by convention, embeds into every tree and causes no exception. A common stronger formulation requires the source root to map to the target root. It also follows: the theorem just proved makes all labelled child subtrees a [well-quasi-ordering](../../../../../../well-quasi-ordering.md), and the product $Q\times\mathcal T(Q)^*$ then provides a good pair with roots explicitly matched, by the same final assembly. Internal child roots may map further down their matched branches. This must not be confused with edge-to-edge embedding, for which the theorem is false in general.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
