<h1 id="17f/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose each vertex independently with probability

$$
p=\frac{4n}{e}\leq1
$$

and take the induced drawing. Let its numbers of vertices, edges, and crossing pairs be $N,E,T$. Since crossing edges have four distinct endpoints,

$$
\mathbb E N=pn,\qquad
\mathbb E E=p^2e,\qquad
\mathbb E T=p^4t(G).
$$

Part (i), with the harmless positive constant dropped, gives $T\geq E-3N$ for every outcome. Taking expectations,

$$
p^4t(G)\geq p^2e-3pn.
$$

For $p=4n/e$, the right side is $4n^2/e$. Dividing by $p^4=256n^4/e^4$ proves the [crossing lemma](../../../../../../../crossing-lemma.md) estimate

$$
\boxed{t(G)\geq\frac{e^3}{64n^2}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [17F](../../../17f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
