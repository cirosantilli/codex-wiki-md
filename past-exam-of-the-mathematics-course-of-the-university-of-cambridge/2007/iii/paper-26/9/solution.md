<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Use [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md): an injective map of vertices preserves ancestor order and lowest common ancestors, so edges may be stretched into paths and distinct branches remain distinct. The source root may map below the target root. [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md) asserts that finite rooted trees are [well-quasi-ordered](../../../../../well-quasi-ordering.md) by this embedding: every infinite sequence $T_0,T_1,\ldots$ has $i<j$ with $T_i\preceq T_j$. More generally, labels from any [well-quasi-ordering](../../../../../well-quasi-ordering.md) may be required to increase under the embedding. This labelled result implies the unlabelled one by using a one-point label set, and also implies the version for unrooted trees by choosing roots arbitrarily.

We first prove the word lemma needed for the tree argument. In a [well-quasi-ordering](../../../../../well-quasi-ordering.md) $Q$, every infinite sequence has an infinite nondecreasing subsequence. Indeed, some term must be below infinitely many later terms: if no term were, recursively avoiding the finitely many successors dominated by each previously chosen term would produce a [bad sequence](../../../../../bad-sequence.md). Repeat this observation inside the infinite set of later terms dominating the chosen one.

The [Higman lemma](../../../../../higman-s-lemma.md) says that finite words over $Q$ are well-quasi-ordered by subsequence embedding with letterwise comparison. Suppose otherwise, and choose a [minimal bad sequence](../../../../../minimal-bad-sequence.md) of words, minimizing length at each position among words admitting a bad continuation of the chosen prefix. No word is empty. Write $w_i=v_i a_i$, separating its last letter. Choose indices $i_0<i_1<\cdots$ on which $a_{i_j}$ is nondecreasing. Then

$$
w_0,\ldots,w_{i_0-1},v_{i_0},v_{i_1},\ldots
$$

is bad. A comparison from a prefix word into some $v_{i_j}$ would give a comparison into $w_{i_j}$ in the old bad sequence. A comparison $v_{i_j}\preceq v_{i_k}$, $j<k$, together with $a_{i_j}\leq a_{i_k}$ would give $w_{i_j}\preceq w_{i_k}$. Both are impossible. But the new continuation uses a shorter word at position $i_0$, contradicting minimality. This proves the [Higman lemma](../../../../../higman-s-lemma.md).

Now suppose there were a bad sequence of labelled finite rooted trees. Choose it minimally by number of vertices at each position. Let $\mathcal P$ be the collection of all proper rooted subtrees occurring at vertices other than the roots in these trees. We claim that $\mathcal P$ is well-quasi-ordered. Otherwise take a bad sequence of such subtrees $S_j$, with $S_j$ a proper subtree of $T_{i_j}$. The indices cannot remain bounded, because finitely many finite trees have only finitely many rooted subtrees, and repetition is a comparison. Pass to a subsequence with strictly increasing $i_j$. The sequence

$$
T_0,\ldots,T_{i_0-1},S_0,S_1,\ldots
$$

is bad: a comparison from an earlier $T_h$ into $S_j$ would compose with the subtree embedding $S_j\preceq T_{i_j}$ to contradict the original badness. Its other comparisons were excluded already. Since $S_0$ has fewer vertices than $T_{i_0}$, this contradicts minimality, proving the claim.

List each tree's immediate root subtrees in any chosen order. These are finite words over $\mathcal P$, hence form a [well-quasi-ordering](../../../../../well-quasi-ordering.md) by the word lemma. Combine the lists with the root labels. A product of two well-quasi-orders is well-quasi-ordered: pass to an infinite nondecreasing subsequence in the first coordinate and find a comparable pair in the second. Thus two trees have comparable root labels and a subsequence matching of their child lists. Map the first root to the second root and use the matched subtree embeddings in distinct child branches. The resulting injective map preserves labels and lowest common ancestors, giving $T_i\preceq T_j$, the desired contradiction. This proves the full labelled form of [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md).

[Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md) is a uniform finite consequence. For every fixed natural $k$, there is $N$ such that any sequence of $N$ finite rooted trees satisfying $|T_i|\leq k+i$ has a comparable pair $i<j$. It also holds with labels in any fixed finite label set. To prove it, assume no such $N$ exists. Form the [finite bad-sequence tree](../../../../../finite-bad-sequence-tree.md) whose nodes are bad finite tree sequences satisfying those size bounds, using one representative of each isomorphism type. Each position has finitely many extensions, since there are finitely many labelled tree types of each bounded size. By assumption this finitely branching tree has nodes at every finite height. The [König infinity lemma](../../../../../konig-s-lemma.md) supplies an infinite branch, which is an infinite bad sequence of trees, contradicting the theorem just proved. Hence

$$
\boxed{\forall k\ \exists N\ \forall(T_i)_{i<N}\ \bigl((\forall i<N\ |T_i|\leq k+i)\Longrightarrow\exists i<j<N\ T_i\preceq T_j\bigr).}
$$

Likewise, using $k$ fixed labels with the bound $|T_i|\leq i$ for $i=1,2,\ldots$ gives the customary finite labelled tree form. Only existence of its finite bound is claimed here, not a small numerical estimate.

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
