<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Consistency of $PA^-$ makes $A$ and $B$ disjoint. Suppose a recursive set $C$ separated them, and let $R(x)$ represent its total characteristic function in $PA^-$. By the [diagonal lemma](../../../../../../diagonal-lemma.md), choose a sentence $\sigma$ satisfying

$$
PA^-\vdash\sigma\leftrightarrow\neg R(\ulcorner\sigma\urcorner).
$$

Put $n=\ulcorner\sigma\urcorner$. If $n\in C$, representability gives $PA^-\vdash R(\bar n)$ and hence $PA^-\vdash\neg\sigma$, so $n\in B$, contradicting $B\cap C=\varnothing$. If $n\notin C$, representability gives $PA^-\vdash\neg R(\bar n)$ and hence $PA^-\vdash\sigma$, so $n\in A\subseteq C$, again a contradiction. Therefore $A$ and $B$ are recursively inseparable.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
