<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $0<b<\lambda=2$, integrate the identity $e^{bz}-1=\int_0^z be^{bt}\,dt$ for $z\geq0$. The [Tonelli theorem](../../../../../../tonelli-theorem.md) and the tail bound in (c) give

$$
\mathbb E e^{bZ}=1+b\int_0^\infty e^{bt}\mathbb P(Z>t)\,dt
\leq1+b\int_0^\infty e^{-(2-b)t}\,dt=\frac2{2-b}.
$$

For $b=0$ the [expectation](../../../../../../expected-value.md) is $1$, and for $b<0$ the fact $Z\geq0$ gives $0<e^{bZ}\leq1$. Therefore

$$
\boxed{\mathbb E e^{bZ}<\infty\quad\text{for every }b<2.}
$$

This is an [exponential moment bound for a Gaussian random-walk maximum](../../../../../../exponential-moment-bound-for-a-gaussian-random-walk-maximum.md). The upper-tail bound proves the requested sufficient range; it alone does not establish a converse at the endpoint.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
