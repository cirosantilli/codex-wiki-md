<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [well-quasi-ordering](../../../../../well-quasi-ordering.md) is a preorder $\preceq$ in which every infinite sequence has $i<j$ with $x_i\preceq x_j$. A sequence without such a pair is a [bad sequence](../../../../../bad-sequence.md). We use [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md): an injective map of vertices preserving [lowest common ancestors](../../../../../lowest-common-ancestor.md), so edges may become paths and a source root may map below the host root. Labels, when present, must increase in their label preorder. This convention is important; adjacency-preserving embeddings do not give the same theorem.

We first prove the auxiliary [Higman lemma](../../../../../higman-s-lemma.md). If $Q$ is a [well-quasi-order](../../../../../well-quasi-ordering.md), its finite words are [well-quasi-ordered](../../../../../well-quasi-ordering.md) by subsequence embedding with increased letters. Suppose not, and choose a [minimal bad sequence](../../../../../minimal-bad-sequence.md) of words: at each position choose one of least length among those permitting a bad continuation of the preceding prefix. No word is empty. Write $w_i=v_i a_i$ by deleting its last letter. A [well-quasi-order](../../../../../well-quasi-ordering.md) has an infinite nondecreasing subsequence of any sequence: if no member of an infinite subsequence had infinitely many later upper bounds within it, one could recursively avoid the finitely many upper bounds of earlier choices and construct a [bad sequence](../../../../../bad-sequence.md). Choose a member with infinitely many later upper bounds, restrict to those bounds and repeat. Apply this to get $a_{i_0}\preceq a_{i_1}\preceq\cdots$.

The sequence $w_0,\ldots,w_{i_0-1},v_{i_0},v_{i_1},\ldots$ is still bad. An earlier prefix word embedding into a $v_{i_j}$ would embed into $w_{i_j}$, contrary to the original [bad sequence](../../../../../bad-sequence.md). An embedding $v_{i_j}\preceq v_{i_k}$ would extend by the comparable last letters to $w_{i_j}\preceq w_{i_k}$, equally impossible. But its next word at position $i_0$ is strictly shorter than $w_{i_0}$, contradicting minimality. This proves Higman's lemma, including the possibility that a deleted word is empty, since that would make the proposed bad continuation impossible immediately.

We now prove the [labelled version of Kruskal's tree theorem](../../../../../labelled-version-of-kruskal-s-tree-theorem.md) for labels in any [well-quasi-order](../../../../../well-quasi-ordering.md) $Q$. Assume there is a [bad sequence](../../../../../bad-sequence.md) $T_0,T_1,\ldots$, and choose one minimal in vertex count at each position, subject to bad extendibility. Let $\mathcal S$ be the collection of rooted subtrees obtained by deleting a root and taking one of its child branches, over all $T_i$.

This collection is [well-quasi-ordered](../../../../../well-quasi-ordering.md). Otherwise take a [bad sequence](../../../../../bad-sequence.md) $U_j$ from $\mathcal S$. Only finitely many of these objects can come from any bounded initial segment of the $T_i$, since that segment has only finitely many child branches and a [bad sequence](../../../../../bad-sequence.md) cannot repeat an object. Pass to a subsequence with $U_j$ a child branch of $T_{k_j}$ and $k_0<k_1<\cdots$. Then

$$
T_0,\ldots,T_{k_0-1},U_0,U_1,\ldots
$$

is bad: a prefix tree embedding into $U_j$ would embed into $T_{k_j}$, and the $U_j$ are already bad among themselves. The next object $U_0$ has fewer vertices than $T_{k_0}$, contradicting the minimal bad choice. Notice that a child branch does embed into its full tree under the stated homeomorphic convention.

List each tree's child branches in any chosen order. The preceding result and Higman's lemma make these finite lists [well-quasi-ordered](../../../../../well-quasi-ordering.md). The product of two [well-quasi-orders](../../../../../well-quasi-ordering.md) is [well-quasi-ordered](../../../../../well-quasi-ordering.md): first thin to an infinite nondecreasing subsequence in one coordinate and then find an increasing pair in the other. Therefore there are $i<j$ such that the root label of $T_i$ increases to that of $T_j$, and the child list of $T_i$ embeds as a subsequence into the child list of $T_j$, with each source branch homeomorphically embedding into its matched branch.

Map the root of $T_i$ to the root of $T_j$, and use these branch embeddings below it. Different child branches map into different host branches, so their [lowest common ancestor](../../../../../lowest-common-ancestor.md) maps to the host root. Within each branch it is preserved by the chosen embedding. Thus the whole map is injective, preserves all [lowest common ancestors](../../../../../lowest-common-ancestor.md) and respects labels, contradicting badness. **Finite [rooted trees](../../../../../rooted-tree.md) labelled by a [well-quasi-order](../../../../../well-quasi-ordering.md) are [well-quasi-ordered](../../../../../well-quasi-ordering.md) under homeomorphic embedding.** Taking one label proves [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md). If one uses a root-preserving convention, mark the root by a separate label incomparable with all ordinary labels and apply the labelled theorem; the marked root then has to map to the marked root. No adjacency-preservation assertion is being made.

For [Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md), fix $k\in\mathbb N$. The required finite conclusion is

$$
\boxed{\exists N\ \forall T_1,\ldots,T_N\quad
\bigl(|T_i|\leq k+i\ \forall i\bigr)\ \Longrightarrow\
\exists i<j\ (T_i\preceq T_j).}
$$

Assume there were arbitrarily long [bad sequences](../../../../../bad-sequence.md) satisfying these size bounds. Form the tree of their finite prefixes, using rooted-tree isomorphism classes as objects. At position $i$ only finitely many finite [rooted trees](../../../../../rooted-tree.md) have at most $k+i$ vertices, so this prefix tree is finitely branching and has nodes at arbitrarily large depths. [König infinity lemma](../../../../../konig-s-lemma.md) supplies an infinite branch: at each step some child must still have arbitrarily deep extensions, because there are only finitely many children. The branch is an infinite [bad sequence](../../../../../bad-sequence.md) of finite [rooted trees](../../../../../rooted-tree.md), contradicting Kruskal's theorem. Thus such an $N$ exists. The argument also works for any prescribed size-bound function, or any fixed finite label set, because each position then still has finitely many possible objects.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
