<h1 id="4h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K\subseteq\mathbb N$ be the undecidable set denoted $\mathbb K$ in the question. The language satisfies the [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md) with pumping length one. For any nonempty $s\in L$, write $s=xyz$ with $x=\varepsilon$, $y$ its first symbol, and $z$ the remaining suffix.

If $s\in b^*$, then $xy^iz\in b^*$ for every $i\geq0$. Otherwise $s=wab^n$ for some $n\in K$. If the chosen first symbol lies in $w$, pumping it preserves the same final suffix $ab^n$. If $w=\varepsilon$, then $s=ab^n$: pumping down gives $b^n\in b^*$, while every positive pump gives $a^ib^n$ and all but its last $a$ can be absorbed into $w$. Thus every sufficiently long word has a valid pumping decomposition.

Nevertheless, if $L$ were [regular language](../../../../../../regular-language.md), closure under intersection would make

$$
L\cap ab^*=\{ab^n:n\in K\}
$$

regular. A finite automaton deciding this unary language would decide whether $n\in K$ by running it on $ab^n$, contradicting the [halting problem](../../../../../../halting-problem.md). Therefore

$$
\boxed{L\text{ satisfies the pumping lemma but is not regular}.}
$$

This is a [nonregular language satisfying the pumping lemma](../../../../../../nonregular-language-satisfying-the-pumping-lemma.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4H](../../4h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
