<h1 id="3f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [moment-generating function](../../../../../../moment-generating-function.md) is $M_Y(t)=\mathbb E[e^{tY}]$ for real $t$ where this expectation is finite; a finite neighborhood of zero is usually required when speaking of an existing [moment-generating function](../../../../../../moment-generating-function.md). For a [standard normal distribution](../../../../../../standard-normal-distribution.md), completing the square gives

$$
M_Y(t)=\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{ty-y^2/2}\,dy
=e^{t^2/2}\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{-(y-t)^2/2}\,dy.
$$

The translated [Gaussian density](../../../../../../multivariate-normal-density.md) integrates to one, so

$$
\boxed{M_Y(t)=e^{t^2/2}\quad(t\in\mathbb R).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3F](../../3f.md)
3. [Section I](../../section-i.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
