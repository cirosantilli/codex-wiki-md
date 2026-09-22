<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
m_n=\min_{0\leq x\leq n^{-1/2}}f(x),
\qquad
M_n=\max_{0\leq x\leq n^{-1/2}}f(x).
$$

Continuity at zero gives $m_n,M_n\to f(0)$. Part (a), with the positive weight $ne^{-nx}$, gives

$$
m_n(1-e^{-\sqrt n})
\leq
\int_0^{1/\sqrt n}nf(x)e^{-nx}\,dx
\leq
M_n(1-e^{-\sqrt n}).
$$

The [squeeze theorem](../../../../../../squeeze-theorem.md) therefore yields

$$
\boxed{
\int_0^{1/\sqrt n}nf(x)e^{-nx}\,dx\to f(0)}.
$$

Since $f$ is bounded on $[0,1]$, say $|f|\leq K$, the omitted tail satisfies

$$
\left|
\int_{1/\sqrt n}^1nf(x)e^{-nx}\,dx
\right|
\leq K(e^{-\sqrt n}-e^{-n})\longrightarrow0.
$$

Adding the tail proves

$$
\boxed{\int_0^1nf(x)e^{-nx}\,dx\to f(0)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
