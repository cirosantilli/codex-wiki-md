<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md) relation: an injective map of vertices preserves [lowest common ancestors](../../../../../lowest-common-ancestor.md), so edges may become paths and the source root may map below the target root. We prove the stronger labelled statement for labels in any [well-quasi-ordering](../../../../../well-quasi-ordering.md) $Q$, with labels increasing under the embedding. Forgetting labels gives [Kruskal's tree theorem](../../../../../kruskal-s-tree-theorem.md).

First every infinite [sequence](../../../../../sequence.md) in a [well-quasi-ordering](../../../../../well-quasi-ordering.md) has an infinite nondecreasing [subsequence](../../../../../subsequence.md). Colour its index pairs according as the earlier term is or is not below the later term. [Ramsey's theorem](../../../../../ramsey-s-theorem.md) gives an infinite constant-colour [subsequence](../../../../../subsequence.md); the bad colour would contradict [well-quasi-ordering](../../../../../well-quasi-ordering.md). Applying this successively in each coordinate proves [finite product closure of well-quasi-orderings](../../../../../finite-product-closure-of-well-quasi-orderings.md).

We need [Higman lemma](../../../../../higman-s-lemma.md) with its proof. Order finite [words](../../../../../string.md) over $Q$ by [subsequence](../../../../../subsequence.md) embedding with increased letters. If there were a [bad sequence](../../../../../bad-sequence.md), choose one $w_0,w_1,\ldots$ minimally: at each position choose a shortest word admitting a bad continuation of the fixed prefix. No word is empty. Write $w_n=u_na_n$, separating the last letter, and choose $n_0<n_1<\cdots$ with $a_{n_0}\leq a_{n_1}\leq\cdots$. Consider

$$
w_0,\ldots,w_{n_0-1},u_{n_0},u_{n_1},\ldots.
$$

An earlier prefix word cannot embed in a later $u_{n_j}$, since it would then embed in $w_{n_j}$. Nor can $u_{n_i}$ embed in $u_{n_j}$: adding the comparable last letters would embed $w_{n_i}$ in $w_{n_j}$. Thus the displayed [sequence](../../../../../sequence.md) is bad, contradicting minimality at $n_0$, since $u_{n_0}$ is shorter. **Finite words over a well-quasi-order are [well-quasi-ordered](../../../../../well-quasi-ordering.md).**

Now suppose labelled [rooted trees](../../../../../rooted-tree.md) admit a bad [sequence](../../../../../sequence.md) $T_0,T_1,\ldots$, chosen minimally in vertex count at each position. Let $\mathcal A$ consist of all proper rooted subtrees of these trees, rooted at a descendant and containing all its descendants. We claim $\mathcal A$ is [well-quasi-ordered](../../../../../well-quasi-ordering.md). Otherwise take a bad [sequence](../../../../../sequence.md) $S_0,S_1,\ldots$ from $\mathcal A$. Only finitely many subtrees come from any fixed finite prefix of the $T_n$'s, and a bad [sequence](../../../../../sequence.md) cannot repeat an object. Thin it so that $S_i$ comes from $T_{m_i}$ with $m_0<m_1<\cdots$. The [sequence](../../../../../sequence.md)

$$
T_0,\ldots,T_{m_0-1},S_0,S_1,\ldots
$$

is bad: $T_j\preceq S_i$ would imply $T_j\preceq T_{m_i}$, since a rooted subtree embeds in its host; comparisons within the $S_i$'s are excluded by their [choice](../../../../../axiom-of-choice.md). But $S_0$ is strictly smaller than $T_{m_0}$, contradicting minimality. This proves the claim.

Choose an arbitrary ordering of the children of each $T_n$. Record its root label and the finite word of rooted child-subtrees:

$$
\left(\ell_n,\ (T_{n,1},\ldots,T_{n,r_n})\right)\in Q\times\mathcal A^*.
$$

By [Higman lemma](../../../../../higman-s-lemma.md) and finite product closure, two records, with indices $i<j$, are comparable. Map the root of $T_i$ to the root of $T_j$, and map its selected child-subtrees into the distinct selected branches of $T_j$. Within a branch the embeddings preserve lowest common ancestors; between different branches both lowest common ancestors are the roots. Labels increase everywhere. This gives $T_i\preceq_Q T_j$, contradicting badness. **Finite labelled [rooted trees](../../../../../rooted-tree.md) are [well-quasi-ordered](../../../../../well-quasi-ordering.md) by label-monotone homeomorphic embedding.** In particular, this proves the unlabelled theorem. A root-preserving variant follows by giving the root a special incomparable label unavailable at nonroot vertices; the general labelled theorem then forces root to root. Adjacency-preserving embeddings are a different, more restrictive relation and do not satisfy the same assertion.

For [Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md), fix $k\in\mathbb N$ and consider finite bad [sequences](../../../../../sequence.md) satisfying $|T_i|\leq k+i$, with indices starting at $1$. Their prefixes form a [finite bad-sequence tree](../../../../../finite-bad-sequence-tree.md). At each depth there are only finitely many possible unlabelled tree isomorphism types below the size bound, so this tree is finitely branching. If bad [sequences](../../../../../sequence.md) existed at every finite length, [König infinity lemma](../../../../../konig-s-lemma.md) would yield an infinite branch, hence an infinite bad [sequence](../../../../../sequence.md) of [rooted trees](../../../../../rooted-tree.md), contrary to what was just proved. Therefore

$$
\boxed{\forall k\ \exists N\ \forall(T_1,\ldots,T_N)\
\left[(\forall i\leq N)\ |T_i|\leq k+i\ \Longrightarrow\
(\exists i<j\leq N)\ T_i\preceq T_j\right].}
$$

The same proof works with any fixed finite label [set](../../../../../set-split.md). The finite size bounds are what make the bad-prefix tree finitely branching; the proof does not claim a small effective numerical bound.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
