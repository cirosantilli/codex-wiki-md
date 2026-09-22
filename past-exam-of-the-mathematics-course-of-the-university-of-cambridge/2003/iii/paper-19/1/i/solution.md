<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For finite [rooted trees](../../../../../../rooted-tree.md), use [rooted-tree homeomorphic embedding](../../../../../../homeomorphic-embedding-of-a-rooted-tree.md): an [injective](../../../../../../injective-function.md) vertex map preserves ancestors and [lowest common ancestors](../../../../../../lowest-common-ancestor.md), so edges may become paths and distinct branches remain distinct. The root can map to a vertex below the host root. More generally label vertices in a [well-quasi-ordering](../../../../../../well-quasi-ordering.md) $Q$ and require each source label to precede its image label. We prove this stronger [labelled version of Kruskal's tree theorem](../../../../../../labelled-version-of-kruskal-s-tree-theorem.md), from which the unlabelled result follows by taking one label.

We first need the finite-word closure, and prove it rather than merely invoking [Higman lemma](../../../../../../higman-s-lemma.md). If finite [words](../../../../../../string.md) over $Q$ were not a [well-quasi-ordering](../../../../../../well-quasi-ordering.md) under order-preserving [subsequence](../../../../../../subsequence.md) embedding with increased labels, choose a [minimal bad sequence](../../../../../../minimal-bad-sequence.md) $w_0,w_1,\ldots$, minimizing the length of $w_n$ among [words](../../../../../../string.md) admitting a bad continuation of the already chosen prefix. No $w_n$ is empty. Write $w_n=v_na_n$ by removing its last letter. The [perfect subsequence lemma](../../../../../../perfect-subsequence-lemma.md) gives $n_0<n_1<\cdots$ with $a_{n_r}\le a_{n_s}$ for $r<s$.

The [sequence](../../../../../../sequence.md) $w_0,\ldots,w_{n_0-1},v_{n_0},v_{n_1},\ldots$ is still bad. An earlier $w_i$ embedding into a later $v_{n_r}$ would embed into $w_{n_r}$, contradicting the original [sequence](../../../../../../sequence.md). An embedding of $v_{n_r}$ into $v_{n_s}$ extends by the last-letter comparison to an embedding of $w_{n_r}$ into $w_{n_s}$. Both possibilities are excluded. This contradicts minimality at position $n_0$, since $v_{n_0}$ is shorter. Thus the finite-word closure holds. The [perfect subsequence lemma](../../../../../../perfect-subsequence-lemma.md) also proves finite product closure: first pass to a nondecreasing [subsequence](../../../../../../subsequence.md) in one coordinate, then in the next, preserving all previous comparisons.

Suppose now that the labelled trees admit a [bad sequence](../../../../../../bad-sequence.md) $T_0,T_1,\ldots$. Choose a [minimal bad sequence](../../../../../../minimal-bad-sequence.md) by vertex number. Let $\mathcal U$ be all the proper descendant-rooted subtrees of these trees. We claim that $\mathcal U$ is a [well-quasi-ordering](../../../../../../well-quasi-ordering.md). If it had a [bad sequence](../../../../../../bad-sequence.md) of subtrees $U_r$, its parent indices can be made strictly increasing, say $U_r$ comes from $T_{n_r}$. Indeed each finite initial collection of parent trees has only finitely many subtrees, and a [bad sequence](../../../../../../bad-sequence.md) cannot contain infinitely many terms from a finite collection. Passing to a [subsequence](../../../../../../subsequence.md) therefore makes $n_0<n_1<\cdots$.

Then $T_0,\ldots,T_{n_0-1},U_0,U_1,\ldots$ is bad. A prefix tree embedding into $U_r$ would embed into its parent $T_{n_r}$, contrary to the original badness, and the tail is bad by construction. But $U_0$ has fewer vertices than $T_{n_0}$, contradicting minimality. This proves the claim.

Give the children of each root any fixed order. Its forest of child subtrees is a finite [word](../../../../../../string.md) in $\mathcal U$. The [word](../../../../../../string.md) theorem and finite product closure show that the pairs consisting of the root label and the child-subtree [word](../../../../../../string.md) are a [well-quasi-ordering](../../../../../../well-quasi-ordering.md). Thus some $i<j$ have comparable root labels and an embedding of the child [word](../../../../../../string.md) of $T_i$ into that of $T_j$. Map the source root to the target root and use the obtained embeddings inside distinct target child subtrees. The paths from the target root into those distinct branches are disjoint except at the root, so this is a [label-monotone tree embedding](../../../../../../label-monotone-tree-embedding.md). It contradicts badness. Hence

$$
\boxed{\text{finite rooted trees labelled in a WQO are a WQO under homeomorphic embedding.}}
$$

For [Friedman's finite form of Kruskal's theorem](../../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md), fix $k\in\mathbb N$. **There is $N(k)$ such that any $N(k)$ trees with $|T_i|\le k+i$ contain $i<j$ with $T_i\preceq T_j$.** Use indices starting at zero; shifting them only changes $k$. To prove this uniform finite bound, form the [finite bad-sequence tree](../../../../../../finite-bad-sequence-tree.md) of finite bad prefixes obeying the size bounds. At position $i$ there are only finitely many rooted-tree [isomorphism](../../../../../../isomorphism.md) types with at most $k+i$ vertices, so every node has finitely many successors.

If no bound existed, this tree would have nodes of arbitrarily large depth. A node with arbitrarily long extensions has a child with arbitrarily long extensions, since it has only finitely many children. Choosing such a child repeatedly produces an infinite branch, as in the [König infinity lemma](../../../../../../konig-s-lemma.md). The branch is an infinite bad tree [sequence](../../../../../../sequence.md), contradicting the theorem just proved. Therefore the required $N(k)$ exists. The same proof works with any fixed finite label alphabet and any specified size bound finite at each position.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
