<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $S$ consist of all [universal-existential sentences](../../../../../../universal-existential-sentence.md) entailed by $T$, and take $A_0\models S$. By (c), there is an [existential embedding](../../../../../../existential-embedding.md) of $A_0$ into $B_0\models T$. By (b), $B_0$ embeds in $A_1$ with $A_0\preccurlyeq A_1$. After replacing structures by isomorphic copies, arrange these maps as inclusions. Since $A_1\equiv A_0$, it also satisfies $S$ and the construction can be repeated. This produces

$$
A_0\subseteq B_0\subseteq A_1\subseteq B_1\subseteq A_2\subseteq\cdots,
\qquad A_i\preccurlyeq A_{i+1},\quad B_i\models T.
$$

The two interleaved chains have the same union $D$. The [elementary chain theorem](../../../../../../elementary-chain-theorem.md) gives $A_0\preccurlyeq D$. The $B_i$ are an ordinary chain of models of $T$, so the assumed closure under unions of chains gives $D\models T$. Therefore $A_0\models T$. This proves

$$
\boxed{\operatorname{Mod}(T)=\operatorname{Mod}(S),\qquad S\subseteq\forall_2.}
$$

Conversely, universal-existential axioms are preserved in such unions: a finite universal tuple occurs in one stage, which already supplies its existential witnesses. The quantifier-free matrix has the same truth value in that stage and in the union. This also explains the [inductive first-order theory](../../../../../../inductive-first-order-theory.md) characterization.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
