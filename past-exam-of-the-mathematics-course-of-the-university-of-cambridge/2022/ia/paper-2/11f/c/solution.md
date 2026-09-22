<h1 id="11f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the process to stop on toss $n$, the last toss must be the $k$th head, while the first $n-1$ tosses must contain exactly $k-1$ heads. Hence the [negative binomial distribution](../../../../../../negative-binomial-distribution.md) gives

$$
\boxed{
\mathbb P(T=n)
=\binom{n-1}{k-1}p^k(1-p)^{n-k}},
\qquad n\geq k.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
