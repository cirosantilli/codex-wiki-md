<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [Young diagram](../../../../../young-diagram.md) $\lambda$, a [Removable node of a Young diagram](../../../../../removable-node-of-a-young-diagram.md) is a cell whose deletion leaves a [partition of an integer](../../../../../partition-of-an-integer.md) diagram; equivalently it is the last cell of row $i$ with $\lambda_i>\lambda_{i+1}$. Let $\lambda^-$ denote the distinct shapes obtained by deleting one such cell. The [restriction branching rule for a symmetric group](../../../../../restriction-branching-rule-for-a-symmetric-group.md) in [characteristic zero](../../../../../characteristic-zero.md) is

$$
\boxed{S^\lambda\downarrow_{S_{n-1}}
\cong\bigoplus_{\mu\in\lambda^-}S^\mu.}
$$

Its induction version adds one cell in each possible way. Over an arbitrary [field](../../../../../field.md), restriction instead has a [Specht filtration](../../../../../specht-filtration.md) with these successive quotients, each once; it need not split.

To prove restriction, list the removable nodes from top to bottom. By the [standard polytabloid basis](../../../../../standard-polytabloid-basis.md), a basis of $S^\lambda$ consists of $e_t$ with $t$ standard. Its entry $n$ is necessarily at a removable node. Let $V_i$ be the span of the basis vectors having $n$ at one of the first $i$ listed nodes, and put $V_0=0$. These are $S_{n-1}$-invariant. To verify this, apply a [permutation](../../../../../permutation.md) of $1,\ldots,n-1$ and straighten the resulting [polytabloid](../../../../../polytabloid.md) by column antisymmetry and [Garnir relations](../../../../../garnir-relation.md). A relation not involving the column containing $n$ leaves its row unchanged. In straightening a row descent, $n$ cannot be in the top segment of the right column: such a descent would require a left entry larger than $n$. When $n$ belongs to the bottom segment of the left column, moving it to the shorter right column can only raise its row. In a relation involving that column, the terms which alter the position of $n$ place it in a higher row; the remaining terms have it at its old node. Thus straightening never moves it past the current top-to-bottom cutoff.

