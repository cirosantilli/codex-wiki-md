<h1 id="31e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The initial data require $\Phi(\xi)=\exp[-(2\nu)^{-1}\int_{x_*}^{\xi}U(s)\,ds]$, up to a positive constant that cancels from $u$. Substituting this into the [heat kernel](../../../../../../heat-kernel.md) formula gives the exponent $-G/(2\nu)$ with

$$
\boxed{G(x,\xi,t)=\frac{(x-\xi)^2}{2t}+\int_{x_*}^{\xi}U(s)\,ds.}
$$

Differentiate the kernel integral in $x$ and apply the [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md). Its constant prefactor cancels, leaving

$$
u(x,t)=\frac{\int_{\mathbb R}(x-\xi)t^{-1}e^{-G/(2\nu)}\,d\xi}{\int_{\mathbb R}e^{-G/(2\nu)}\,d\xi}.
$$

The choice of $x_*$ adds an irrelevant constant to $G$; the usual convergence assumptions on the initial data justify the integrals and differentiation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [31E](../../31e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
