<h1 id="14a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
g(x,t)=\frac1{\sqrt{4\pi Dt}}
\exp\left(-\frac{x^2}{4Dt}\right),
\qquad t>0.
$$

Convolution with the initial [Dirac delta function](../../../../../../dirac-delta-function.md) translates the [heat kernel](../../../../../../heat-kernel.md), while part (b) propagates the impulsive source from time one. Hence

$$
\boxed{
\theta_c(x,t)=g(x-2\sqrt D,t)
-A H(t-1)g(x+2\sqrt D,t-1)}.
$$

At $(x,t)=(0,2)$ this becomes

$$
\theta_c(0,2)
=\frac{e^{-1/2}}{\sqrt{8\pi D}}
-A\frac{e^{-1}}{\sqrt{4\pi D}}.
$$

It vanishes exactly when

$$
A=\frac{e^{-1/2}}{\sqrt{8\pi D}}
\frac{\sqrt{4\pi D}}{e^{-1}}
=\boxed{\sqrt{\frac e2}}.
$$

This is the [cancellation of two heat-kernel impulses](../../../../../../cancellation-of-two-heat-kernel-impulses.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14A](../../14a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
