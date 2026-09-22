<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the finite relational vocabulary hypothesis of the [Ehrenfeucht-Fraïssé theorem](../../../../../../ehrenfeucht-fraisse-theorem.md), **II wins the timed game exactly when the structures are [elementarily equivalent](../../../../../../elementary-equivalence.md).** If II wins, then for every choice of $n$ by I, its strategy restricts to a winning strategy in $G_n$. Hence the models agree on every sentence of [quantifier rank](../../../../../../quantifier-rank.md) at most $n$. Every [first-order sentence](../../../../../../first-order-sentence.md) has finite [quantifier rank](../../../../../../quantifier-rank.md), so they agree on all sentences.

Conversely, [elementary equivalence](../../../../../../elementary-equivalence.md) gives $\mathcal M\equiv_n\mathcal N$ for every $n$. Choose a winning strategy for each $G_n$, and use that strategy once I announces $n$. Unlike the infinite game, the timed game permits the strategy to depend on the announced horizon.

The PDF does not explicitly impose finite vocabulary. If an arbitrary language and the full [partial isomorphism of structures](../../../../../../partial-embedding.md) winning condition are intended, the reverse assertion is false. Here is a [failure of finite-round game equivalence in infinite languages](../../../../../../failure-of-finite-round-game-equivalence-in-infinite-languages.md). Let $L=\{P_i:i\in\mathbb N\}$ be unary relational. Let

$$
M=\{(s,k):s\subseteq\mathbb N\text{ finite},\ k\in\mathbb N\},\qquad
P_i(s,k)\iff i\in s,
$$

and obtain $N$ by adjoining one point $b$ satisfying every $P_i$.

For any finite sublanguage, every Boolean cell of predicates has infinitely many elements in both structures. Every finite [partial isomorphism of structures](../../../../../../partial-embedding.md) of these reducts can therefore be extended in either direction. Induction on formulas, or a [back-and-forth method](../../../../../../back-and-forth-method.md), shows their reducts are [elementarily equivalent](../../../../../../elementary-equivalence.md). Since every sentence uses finitely many symbols, $M\equiv N$ in the whole language.

Nevertheless I wins $G_1(M,N)$ by choosing $b$: every point of $M$ fails some $P_i$, so no response preserves all atomic formulas. Thus **the printed unrestricted equivalence requires the finite-vocabulary convention**, or a game which additionally restricts each play to a finite vocabulary fragment.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
