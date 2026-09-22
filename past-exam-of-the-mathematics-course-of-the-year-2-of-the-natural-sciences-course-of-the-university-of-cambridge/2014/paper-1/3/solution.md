<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Kernel conditions.** The [clamped-beam Green function](../../../../clamped-beam-green-function.md) must obey $G(0,\xi)=G_x(0,\xi)=G(1,\xi)=G_x(1,\xi)=0$. Away from $x=\xi$, $G_{xxxx}=0$. At the load point, $G,G_x,G_{xx}$ are continuous and

$$
\boxed{G_{xxx}(\xi+,\xi)-G_{xxx}(\xi-,\xi)=1.}
$$

A jump in any lower [derivative](../../../../derivative.md) would create a [derivative](../../../../derivative.md) of the [Dirac delta](../../../../dirac-delta-function.md), rather than the single point load required by $D_x^4G=\delta(x-\xi)$.

**Construction.** A particularly simple representation is

$$
G(x,\xi)=ax^2+bx^3+\frac{(x-\xi)_+^3}{6}.
$$

It already enforces the left-end conditions and the correct source jump. The right-end conditions give $a+b=-(1-\xi)^3/6$ and $2a+3b=-(1-\xi)^2/2$, hence

$$
a=\frac{\xi(1-\xi)^2}{2},\qquad b=-\frac{(1-\xi)^2(1+2\xi)}6.
$$

For $x<\xi$ this is already factored; for $x>\xi$, expanding and refactoring gives

$$
\boxed{G(x,\xi)=\begin{cases}\dfrac{x^2(1-\xi)^2}{6}[3\xi-(1+2\xi)x],&x\leq\xi,\\\dfrac{\xi^2(1-x)^2}{6}[3x-(1+2x)\xi],&x\geq\xi.\end{cases}}
$$

The formulas agree at the junction. The forced displacement is obtained by integrating this kernel against $f$; for continuous loads it satisfies the equation and all four end conditions. Uniqueness follows because a cubic with zero value and slope at both ends is identically zero.

**Reciprocity.** In terms of $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$, the same expression is

$$
G(x,\xi)=\frac{x_<^2(1-x_>)^2}{6}[3x_>-(1+2x_>)x_<].
$$

It is visibly symmetric under interchange of $x$ and $\xi$. Thus the [reciprocity of the clamped-beam Green function](../../../../reciprocity-of-the-clamped-beam-green-function.md) gives

$$
\boxed{y_1(x_2)=G(x_2,x_1)=G(x_1,x_2)=y_2(x_1).}
$$

Equivalently, two [integrations by parts](../../../../integration-by-parts.md) show [self-adjointness](../../../../self-adjoint-operator.md) of $D_x^4$ under the clamped conditions, with bilinear form $\int u''v''dx$.

<a id="3/image-point-load-deflections-and-the-symmetric-green-function-of-a-clamped-beam"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1-q3-clamped-beam-kernel.png)

**[Figure 1](#3/image-point-load-deflections-and-the-symmetric-green-function-of-a-clamped-beam). Point-load deflections and the symmetric Green function of a clamped beam**.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
