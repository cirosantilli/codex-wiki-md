<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Let $M^*$ be a full [Skolem expansion](../../../../../skolem-expansion.md) of an infinite structure $M$, choose distinct $b_n\in M$ for $n\in\mathbb N$, and extend the [cofinite filter](../../../../../cofinite-filter.md) to a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) $U$ on $\mathbb N$. For a finite subset $F=\{i_1<\cdots<i_r\}$ of the desired index order $I$, define the ordered [Fubini product of ultrafilters](../../../../../fubini-product-of-ultrafilters.md) $U_F$ on $\mathbb N^F$ by

$$
X\in U_F\quad\Longleftrightarrow\quad U n_{i_1}\,U n_{i_2}\cdots U n_{i_r}\,[\mathbf n\in X],
$$

where $U n\,P(n)$ means $\{n:P(n)\}\in U$. These nested tests decide complements and preserve intersections by induction on $r$, so $U_F$ is indeed an [ultrafilter](../../../../../ultrafilter.md). For the empty set use the one-point index set and its principal [ultrafilter](../../../../../ultrafilter.md).

Put $M_F=(M^*)^{\mathbb N^F}/U_F$. If $F\subseteq G$, projection of coordinates induces

$$
e_{FG}([h])=[h\circ\operatorname{pr}_{GF}].
$$

A truth test independent of a coordinate is unchanged by its dummy [ultrafilter](../../../../../ultrafilter.md) quantifier. Consequently pullback preserves exactly the $U_F$-large subsets, proving that the map is well defined and injective. The [Łoś theorem](../../../../../los-theorem.md), applied to every formula rather than just to equality, proves that it is an [elementary embedding](../../../../../elementary-embedding.md). Projections compose, so these elementary maps form a coherent directed system.

Take its [directed limit of elementary embeddings](../../../../../directed-limit-of-elementary-embeddings.md) $N^*$. Explicitly identify two stage elements when their images agree at a common larger stage, and interpret functions and relations there. For an existential formula true in the limit, its parameters and a witness occur at a common stage; elementarity then pulls truth back to the stage of the original parameters. This verifies that all stage maps into the limit are elementary.

Let $a_i$ be the image in this limit of the coordinate class $[n\mapsto b_n]\in M_{\{i\}}$. These elements are distinct: in $U_{\{i,j\}}$, equality would require $n_i=n_j$, whose inner-coordinate section is a singleton and hence not in the nonprincipal $U$. For $i_1<\cdots<i_r$, the truth of any expanded-language formula on $(a_{i_1},\ldots,a_{i_r})$ is exactly

$$
U n_1\cdots U n_r\,[M^*\models\phi(b_{n_1},\ldots,b_{n_r})].
$$

This expression depends on the formula and the tuple length, not on the chosen increasing indices. Thus $(a_i)_{i\in I}$ is an [order-indiscernible sequence](../../../../../order-indiscernible-sequence.md). The empty-coordinate stage embeds $M^*$ elementarily into $N^*$.

Their [Skolem hull](../../../../../skolem-hull.md) is elementary by the witness-function argument, and an order automorphism of $I$ extends to it by transporting the generators in every term. Equality and relation preservation follow from the displayed uniform truth test, and the inverse order automorphism gives the inverse map. Therefore **this proves the [Ehrenfeucht-Mostowski theorem](../../../../../ehrenfeucht-mostowski-theorem.md) through [ultrapowers](../../../../../ultrapower.md) and their directed limit**, with no Ramsey-theoretic step.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
