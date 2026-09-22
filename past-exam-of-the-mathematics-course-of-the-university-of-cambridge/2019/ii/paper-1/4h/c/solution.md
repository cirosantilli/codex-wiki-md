<h1 id="4h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take [context-free grammars](../../../../../../context-free-grammar.md) $G_L,G_M$ for $L,M$ and rename their nonterminals so that they are disjoint. If their start symbols are $S_L,S_M$, add a new start symbol $S$ and the production

$$
S\to S_LS_M.
$$

All productions remain context-free. A derivation from $S$ produces a word from $L$ followed by a word from $M$, and every such concatenation has a derivation. Thus the new grammar generates $LM$, proving [closure of context-free languages under concatenation](../../../../../../closure-of-context-free-languages-under-concatenation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4H](../../4h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
