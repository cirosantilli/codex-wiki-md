<h1 id="12f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [partition of an interval](../../../../../../partition-of-an-interval.md) $P:0=x_0<\cdots<x_m=1$, put

$$
M_j=\sup_{x\in[x_{j-1},x_j]}f(x),
\qquad
m_j=\inf_{x\in[x_{j-1},x_j]}f(x).
$$

The [upper Darboux sum](../../../../../../upper-darboux-sum.md) and [lower Darboux sum](../../../../../../lower-darboux-sum.md) are

$$
U(f,P)=\sum_{j=1}^mM_j(x_j-x_{j-1}),
\qquad
L(f,P)=\sum_{j=1}^mm_j(x_j-x_{j-1}).
$$

The upper and lower integrals are

$$
\overline{\int_0^1}f=\inf_PU(f,P),
\qquad
\underline{\int_0^1}f=\sup_PL(f,P).
$$

The bounded function is [Riemann integrable](../../../../../../riemann-integrable-function.md) when these values agree, and their common value is its [Riemann integral](../../../../../../riemann-integral.md).

For the indicator of the rational numbers, every nondegenerate interval contains both a [rational number](../../../../../../rational-number.md) and an [irrational number](../../../../../../irrational-number.md). Hence every upper sum is one and every lower sum is zero. The function is not Riemann integrable.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
