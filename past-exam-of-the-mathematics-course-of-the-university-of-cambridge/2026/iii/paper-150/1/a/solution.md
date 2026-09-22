<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf1(n)=1$. The basic [Von Mangoldt divisor identity](../../../../../../von-mangoldt-divisor-identity.md) is

$$
\log n=\sum_{d\mid n}\Lambda(d),
$$

because if $n=\prod_pp^{v_p(n)}$, the right-hand side is $\sum_pv_p(n)\log p=\log n$. In terms of [Dirichlet convolution](../../../../../../dirichlet-convolution.md), this says $\log=\mathbf1*\Lambda$. Since the [Möbius function](../../../../../../mobius-function.md) is the convolution inverse of $\mathbf1$, convolving with $\mu$ gives $\Lambda=\mu*\log$. Consequently

$$
\boxed{\Lambda(n)=\sum_{d\mid n}\mu(d)\log\frac nd.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
