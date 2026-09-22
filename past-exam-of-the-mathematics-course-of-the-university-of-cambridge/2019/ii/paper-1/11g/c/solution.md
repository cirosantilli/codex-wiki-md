<h1 id="11g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply part (b) repeatedly. After the first puncturing, the code has rank $k-1$, length $n-d$, and minimum distance at least $\lceil d/2\rceil$. Repeating with a minimum-weight codeword at each stage gives

$$
n\geq d+\left\lceil\frac d2\right\rceil
+\left\lceil\frac d{2^2}\right\rceil+cdots
+\left\lceil\frac d{2^{k-1}}\right\rceil,
$$

because nested ceilings obey

$$
\left\lceil\frac{\lceil d/2^j\rceil}{2}\right\rceil
=\left\lceil\frac d{2^{j+1}}\right\rceil.
$$

Thus

$$
\boxed{n\geq d+\sum_{1\leq l\leq k-1}
\left\lceil\frac d{2^l}\right\rceil},
$$

which is the binary [Griesmer bound](../../../../../../griesmer-bound.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11G](../../11g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
