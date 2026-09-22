<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Induction shows $(PAP^{-1})^k=PA^kP^{-1}$ for every nonnegative integer $k$: in a product, adjacent factors $P^{-1}P$ cancel. At $k=0$, this is $I=PIP^{-1}$. Hence each partial sum of the [matrix exponential](../../../../../matrix-exponential.md) satisfies

$$
\sum_{k=0}^N\frac{(PAP^{-1})^k}{k!}
=P\left(\sum_{k=0}^N\frac{A^k}{k!}\right)P^{-1}.
$$

The series is absolutely convergent, since a submultiplicative [matrix norm](../../../../../matrix-norm.md) bounds it by $\sum_k\|A\|^k/k!=e^{\|A\|}$. Passing to the limit therefore proves that the [matrix exponential respects similarity](../../../../../matrix-exponential-respects-similarity.md):

$$
\boxed{e^{PAP^{-1}}=Pe^AP^{-1}}.
$$

No [diagonalizability](../../../../../diagonalizable-matrix.md) assumption is required.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
