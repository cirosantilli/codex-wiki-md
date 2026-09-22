<h1 id="4h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [context-free languages](../../../../../../context-free-language.md) $L_1=\{a^n b^n c^m:n,m\geq0\}$ and $L_2=\{a^m b^n c^n:n,m\geq0\}$ have [context-free grammars](../../../../../../context-free-grammar.md) $S\to TC$, $T\to aTb\mid\varepsilon$, $C\to cC\mid\varepsilon$, and $S\to AT$, $A\to aA\mid\varepsilon$, $T\to bTc\mid\varepsilon$, respectively.

Their [intersection](../../../../../../set-intersection.md) is $L=\{a^n b^n c^n:n\geq0\}$. Suppose $L$ satisfied the [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md) with length $p$. In a decomposition $a^p b^p c^p=uvwxy$ with $|vwx|\leq p$ and $|vx|>0$, the window $vwx$ cannot meet both the $a$ and $c$ blocks. Pumping down changes at least one count and leaves at least one count unchanged. Thus the three counts are unequal, or the word order is invalid, contrary to the [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md). Hence **CFLs are not closed under [intersection](../../../../../../set-intersection.md)**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4H](../../4h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
