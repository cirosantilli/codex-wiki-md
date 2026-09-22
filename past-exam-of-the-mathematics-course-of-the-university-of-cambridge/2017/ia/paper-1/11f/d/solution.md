<h1 id="11f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We first prove by induction that

$$
a_n\geq2^n\qquad(n\geq1).
$$

It holds for $n=1$, and if it holds at $n$, then

$$
a_{n+1}=2^{a_n}\geq2^{2^n}\geq2^{n+1}.
$$

Consequently

$$
0\leq\frac{2n^k}{a_n}\leq2^{1-n}n^k.
$$

Part (c) and the [squeeze theorem](../../../../../../squeeze-theorem.md) now give

$$
\boxed{\lim_{n\to\infty}\frac{2n^k}{a_n}=0}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11F](../../11f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
