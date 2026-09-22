<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [character formula for an induced representation](../../../../../../character-formula-for-an-induced-representation.md). For $g\in G$,

$$
\begin{aligned}
\chi(g)(\phi\!\uparrow_H^G)(g)
&=\frac1{|H|}\sum_{\substack{x\in G\\x^{-1}gx\in H}}
\chi(g)\phi(x^{-1}gx)\\
&=\frac1{|H|}\sum_{\substack{x\in G\\x^{-1}gx\in H}}
\chi(x^{-1}gx)\phi(x^{-1}gx)\\
&=\bigl((\chi\!\downarrow_H)\phi\bigr)\!\uparrow_H^G(g).
\end{aligned}
$$

The middle equality uses that a [character of a representation](../../../../../../character-of-a-representation.md) is constant on conjugacy classes. This proves the [tensor identity for an induced character](../../../../../../tensor-identity-for-an-induced-character.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 160](../../../paper-160-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
