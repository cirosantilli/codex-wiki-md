<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [test function](../../../../../../test-function.md) $f\in\mathcal D(\mathbb R)$, define the proposed integral by reversing the order of integration:

$$
\langle I,f\rangle
=\int_{\mathbb R}
\left(\int_{\mathbb R}f(x)e^{ix\sqrt{\theta^2+1}}\,dx\right)d\theta
=\int_{\mathbb R}
\widehat f\bigl(-\sqrt{\theta^2+1}\bigr)\,d\theta.
$$

The [Fourier transform](../../../../../../fourier-transform.md) of a test function is a [Schwartz function](../../../../../../schwartz-function.md), while $\sqrt{\theta^2+1}\asymp1+|\theta|$. The final integral is consequently [absolutely convergent](../../../../../../absolute-convergence.md). Repeated [integration by parts](../../../../../../integration-by-parts.md) in $x$ bounds it by finitely many [seminorms](../../../../../../seminorm.md) of the test function, so it defines a [continuous linear functional](../../../../../../continuous-dual-space-split.md) on $\mathcal D(\mathbb R)$.

Equivalently, put $\lambda=\sqrt{\theta^2+1}$ on the two half-lines. Then

$$
\langle I,f\rangle
=2\int_1^\infty
\widehat f(-\lambda)
\frac{\lambda}{\sqrt{\lambda^2-1}}\,d\lambda.
$$

The density has only an integrable inverse-square-root singularity at one and is bounded at infinity, so it is a regular [tempered distribution](../../../../../../tempered-distribution.md). Its inverse [Fourier transform](../../../../../../fourier-transform.md) is exactly the proposed oscillatory integral. Thus

$$
\boxed{\int_{\mathbb R}e^{ix\sqrt{\theta^2+1}}\,d\theta
\in\mathcal D'(\mathbb R)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
