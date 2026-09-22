<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

We prove the [Ehrenfeucht-Mostowski theorem](../../../../../ehrenfeucht-mostowski-theorem.md) by ordered products of [ultrafilters](../../../../../ultrafilter.md), without using [Ramsey's theorem](../../../../../ramsey-s-theorem.md). Choose a [Skolem expansion](../../../../../skolem-expansion.md) $M^*$ of the infinite structure and distinct elements $b_0,b_1,\ldots$. Fix a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) $U$ on $\mathbb N$.

For a finite increasing subset $F=\{i_1<\cdots<i_r\}$ of the desired index order $I$, define the ordered [Fubini product of ultrafilters](../../../../../fubini-product-of-ultrafilters.md) $U_F$ on $\mathbb N^F$ by

$$
A\in U_F\quad\Longleftrightarrow\quad
U n_{i_1}\ U n_{i_2}\ \cdots\ U n_{i_r}\ [(n_i)_{i\in F}\in A].
$$

The notation $U n\ P(n)$ means that the set of $n$ satisfying $P$ belongs to $U$; the leftmost quantifier is outermost. Upward closure and intersection follow successively at each coordinate, and applying complement at each step proves the [ultrafilter](../../../../../ultrafilter.md) dichotomy. Products are ordered; no false claim of symmetry is needed.

Put $M_F=(M^*)^{\mathbb N^F}/U_F$, with $M_\varnothing=M^*$. If $F\subseteq G$, pullback of a function by coordinate projection induces

$$
\sigma_{FG}:[f]_{U_F}\longmapsto[f\circ\operatorname{pr}_F]_{U_G}.
$$

For a cylinder condition involving only coordinates in $F$, deleting the unused [ultrafilter](../../../../../ultrafilter.md) quantifiers makes its membership in $U_G$ exactly its membership in $U_F$. The [Łoś theorem](../../../../../los-theorem.md) therefore makes $\sigma_{FG}$ an [elementary embedding](../../../../../elementary-embedding.md), not merely a homomorphism. The projection identities give $\sigma_{GH}\sigma_{FG}=\sigma_{FH}$.

Take the directed limit of this system: elements from two stages are identified if their images agree at a common larger finite stage, and formulas are evaluated at such a stage. Elementary coherence makes this well-defined. It also makes each stage elementary in the limit: a formula uses finitely many parameters, and an existential witness at a later stage can be pulled back at the level of existential truth because the transition maps are elementary. Denote the limit by $N^*$.

For each $i\in I$, let $a_i$ be the limit image of the coordinate function $n_i\mapsto b_{n_i}$. These elements are distinct. For $i<j$, after fixing $n_i$, equality $b_{n_i}=b_{n_j}$ holds for at most one $n_j$, a set not in $U$; hence equality fails in the two-coordinate [ultrapower](../../../../../ultrapower.md) and therefore in the limit.

For any increasing $i_1<\cdots<i_r$, Łoś evaluates

$$
N^*\models\varphi(a_{i_1},\ldots,a_{i_r})
\quad\Longleftrightarrow\quad
U n_1\cdots U n_r\ [M^*\models\varphi(b_{n_1},\ldots,b_{n_r})].
$$

The right-hand side depends on the formula and the number of increasing coordinates, not their particular indices. Thus $(a_i)_{i\in I}$ is order-indiscernible for every formula of the expanded language simultaneously; no preliminary homogeneous thinning is used. If elements of $M$ were named before expanding, the same computation gives indiscernibility over those names and the initial stage embeds the original structure into the limit.

The [Skolem hull](../../../../../skolem-hull.md) of these generators is elementary by the witness property. Transporting the generators by any [order automorphism](../../../../../order-automorphism.md) of $I$ transports every term, with well-definedness and relation preservation supplied by the formula equivalence just proved. The inverse transport supplies an inverse automorphism. **The ordered-ultrapower construction gives the full Ehrenfeucht–Mostowski model and its [order automorphisms](../../../../../order-automorphism.md) without [Ramsey's theorem](../../../../../ramsey-s-theorem.md).**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
