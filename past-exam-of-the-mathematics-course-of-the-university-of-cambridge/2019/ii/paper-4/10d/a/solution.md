<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [multiplicative order](../../../../../../multiplicative-order.md) of $\alpha$ modulo $N$ is the least positive integer $r$ such that

$$
\alpha^r\equiv1\pmod N.
$$

It exists because $\alpha$ and $N$ are [coprime integers](../../../../../../coprime-integers.md).

Suppose that $r$ is [even](../../../../../../even-function.md) and

$$
\alpha^{r/2}\not\equiv-1\pmod N.
$$

The minimality of $r$ also gives $\alpha^{r/2}\not\equiv1\pmod N$. Since

$$
(\alpha^{r/2}-1)(\alpha^{r/2}+1)
=\alpha^r-1\equiv0\pmod N,
$$

the [factor extraction from an even modular order](../../../../../../factor-extraction-from-an-even-modular-order.md) yields

$$
\boxed{\gcd(\alpha^{r/2}-1,N)}
$$

as a nontrivial factor of $N$; equivalently one may also compute $\gcd(\alpha^{r/2}+1,N)$. Thus the required conditions are that $r$ be even and that $\alpha^{r/2}\not\equiv-1\pmod N$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
