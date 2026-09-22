<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [well-quasi-ordering](../../../../../well-quasi-ordering.md) is a reflexive transitive relation $\le_Q$ such that every infinite sequence $q_0,q_1,\ldots$ contains $i<j$ with $q_i\le_Qq_j$. Such a pair is good; a sequence without one is bad. A [better-quasi-ordering](../../../../../better-quasi-ordering.md) strengthens this condition from sequences to barrier arrays. A [barrier in better-quasi-order theory](../../../../../barrier-in-better-quasi-order-theory.md) on an infinite $A\subseteq\mathbb N$ is a family $B$ of nonempty finite increasing sequences whose underlying [sets](../../../../../set-split.md) are inclusion-incomparable, such that every infinite subset of $A$ has an initial segment in $B$. Write $s\triangleleft t$ if both are initial segments of some increasing sequence $u$ and its first-term deletion, respectively. BQO means that every $f:B\to Q$ has $s\triangleleft t$ with $f(s)\le_Q f(t)$. Singleton barriers give the WQO condition, so BQO implies WQO. These are the barrier-array conventions explained in [the treatment of better-quasi-orders](https://arxiv.org/abs/1604.05866).

The [labelled version of Kruskal's tree theorem](../../../../../labelled-version-of-kruskal-s-tree-theorem.md) states that finite [rooted trees](../../../../../rooted-tree.md) labelled by a WQO $Q$ are WQO under [label-monotone tree embedding](../../../../../label-monotone-tree-embedding.md). An embedding is an injective vertex map preserving lowest common ancestors and increasing labels. In particular an edge may map to a nonempty path, and the source root may map below the target root. The unlabelled theorem follows by taking one label. We prove the stronger labelled assertion.

We first supply the word lemma needed in the proof. Every sequence in a WQO has an infinite nondecreasing subsequence: color pairs $i<j$ according to whether $q_i\le q_j$ and use Ramsey's theorem; the all-bad homogeneous possibility is excluded by WQO. Suppose finite words over $Q$ had a [bad sequence](../../../../../bad-sequence.md). Choose a [minimal bad sequence](../../../../../minimal-bad-sequence.md) $w_n$, minimizing length at each stage among choices admitting a bad continuation. No word is empty. Write $w_n=v_n a_n$ and choose $n_0<n_1<\cdots$ with $a_{n_r}\le a_{n_s}$ for $r<s$. The sequence

$$
w_0,\ldots,w_{n_0-1},v_{n_0},v_{n_1},v_{n_2},\ldots
$$

cannot be bad by minimality, since its new word at position $n_0$ is shorter. A good pair within the old prefix was already forbidden. A prefix word embedding in some $v_{n_r}$ embeds in $w_{n_r}$, also forbidden. A good pair $v_{n_r}\le v_{n_s}$ extends by the ordered last letters to $w_{n_r}\le w_{n_s}$, again forbidden. This proves the [Higman lemma](../../../../../higman-s-lemma.md).

Assume next that labelled trees have a [bad sequence](../../../../../bad-sequence.md). Choose $T_n$ minimally by number of vertices, again among choices admitting a bad continuation. Let $\mathcal S$ be the collection of all immediate child subtrees of all $T_n$. We claim it is WQO. If $S_0,S_1,\ldots$ were a [bad sequence](../../../../../bad-sequence.md) in $\mathcal S$, attach to each $S_r$ a parent index $k_r$ with $S_r$ a proper child subtree of $T_{k_r}$. The indices must be unbounded on every tail: bounded indices provide only finitely many actual child subtrees, forcing a repeated tree and hence a good pair. Pass to a subsequence with strictly increasing parent indices $k_0<k_1<\cdots$. Then

$$
T_0,\ldots,T_{k_0-1},S_0,S_1,S_2,\ldots
$$

is bad. Indeed a prefix tree embedding into $S_r$ also embeds into its host $T_{k_r}$, contrary to the original [bad sequence](../../../../../bad-sequence.md), and the other possible good pairs were excluded already. But $S_0$ is smaller than $T_{k_0}$, contradicting minimality. This proves the claim.

Enumerate each tree's child subtrees in any chosen order. Higman's lemma makes the resulting finite words over $\mathcal S$ WQO. Products of two WQOs are WQO: choose a nondecreasing subsequence in the first coordinate and then a good pair in the second. Apply this to each root label and child word. Some $i<j$ has an increasing root label and an embedding of its child word into the other's child word. Map the first root to the second root and use the child-subtree embeddings in the matched distinct branches. Their images lie below distinct children, so their pairwise meets are the second root; within each branch the chosen embeddings preserve meets. This gives an embedding $T_i\preceq_QT_j$, contradicting badness. Hence **Kruskal's theorem holds**. If one requires roots to be preserved, label the root with a new label incomparable with all ordinary labels and apply the just-proved labelled version; its unique occurrence forces root preservation.

For [Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md), fix $k$. Consider bad finite sequences of unlabelled tree isomorphism types satisfying $|T_i|\le k+i$, with indices starting at one. Put them in a tree ordered by extension. At each position there are only finitely many isomorphism types with the allowed vertex bound, so this tree is finitely branching. If [bad sequences](../../../../../bad-sequence.md) had arbitrarily large lengths, the [König infinity lemma](../../../../../konig-s-lemma.md) would give an infinite branch, an infinite [bad sequence](../../../../../bad-sequence.md) contradicting Kruskal's theorem. Consequently

$$
\boxed{\forall k\ \exists N\ \forall(T_1,\ldots,T_N)\;
\bigl[\,|T_i|\le k+i\ \Longrightarrow\ \exists i<j\ T_i\preceq T_j\,\bigr].}
$$

The bound is uniform over all such sequences. Quotienting by tree isomorphism types is essential to the finite-branching argument; arbitrary vertex names would give infinitely many codes for the same finite tree. A fixed finite label alphabet can be included with the same argument.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
