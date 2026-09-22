<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We prove the [labelled version of Kruskal's tree theorem](../../../../../labelled-version-of-kruskal-s-tree-theorem.md), with labels in a [well-quasi-ordering](../../../../../well-quasi-ordering.md) $Q$; the unlabelled result is its one-label case. A [label-monotone tree embedding](../../../../../label-monotone-tree-embedding.md) is an injective map of finite [rooted trees](../../../../../rooted-tree.md) preserving [lowest common ancestors](../../../../../lowest-common-ancestor.md) and increasing labels. Its root may map below the host root, and an edge may map to a path. These conventions distinguish [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md) from the stricter adjacency-preserving relation, which is not well-quasi-ordered.

We will use two elementary consequences of [well-quasi-ordering](../../../../../well-quasi-ordering.md). Every infinite sequence in a [well-quasi-ordering](../../../../../well-quasi-ordering.md) has an infinite nondecreasing subsequence: color pairs by whether the earlier element precedes the later one, apply [Ramsey's theorem](../../../../../ramsey-s-theorem.md), and exclude an all-bad infinite set. Restricting successively in each coordinate proves [finite product closure of well-quasi-orderings](../../../../../finite-product-closure-of-well-quasi-orderings.md).

For completeness, here is the required proof of [Higman's lemma](../../../../../higman-s-lemma.md). If finite [words](../../../../../string.md) over $Q$ admitted a [bad sequence](../../../../../bad-sequence.md), choose one $w_0,w_1,\ldots$ whose next word always has the least length admitting a bad continuation of the fixed prefix. No word is empty. Write $w_i=v_i a_i$, separating the last letter. The set of prefixes $\{v_i\}$ is a [well-quasi-ordering](../../../../../well-quasi-ordering.md). Otherwise select a bad sequence of these prefixes with strictly increasing owner indices $n_0<n_1<\cdots$; this is possible because every finite initial set of owners supplies only finitely many prefixes, and a bad sequence cannot repeat a word. Then

$$
w_0,\ldots,w_{n_0-1},v_{n_0},v_{n_1},\ldots
$$

is bad. An earlier original word embedding into $v_{n_j}$ would also embed into $w_{n_j}$, contradicting the original badness; comparisons inside the new tail are excluded by its choice. But $v_{n_0}$ is shorter than $w_{n_0}$, contradicting minimality. Since the prefixes and the last letters are [well-quasi-ordered](../../../../../well-quasi-ordering.md), their product gives $i<j$ with $v_i$ embedding into $v_j$ and $a_i\le_Q a_j$. Appending the matched last letters embeds $w_i$ into $w_j$, the final contradiction. Thus **finite words over a WQO are WQO**.

Now suppose labelled finite [rooted trees](../../../../../rooted-tree.md) admit a [bad sequence](../../../../../bad-sequence.md) $T_0,T_1,\ldots$. Choose it minimally in vertex count at each successive position. Let $\mathcal S$ be all immediate child subtrees of its members. This is a [well-quasi-ordering](../../../../../well-quasi-ordering.md): if not, select a bad sequence $S_0,S_1,\ldots$ of child subtrees with increasing owner indices $n_j$, and splice it after $T_0,\ldots,T_{n_0-1}$. Every child subtree embeds into its owner, so a comparison from the prefix to the tail would contradict original badness. The splice is bad and its first replacement is strictly smaller, contradicting the [minimal bad sequence](../../../../../minimal-bad-sequence.md) choice.

For each $T_i$, list its child subtrees in any order as a finite [word](../../../../../string.md) $c_i$ over $\mathcal S$ and record its root label $q_i$. The product $Q\times\mathcal S^*$ is a [well-quasi-ordering](../../../../../well-quasi-ordering.md) by [Higman's lemma](../../../../../higman-s-lemma.md). Hence some $i<j$ has $q_i\le_Q q_j$ and a subsequence embedding of $c_i$ into $c_j$. Match the roots and use the chosen subtree embeddings in distinct target branches. Their union preserves [lowest common ancestors](../../../../../lowest-common-ancestor.md) and labels, and stretches only edge paths. Thus $T_i$ embeds into $T_j$, a contradiction. We have proved

$$
\boxed{\text{Finite rooted trees labelled in a WQO are WQO under label-monotone homeomorphic embedding.}}
$$

To deduce [Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md), fix $k\in\mathbb N$. At position $i=0,1,\ldots$ permit unlabelled trees of at most $k+i$ vertices. Up to [isomorphism](../../../../../isomorphism.md) only finitely many trees are possible at each position. Form the [finite bad-sequence tree](../../../../../finite-bad-sequence-tree.md) whose nodes are finite bad sequences satisfying these bounds, ordered by extension. It is finitely branching. If there were arbitrarily long admissible bad sequences, [König infinity lemma](../../../../../konig-s-lemma.md) would give an infinite branch, contradicting [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md). Therefore

$$
\boxed{\forall k\ \exists N\ \forall(T_0,\ldots,T_{N-1})\ \left[\forall i<N\ (|T_i|\le k+i)\ \Longrightarrow\ \exists i<j<N\ (T_i\preceq T_j)\right].}
$$

One can instead use a fixed finite set of labels, giving a correspondingly parameterized finite statement by exactly the same proof. The crucial feature is a uniform bound $N$ for each initial size allowance, not merely termination of one chosen sequence.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
