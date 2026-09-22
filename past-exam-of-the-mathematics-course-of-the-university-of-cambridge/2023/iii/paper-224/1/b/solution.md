<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $p=(1+\mu)^{-1}$. Since $X$ and the [geometric random variable](../../../../../../geometric-distribution.md) $Z$ have the same [expected value](../../../../../../expected-value.md) $\mu$,

$$
\begin{aligned}
D(P_X\Vert P_Z)
&=\sum_{k\geq0}P_X(k)\log_2\frac{P_X(k)}{p(1-p)^k}\\
&=-H(X)-\log_2p-\mu\log_2(1-p)\\
&=H(Z)-H(X).
\end{aligned}
$$

This is also the entropy deficit relative to the [maximum entropy distribution on the nonnegative integers](../../../../../../maximum-entropy-distribution-on-the-nonnegative-integers.md).

The random variables $X$ and $-Z$ are independent, so part a gives $H(X-Z)\geq H(-Z)=H(Z)$. Consequently

$$
\begin{aligned}
2d_R(X,Z)-D(P_X\Vert P_Z)
&=2H(X-Z)-H(X)-H(Z)-\{H(Z)-H(X)\}\\
&=2\{H(X-Z)-H(Z)\}\geq0,
\end{aligned}
$$

which is the required bound in terms of the [Entropic Ruzsa distance](../../../../../../entropic-ruzsa-distance.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
