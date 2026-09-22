<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $p_n=\mathbb P(A_n)$. Independence gives, first for finite partial counts and then by monotone convergence,

$$
\mathbb E[2^{-N}]
=\prod_{n\geq1}
\mathbb E[2^{-\mathbf1_{A_n}}]
=\prod_{n\geq1}\left(1-\frac{p_n}{2}\right).
$$

Using $1-x\leq e^{-x}$ factor by factor,

$$
\boxed{
\mathbb E[2^{-N}]
\leq\exp\left(-\frac12\sum_{n\geq1}p_n\right)
=e^{-\mathbb E[N]/2}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