On $V_i/V_{i-1}$ send the class of $e_t$, with $n$ at the $i$th node, to the [polytabloid](../../../../../polytabloid.md) obtained by deleting that node. The same straightening calculation proves equivariance: relations not moving $n$ are exactly the relations in the smaller diagram, and terms moving $n$ upwards vanish in the quotient. Deletion bijects the standard basis of this quotient with the [standard Young tableaux](../../../../../standard-young-tableau.md) of the smaller shape. It is consequently an isomorphism, proving the asserted filtration over every [field](../../../../../field.md). In [characteristic zero](../../../../../characteristic-zero.md), [Maschke's theorem](../../../../../maschke-s-theorem.md) splits the filtration and gives the direct sum. Finally [Frobenius reciprocity](../../../../../frobenius-reciprocity.md) gives the induction rule, since a constituent $S^\nu$ has multiplicity one exactly when $\lambda\in\nu^-$.

The [hook-length formula](../../../../../hook-length-formula.md) states

$$
\boxed{f^\lambda=\dim S^\lambda=\frac{n!}{\prod_{(i,j)\in\lambda}h_{ij}},
\qquad h_{ij}=\lambda_i-j+\lambda'_j-i+1.}
$$

The [hook of a Young diagram](../../../../../hook-of-a-young-diagram.md) consists of its cell, the cells to its right in the same row, and the cells below it in the same column. This formula concerns ordinary [irreducible](../../../../../irreducible-representation.md) [dimensions](../../../../../dimension-vector-space.md); the [standard polytabloid basis](../../../../../standard-polytabloid-basis.md) also makes the [dimension](../../../../../dimension-vector-space.md) of a modular [Specht module](../../../../../specht-module.md) the same integer.

All [transpositions](../../../../../transposition-permutation.md) are conjugate, have order two, and generate $S_n$. In a one-dimensional ordinary [representation](../../../../../group-representation.md) their common scalar is therefore either $1$ or $-1$. These choices give precisely the [trivial representation](../../../../../trivial-representation.md) $S^{(n)}$ and the [sign representation](../../../../../sign-representation.md) $S^{(1^n)}$. At $n=1$ they coincide. The standard shape $(n-1,1)$ has [dimension](../../../../../dimension-vector-space.md) $n-1$: its [standard Young tableau](../../../../../standard-young-tableau.md) is specified by choosing the bottom entry from $2,\ldots,n$. Conjugating the shape preserves the [dimension](../../../../../dimension-vector-space.md), so $(2,1^{n-2})$ has the same degree.

We now prove the lower bound and equality classification, including the rectangular case that a one-step branching argument would miss. Small degrees, computed from the displayed [hook-length formula](../../../../../hook-length-formula.md), are summarized below. An exponent in the middle column records multiplicity among [partition of an integer](../../../../../partition-of-an-integer.md) labels.

| $n$ | Complete multiset of [irreducible](../../../../../irreducible-representation.md) degrees | Least degree of a shape other than the linear and standard shapes |
| --- | --- | --- |
| $3$ | $1^{(2)},2$ | No other shape |
| $4$ | $1^{(2)},2,3^{(2)}$ | $2$ at $(2,2)$ |
| $5$ | $1^{(2)},4^{(2)},5^{(2)},6$ | $5$ |
| $6$ | $1^{(2)},5^{(4)},9^{(2)},10^{(2)},16$ | $5$ at $(3,3),(2,2,2)$ |
| $7$ | $1^{(2)},6^{(2)},14^{(4)},15^{(2)},20,21^{(2)},35^{(2)}$ | $14$ |
| $8$ | $1^{(2)},7^{(2)},14^{(2)},20^{(2)},21^{(2)},28^{(2)},35^{(2)},42,56^{(2)},64^{(2)},70^{(2)},90$ | $14$ |

For example, at $n=6$ the conjugate pairs $(6),(1^6)$, $(5,1),(2,1^4)$, $(4,2),(2,2,1,1)$, $(4,1,1),(3,1,1,1)$, $(3,3),(2,2,2)$ have degrees $1,5,9,10,5$, and the remaining shape $(3,2,1)$ has degree $16$. These checks also identify every small equality case.

Induct on $n\ge9$, assuming the lower bound for all smaller degrees. If a non-linear, nonstandard shape has at least two removable nodes, none of its predecessors is a single row or single column: adding one cell to a row or column could produce only a linear or standard shape. Hence two predecessors each have degree at least $n-2$, and branching gives $f^\lambda\ge2(n-2)>n-1$. If it has only one removable node, it is a rectangle $(a^b)$ with $a,b\ge2$. Its sole predecessor is $(a^{b-1},a-1)$, which has two removable nodes. Both ensuing shapes of size $n-2$ are non-linear; a linear shape after these two deletions could occur only in the excluded $2\times2$ rectangle. Therefore two-step branching gives $f^\lambda\ge2(n-3)>n-1$. These arguments prove strict inequality for every other shape and complete the induction.

Consequently the [least non-linear ordinary degree of a symmetric group](../../../../../least-non-linear-ordinary-degree-of-a-symmetric-group.md) is

$$
\boxed{n-1\text{ for }n\ge3,\ n\ne4;qquad 2\text{ for }n=4.}
$$

For degree $n-1$, the only labels are the two standard conjugate shapes, except that at $n=6$ there are also $(3,3)$ and $(2,2,2)$, both degree five. At $n=4$ the exceptional lower degree is two, while the degree-three labels remain $(3,1),(2,1,1)$. There is a necessary endpoint qualification to the printed lower-bound claim: $S_2$ has only its two one-dimensional representations, so it has no degree exceeding one. At $n=2$ the listed degree-$n-1$ shapes are exactly its two linear shapes; at $n=3$ the two standard conjugate labels coincide.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
