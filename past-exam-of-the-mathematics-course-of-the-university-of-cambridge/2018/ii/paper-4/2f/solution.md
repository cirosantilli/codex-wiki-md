<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

Let

$$
S=\sum_{n=1}^{\infty}\frac{m_n}{n!}.
$$

Assume for a contradiction that $S=a/b$ is [rational](../../../../../rational-number.md). For every $N\geq b$, both $N!S$ and

$$
N!\sum_{n=1}^{N}\frac{m_n}{n!}
$$

are [integers](../../../../../integer.md), because the $m_n$ are integers. Their positive difference

$$
R_N=N!\sum_{n=N+1}^{\infty}\frac{m_n}{n!}
=\sum_{k=1}^{\infty}
\frac{m_{N+k}}{(N+1)\cdots(N+k)}
$$

must therefore be a positive integer.

On the other hand, [concavity](../../../../../concave-function.md) of $x^\alpha$ for $0\leq\alpha<1$ gives $(N+k)^\alpha\leq N^\alpha+k^\alpha\leq N^\alpha+k$. Since $(N+1)\cdots(N+k)\geq(N+1)^k$,

$$
0<R_N
\leq A\sum_{k=1}^{\infty}\frac{N^\alpha+k}{(N+1)^k}
=A\left(N^{\alpha-1}+\frac{N+1}{N^2}\right)
\longrightarrow0.
$$

Eventually $0<R_N<1$, contradicting its integrality. Hence

$$
\boxed{\sum_{n=1}^{\infty}\frac{m_n}{n!}\text{ is irrational}.}
$$

The integrality assumption is essential. For example, take $\alpha=0$, $A=2$, and

$$
m_n=\frac2{e-1}\qquad(n\geq1).
$$

Then $1<m_n<2$, but the [exponential series](../../../../../exponential-series.md) gives

$$
\sum_{n=1}^{\infty}\frac{m_n}{n!}
=\frac2{e-1}\sum_{n=1}^{\infty}\frac1{n!}=2.
$$

Thus **the result does not remain true for arbitrary real $m_n$**.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
