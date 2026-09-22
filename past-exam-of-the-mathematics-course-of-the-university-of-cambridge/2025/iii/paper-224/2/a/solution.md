<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X_1,X_2,\ldots$ be i.i.d. with mass function $Q$ on a finite alphabet, and let $\widehat P_n$ be their [empirical distribution](../../../../../../type-information-theory.md). [Sanov theorem](../../../../../../sanov-theorem.md) states that for every set $\Gamma$ of probability mass functions,

$$
-\inf_{R\in\Gamma^\circ}D_e(R\Vert Q)
\leq\liminf_{n\to\infty}\frac1n\log\mathbb P(\widehat P_n\in\Gamma)
$$

and

$$
\limsup_{n\to\infty}\frac1n\log\mathbb P(\widehat P_n\in\Gamma)
\leq-\inf_{R\in\overline\Gamma}D_e(R\Vert Q),
$$

where interior and closure use the probability-simplex topology. Thus the empirical distributions satisfy a [large deviation principle](../../../../../../large-deviation-principle.md) with rate function $D_e(\mathord\cdot\Vert Q)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
