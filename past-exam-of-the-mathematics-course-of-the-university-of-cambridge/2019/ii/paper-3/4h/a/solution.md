<h1 id="4h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [context-free grammar](../../../../../../context-free-grammar.md) is in [Chomsky normal form](../../../../../../chomsky-normal-form.md) when every production is of one of the forms

$$
A\to BC,
\qquad A\to a,
$$

where $A,B,C$ are [nonterminal symbols](../../../../../../nonterminal-symbol.md) and $a$ is a [terminal symbol](../../../../../../terminal-symbol.md). Under this strict convention there is no [epsilon production](../../../../../../epsilon-production.md), so such a grammar cannot generate the [empty word](../../../../../../empty-word.md). Conversion of an arbitrary grammar therefore gives

$$
\boxed{\mathcal L(G_{\rm Chom})=\mathcal L(G)\setminus\{\epsilon\}.}
$$

If $\epsilon\notin\mathcal L(G)$, the two languages are equal. An alternative extended convention permits the exceptional start production $S_0\to\epsilon$; under that convention conversion preserves the whole language.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4H](../../4h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
