<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We use [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md): an injective [vertex](../../../../../vertex-graph-theory.md) map preserves ancestors and lowest common ancestors, while an [edge](../../../../../edge-of-a-graph.md) may map to a longer path. The root may map below the host root. Write $T\preceq U$ for this relation. The assertion of [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md) is that finite [rooted trees](../../../../../rooted-tree.md) form a [well-quasi-ordering](../../../../../well-quasi-ordering.md): every infinite [sequence](../../../../../sequence.md) has $i<j$ with $T_i\preceq T_j$.

We first supply the [word](../../../../../string.md) lemma needed in the proof. In a [well-quasi-order](../../../../../well-quasi-ordering.md) $Q$, every [sequence](../../../../../sequence.md) has an infinite nondecreasing [subsequence](../../../../../subsequence.md). Indeed, if no term had infinitely many later terms above it, successive choices beyond the finite [sets](../../../../../set-split.md) of later dominators would give a [bad sequence](../../../../../bad-sequence.md). Some term therefore has infinitely many later dominators; repeat the argument inside that infinite [subsequence](../../../../../subsequence.md), which is still well-quasi-ordered, to build a chain.

Now order finite [words](../../../../../string.md) over $Q$ by [subsequence](../../../../../subsequence.md) embedding with coordinatewise increase. Suppose a bad [word](../../../../../string.md) [sequence](../../../../../sequence.md) exists and choose one $w_0,w_1,\ldots$ minimally: at each position use a [word](../../../../../string.md) of least length allowing a bad continuation of the fixed prefix. No [word](../../../../../string.md) is empty. Write $w_i=v_i a_i$, removing its last letter. Choose indices $i_0<i_1<\cdots$ with $a_{i_0}\le a_{i_1}\le\cdots$. The [sequence](../../../../../sequence.md)

$$
w_0,\ldots,w_{i_0-1},v_{i_0},v_{i_1},\ldots
$$

would also be bad. An old [word](../../../../../string.md) embedding into $v_{i_j}$ embeds into $w_{i_j}$, contrary to the original badness; and $v_{i_j}\preceq v_{i_l}$ would extend, using the last-letter comparison, to $w_{i_j}\preceq w_{i_l}$. But $v_{i_0}$ is shorter than $w_{i_0}$, contradicting minimality. This proves [Higman lemma](../../../../../higman-s-lemma.md), including its empty-word case.

Suppose next that there is a [bad sequence](../../../../../bad-sequence.md) of finite [rooted trees](../../../../../rooted-tree.md), and choose a [minimal bad sequence](../../../../../minimal-bad-sequence.md) $T_0,T_1,\ldots$ by [vertex](../../../../../vertex-graph-theory.md) count. Let $\mathcal S$ consist of all proper rooted subtrees hanging below [vertices](../../../../../vertex-graph-theory.md) of the $T_i$. This collection is well-quasi-ordered. Otherwise choose a [bad sequence](../../../../../bad-sequence.md) $S_0,S_1,\ldots$ in $\mathcal S$. Its containing-tree indices can be selected strictly increasing, say $S_j$ is a proper subtree of $T_{i_j}$: a finite initial collection of containing [trees](../../../../../tree-graph-theory.md) has only finitely many proper subtrees, and a [bad sequence](../../../../../bad-sequence.md) cannot repeat an [isomorphism](../../../../../isomorphism.md) class. Then

$$
T_0,\ldots,T_{i_0-1},S_0,S_1,\ldots
$$

is bad. No earlier $T_l$ can embed into $S_j$, because $S_j\preceq T_{i_j}$ and this would contradict the original [sequence](../../../../../sequence.md). The new tail is bad by construction. Since $|S_0|<|T_{i_0}|$, this contradicts minimality.

List each [tree](../../../../../tree-graph-theory.md)'s immediate root subtrees in any chosen order. These are finite [words](../../../../../string.md) in the [well-quasi-order](../../../../../well-quasi-ordering.md) $\mathcal S$, so the [word](../../../../../string.md) lemma gives $i<j$ for which the child [word](../../../../../string.md) of $T_i$ embeds into that of $T_j$. Send the root of $T_i$ to the root of $T_j$, and use the chosen embeddings inside the selected, distinct target branches. The connecting paths from the target root to the images of the source children have disjoint interiors; lowest common ancestors in different branches are preserved. This constructs $T_i\preceq T_j$, the final contradiction. Thus **finite [rooted trees](../../../../../rooted-tree.md) are well-quasi-ordered by homeomorphic embedding**. If labels lie in an arbitrary [well-quasi-order](../../../../../well-quasi-ordering.md), the same proof uses label-monotone embeddings; compare root labels and child [words](../../../../../string.md) in their product [well-quasi-order](../../../../../well-quasi-ordering.md). The product property follows by taking a nondecreasing [subsequence](../../../../../subsequence.md) in the first coordinate and a good pair in the second.

For [Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md), fix $k$. Consider all finite bad prefixes $(T_1,\ldots,T_l)$ satisfying $|T_i|\le k+i$, up to rooted-tree [isomorphism](../../../../../isomorphism.md). They form a prefix [tree](../../../../../tree-graph-theory.md). At each node there are finitely many possible next [trees](../../../../../tree-graph-theory.md), because there are only finitely many rooted-tree [isomorphism](../../../../../isomorphism.md) types on at most $k+l+1$ [vertices](../../../../../vertex-graph-theory.md). If prefixes of arbitrary length existed, the [König infinity lemma](../../../../../konig-s-lemma.md) would give an infinite branch, hence an infinite [bad sequence](../../../../../bad-sequence.md), contrary to what we proved. Its height is therefore bounded. Consequently

$$
\boxed{\forall k\ \exists N\ \forall(T_1,\ldots,T_N),\quad |T_i|\le k+i\ \Longrightarrow\ \exists i<j\ (T_i\preceq T_j).}
$$

The same finite-prefix argument works with a fixed finite label alphabet, and more generally with any prescribed size bound $b(i)$ having only finitely many possibilities at each position. These are finite existence statements; no numerical estimate on $N$ is needed for the conclusion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
