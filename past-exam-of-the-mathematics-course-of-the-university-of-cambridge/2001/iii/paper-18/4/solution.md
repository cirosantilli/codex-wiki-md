<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The consistency implication needs more than the fact that the finite tree statement is unprovable in [Peano arithmetic](../../../../../peano-arithmetic.md). Its mechanism is a concrete encoding of [ordinal](../../../../../ordinal.md) descent by bad finite-tree sequences, combined with the controlled-termination form of [Gentzen ordinal reduction for arithmetic](../../../../../gentzen-ordinal-reduction-for-arithmetic.md).

First define the [natural-sum ordinal rank of a finite rooted tree](../../../../../natural-sum-ordinal-rank-of-a-finite-rooted-tree.md). A leaf has rank zero, and a tree with immediate child subtrees $T_1,\ldots,T_m$ has

$$
o(T)=\omega^{o(T_1)}\mathbin\#\cdots\mathbin\#\omega^{o(T_m)},
$$

where $\#$ is [Hessenberg natural sum](../../../../../hessenberg-natural-sum.md). By induction every such rank is below [epsilon zero](../../../../../epsilon-zero.md). Conversely, if $\alpha=\sum_{j=1}^r\omega^{\alpha_j}c_j$ is in [Cantor normal form](../../../../../cantor-normal-form.md), represent it by a root with $c_j$ copies of the recursively constructed tree for $\alpha_j$. The leaf represents zero. Denote the resulting canonical tree by $\tau(\alpha)$ and its vertex count by $\|\alpha\|$.

We claim that a [rooted-tree homeomorphic embedding](../../../../../homeomorphic-embedding-of-a-rooted-tree.md) $T\preceq U$ implies $o(T)\le o(U)$. If the roots match, the source child subtrees embed into distinct target branches. By induction their ranks do not decrease; exponentiation and [Hessenberg natural sum](../../../../../hessenberg-natural-sum.md) preserve these comparisons, and additional target branches only increase the sum. If the source root maps below the host root, its entire image lies in an immediate subtree $V$ of $U$. Induction gives $o(T)\le o(V)$, while

$$
o(V)<\omega^{o(V)}\le o(U).
$$

This also holds when $o(V)=0$. Thus the claim follows by induction on the host tree. In particular,

$$
\tau(\alpha)\preceq\tau(\beta)\quad\Longrightarrow\quad\alpha\le\beta.
$$

Consequently [Friedman's finite form of Kruskal's theorem](../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md) supplies [slow well-ordering below epsilon zero](../../../../../slow-well-ordering-below-epsilon-zero.md): for each $k$, descending ordinal sequences with $\|\alpha_i\|\le k+i$ have uniformly bounded length. Otherwise their canonical trees would be arbitrarily long admissible [bad sequences](../../../../../bad-sequence.md). The notation system and its comparisons are [primitive recursive](../../../../../primitive-recursive-function.md), and there are only finitely many notations of bounded norm.

The proof-theoretic input is the following precise miniaturization lemma: for the standard effective [Cantor normal form](../../../../../cantor-normal-form.md) notation system below $\varepsilon_0$, slow well-ordering with linear norm control implies the [formal consistency statement](../../../../../formal-consistency-statement.md) for [Peano arithmetic](../../../../../peano-arithmetic.md). The Friedman–Smith controlled-termination theorem, stated in its general ordinal-analysis form in Section 2.2 of [https://formal.hknu.ac.kr/Publi/kruskalJKMS.pdf](https://formal.hknu.ac.kr/Publi/kruskalJKMS.pdf) , supplies this implication over [arithmetical comprehension theory](../../../../../arithmetical-comprehension-theory.md) $\mathrm{ACA}_0$, whose first-order part is conservative over [Peano arithmetic](../../../../../peano-arithmetic.md). This is an established proof-theoretic lemma, separate from the elementary tree-rank calculation above.

Here is why that lemma is a consistency result. [Gentzen ordinal reduction for arithmetic](../../../../../gentzen-ordinal-reduction-for-arithmetic.md) assigns an alleged arithmetic contradiction an effective ordinal below $\varepsilon_0$. Reducing cuts and induction inferences preserves the contradictory end-sequent while strictly decreasing the assigned ordinal. A terminal normal derivation of a contradiction is excluded by inspection of the rules. The miniaturization argument converts this reduction/induction analysis into finite controlled descents: a contradictory proof would yield arbitrarily long descending notation sequences with a common initial allowance and linear norm control. Slow well-ordering excludes these. The control conversion is substantive; ordinary proof reductions must not simply be asserted to have linear-size growth. Gentzen's ordinal-reduction framework is discussed in [https://math.stanford.edu/~feferman/papers/reductive.pdf](https://math.stanford.edu/~feferman/papers/reductive.pdf) .

Combining the coding with that precise termination lemma gives

$$
\boxed{\mathrm{ACA}_0\vdash(\mathrm{FFF}\Rightarrow\operatorname{Con}(\mathrm{PA})).}
$$

Thus **the finite combinatorial principle proves that no PA proof of a contradiction exists** in the specified arithmetic metatheory. If consistent [Peano arithmetic](../../../../../peano-arithmetic.md) proved FFF, it would also prove its own [formal consistency statement](../../../../../formal-consistency-statement.md): the displayed implication is arithmetical and the first-order conservativity of $\mathrm{ACA}_0$ transfers it to PA. This contradicts the [Gödel second incompleteness theorem](../../../../../godel-second-incompleteness-theorem.md). It is the consistency implication, rather than unprovability by itself, that explains the strength of the finite tree principle.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
