<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $W=Y-\theta\sim G_0$ and suppose $a=\mathbb E_{G_0}[\psi'(W)]\ne0$. A first-order expansion of the [estimating equation](../../../../../../estimating-equation.md) $n^{-1}\sum_i\psi(Y_i-T_n)=0$ gives the [asymptotic linear representation](../../../../../../asymptotic-linear-representation.md)

$$
\sqrt n(T_n-\theta)
=\frac1a\frac1{\sqrt n}\sum_{i=1}^n\psi(W_i)+o_p(1).
$$

The [central limit theorem](../../../../../../central-limit-theorem.md) therefore yields

$$
\boxed{\sqrt n(T_n-\log\sigma^2)
\xrightarrow d
N\!\left(0,
\frac{\mathbb E_{G_0}[\psi(W)^2]}
{\{\mathbb E_{G_0}[\psi'(W)]\}^2}
\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
