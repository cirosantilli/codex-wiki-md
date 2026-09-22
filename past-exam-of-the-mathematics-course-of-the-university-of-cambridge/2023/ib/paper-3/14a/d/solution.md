<h1 id="14a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the [Fourier transform](../../../../../../fourier-transform.md) in $x$. The [wave equation](../../../../../../wave-equation-split.md) becomes the [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\partial_t^2\widetilde u(k,t)+k^2\widetilde u(k,t)=0,
$$

with initial data $\widetilde u(k,0)=\widetilde f(k)$ and $\partial_t\widetilde u(k,0)=\widetilde g(k)$. Therefore

$$
\widetilde u(k,t)=\widetilde f(k)\cos(kt)
+\widetilde g(k)\frac{\sin(kt)}k.
$$

Part (c) and the [Translation property of the Fourier transform](../../../../../../translation-property-of-the-fourier-transform.md) invert the first term to

$$
\frac12\{f(x+t)+f(x-t)\}.
$$

For the second term choose an [antiderivative](../../../../../../antiderivative.md) $p$ of $g$. By part (b), $\widetilde g=ik\widetilde p$, and hence

$$
\widetilde g(k)\frac{\sin(kt)}k
=\frac12\widetilde p(k)\{e^{ikt}-e^{-ikt}\}.
$$

Its inverse transform is

$$
\frac12\{p(x+t)-p(x-t)\}
=\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi.
$$

Combining the terms gives the [D'Alembert formula](../../../../../../d-alembert-s-formula.md)

$$
\boxed{u(x,t)=\frac12\{f(x+t)+f(x-t)\}
+\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [14A](../../14a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
