<h1 id="4g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a [context-free grammar](../../../../../../context-free-grammar.md) for $L$ with start symbol $S$, rename nonterminals if necessary, and add a fresh start symbol $S_0$ with

$$
S_0\to\epsilon\mid SS_0.
$$

Every derivation concatenates finitely many words of $L$, and every finite concatenation can be derived. **The resulting grammar generates $L^*$**, proving [closure of context-free languages under Kleene star](../../../../../../closure-of-context-free-languages-under-kleene-star.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4G](../../4g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
