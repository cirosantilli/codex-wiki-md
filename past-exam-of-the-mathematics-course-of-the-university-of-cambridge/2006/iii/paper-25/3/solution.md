<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md): edges may be stretched into downward paths, different child branches stay disjoint, and the source root may map to any target vertex. Write $S\preceq T$ for this relation. More generally allow labels in a [well-quasi-ordering](../../../../../well-quasi-ordering.md) $Q$ and require every source label to be at most its image label. We prove this labelled version, which includes the unlabelled case by taking one label.

First, every infinite [sequence](../../../../../sequence.md) in a [well-quasi-ordering](../../../../../well-quasi-ordering.md) has an infinite nondecreasing subsequence. In every [infinite set](../../../../../infinite-set.md) of indices there is an index with infinitely many later successors above its value. Otherwise repeatedly discard the finitely many successors of each chosen index, obtaining a [bad sequence](../../../../../bad-sequence.md). Applying this observation successively within the infinite successor [set](../../../../../set-split.md) produces the required [subsequence](../../../../../subsequence.md).

We also need the [Higman lemma](../../../../../higman-s-lemma.md), and prove it here. If finite [words](../../../../../string.md) over $Q$ admitted a [bad sequence](../../../../../bad-sequence.md), choose one $w_0,w_1,\ldots$ with each [word](../../../../../string.md) of least possible length among choices permitting a bad continuation of its fixed prefix. No [word](../../../../../string.md) is empty. Write $w_i=v_i a_i$, and extract indices $n_0<n_1<\cdots$ with $a_{n_0}\le a_{n_1}\le\cdots$. The [sequence](../../../../../sequence.md)

$$
w_0,\ldots,w_{n_0-1},v_{n_0},v_{n_1},\ldots
$$

is bad: an earlier $w_i$ embedding into some $v_{n_j}$ would embed into $w_{n_j}$, while $v_{n_i}\preceq v_{n_j}$ together with $a_{n_i}\le a_{n_j}$ would give $w_{n_i}\preceq w_{n_j}$. This contradicts the minimal length of $w_{n_0}$, since $v_{n_0}$ is shorter. Hence finite [words](../../../../../string.md) are [well-quasi-ordered](../../../../../well-quasi-ordering.md) under [subsequence](../../../../../subsequence.md) embedding with increased labels.

Now suppose labelled [rooted trees](../../../../../rooted-tree.md) admitted a [bad sequence](../../../../../bad-sequence.md) $T_0,T_1,\ldots$, chosen minimally by number of vertices at each successive position. Let $B$ consist of all immediate child subtrees of all the $T_i$, with the inherited labels. We claim $B$ is a [well-quasi-ordering](../../../../../well-quasi-ordering.md). Otherwise take a bad [sequence](../../../../../sequence.md) of members of $B$. Only finitely many distinct [rooted trees](../../../../../rooted-tree.md) occur among the children of any finite initial list of $T_i$, so, by discarding terms and selecting a [subsequence](../../../../../subsequence.md), we may arrange its members $S_0,S_1,\ldots$ to come from strictly increasing parent indices $n_0<n_1<\cdots$. Then

$$
T_0,\ldots,T_{n_0-1},S_0,S_1,\ldots
$$

is bad. A prefix [rooted tree](../../../../../rooted-tree.md) embedding into $S_j$ would embed into its parent $T_{n_j}$; embeddings between the $S_j$ are excluded by their choice. But $S_0$ has fewer vertices than $T_{n_0}$, contradicting minimality. This proves the claim.

List the child subtrees of each $T_i$ in any order. By the [Higman lemma](../../../../../higman-s-lemma.md) these child lists are [well-quasi-ordered](../../../../../well-quasi-ordering.md). Extract an infinite [subsequence](../../../../../subsequence.md) with nondecreasing root labels, and then compare two child lists on that [subsequence](../../../../../subsequence.md). Their [subsequence](../../../../../subsequence.md) embedding gives distinct target child branches into which the source child subtrees embed. Map the source root to the target root and join each embedded child root to it by the corresponding downward path. The paths are disjoint except at the root, and labels increase. Thus $T_i\preceq T_j$ for some $i<j$, contradicting badness. This proves [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md) and its labelled version. If root preservation is required, mark the root with a special label incomparable with all ordinary labels; the same proof then forces root to map to root.

For [Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md), fix $k\in\omega$ and suppose there are arbitrarily long bad lists satisfying $|T_i|\le k+i$ for $i=1,2,\ldots$. Make a [finite bad-sequence tree](../../../../../finite-bad-sequence-tree.md) whose nodes are these lists, using one representative of each finite rooted-[rooted tree](../../../../../rooted-tree.md) isomorphism type. At each position only finitely many choices satisfy the size bound, so the [rooted tree](../../../../../rooted-tree.md) is finitely branching. An infinite path exists: at every stage choose a child having extensions of arbitrarily large length, which must exist because there are finitely many children. The path is an infinite bad [sequence](../../../../../sequence.md), contradicting [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md). Therefore

$$
\boxed{\forall k\in\omega\ \exists N\ \forall (T_i)_{1\le i\le N}\quad
\bigl[(\forall i\ |T_i|\le k+i)\Rightarrow(\exists i<j\ T_i\preceq T_j)\bigr].}
$$

The identical argument works with finitely many labels and any fixed finite size bound at each position.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
