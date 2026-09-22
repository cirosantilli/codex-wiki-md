<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a locally integrable $u$, the [change of variables formula](../../../../../../change-of-variables-formula.md) $y=Ax$ gives

$$
\int_{\mathbb R^n}u(Ax)\varphi(x)\,dx
=\frac1{|\det A|}
\int_{\mathbb R^n}u(y)\varphi(A^{-1}y)\,dy.
$$

This motivates

$$
\boxed{
\langle A^*u,\varphi\rangle
=\frac1{|\det A|}
\langle u,(A^{-1})^*\varphi\rangle}.
$$

Because pullback by an invertible linear map acts continuously on the [Schwartz space](../../../../../../schwartz-space.md), the right side is a continuous linear functional of $\varphi$. It therefore defines a [tempered distribution](../../../../../../tempered-distribution.md) and agrees with ordinary pullback when $u$ is a function.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
