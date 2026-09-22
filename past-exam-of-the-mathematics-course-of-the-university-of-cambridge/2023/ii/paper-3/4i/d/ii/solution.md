<h1 id="4i/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The grammars are non-equivalent. In the first grammar, terminal derivations without $AB\to c$ give

$$
\{a^rb^s:r,s\geq1\}.
$$

After applying $B\to Bb$ any number of times while $A$ and $B$ remain adjacent, the production $AB\to c$ also gives

$$
\{cb^t:t\geq0\}.
$$

Hence, in particular, $ab\in L(G_0)$ and $c\in L(G_0)$.

In the second grammar, the fixed terminals $ab$ in $XabY$ prevent $X$ and $Y$ from ever becoming adjacent, so $XY\to c$ can never be used. The remaining productions give exactly

$$
L(G_1)=\{a^rb^s:r,s\geq2\}.
$$

**Thus $ab,c\notin L(G_1)$, proving that the generated [languages](../../../../../../../formal-language-theory.md) differ.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [4I](../../../4i.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
