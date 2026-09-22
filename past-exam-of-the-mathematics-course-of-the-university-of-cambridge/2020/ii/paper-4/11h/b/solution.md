<h1 id="11h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take both functions to be the constant arithmetic function $1$. Then

$$
(1\star1)(n)=\sum_{d\mid n}1=\tau(n),
$$

so the [divisor function](../../../../../../divisor-function.md) is multiplicative by part (a). For $s$ with $\operatorname{Re}s>1$, the relevant [Dirichlet series](../../../../../../dirichlet-series.md) are absolutely convergent, so their [Cauchy product](../../../../../../cauchy-product.md) may be rearranged:

$$
\begin{aligned}
\zeta(s)^2
&=\sum_{a,b\geq1}\frac1{(ab)^s}
=\sum_{n\geq1}\frac1{n^s}\sum_{a\mid n}1
=\sum_{n\geq1}\frac{\tau(n)}{n^s}.
\end{aligned}
$$

Equivalently, Dirichlet convolution becomes multiplication of absolutely convergent Dirichlet series.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11H](../../11h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
