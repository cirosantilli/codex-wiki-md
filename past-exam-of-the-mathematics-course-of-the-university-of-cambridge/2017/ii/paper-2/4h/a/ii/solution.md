<h1 id="4h/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $L=\{a^nb^nc^n:n\geq0\}$. A halting algorithm checks that a word consists of three consecutive blocks in the correct order and compares their lengths, so $L$ is a [decidable language](../../../../../../../recursive-language.md). If it were a [context-free language](../../../../../../../context-free-language.md), apply the [pumping lemma for context-free languages](../../../../../../../pumping-lemma-for-context-free-languages.md) to $a^pb^pc^p$. The segment containing both pumped pieces has length at most $p$, so it cannot meet both the $a$ and $c$ blocks. Pumping down therefore changes at least one block count but leaves another equal to $p$, or destroys the required block order. Either way the resulting word is not in $L$, a contradiction. Thus **$L$ is a [decidable language](../../../../../../../recursive-language.md) but not a [context-free language](../../../../../../../context-free-language.md)**.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4H](../../../4h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
