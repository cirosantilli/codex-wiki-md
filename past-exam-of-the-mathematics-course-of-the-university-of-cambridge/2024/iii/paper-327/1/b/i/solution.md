<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
v(\lambda)=-i\int_1^\infty\frac{e^{-i\lambda x}}{x^2}\,dx.
$$

The integral is [absolutely convergent](../../../../../../../absolute-convergence.md). For a [Schwartz function](../../../../../../../schwartz-function.md) $\varphi$, [Fubini's theorem](../../../../../../../fubini-s-theorem.md) and [integration by parts](../../../../../../../integration-by-parts.md) in $\lambda$ give

$$
\begin{aligned}
\int_{\mathbb R}\varphi'(\lambda)v(\lambda)\,d\lambda
&=-i\int_1^\infty\frac1{x^2}
\left(\int_{\mathbb R}\varphi'(\lambda)e^{-i\lambda x}\,d\lambda\right)dx\\
&=-\int_1^\infty\frac1x
\left(\int_{\mathbb R}\varphi(\lambda)e^{-i\lambda x}\,d\lambda\right)dx\\
&=\langle\widehat u,\varphi\rangle.
\end{aligned}
$$

Equivalently, $v'=-\widehat u$ as a [distributional derivative](../../../../../../../distributional-derivative.md), and hence

$$
\boxed{\langle\widehat u,\varphi\rangle
=\int_{\mathbb R}\varphi'(\lambda)v(\lambda)\,d\lambda}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 327](../../../../paper-327-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
