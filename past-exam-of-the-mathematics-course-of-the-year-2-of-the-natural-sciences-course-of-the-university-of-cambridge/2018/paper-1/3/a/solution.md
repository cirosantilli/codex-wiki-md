<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x\ne\xi$, the homogeneous solutions are $e^x,e^{-x}$. The left [boundary condition](../../../../../boundary-condition.md) selects $\sinh x$, while boundedness at infinity selects $e^{-x}$ on the right. Thus write $G=A(\xi)\sinh x$ for $x<\xi$ and $G=B(\xi)e^{-x}$ for $x>\xi$.

A unit [Dirac delta distribution](../../../../../dirac-delta-function.md) in the second [derivative](../../../../../derivative.md) requires continuity of $G$ and a [derivative](../../../../../derivative.md) jump of one:

$$
A\sinh\xi=Be^{-\xi},\qquad
-Be^{-\xi}-A\cosh\xi=1.
$$

The second equation and the first give $-A e^\xi=1$, so the [Dirichlet half-line Green function for d2 minus 1](../../../../../dirichlet-half-line-green-function-for-d2-minus-1.md) is

$$
\boxed{G(x,\xi)=-\sinh(\min\{x,\xi\})e^{-\max\{x,\xi\}}
=-\frac12\left(e^{-|x-\xi|}-e^{-(x+\xi)}\right)}.
$$

The second expression is also a [method of images](../../../../../method-of-images.md) construction. Applying the [Green's function](../../../../../green-s-function-split.md) to the forcing gives

$$
\boxed{y(x)=-e^{-x}\int_0^x\sinh\xi\,f(\xi)\,d\xi
-\sinh x\int_x^\infty e^{-\xi}f(\xi)\,d\xi}.
$$

For bounded forcing this is bounded, vanishes at zero and solves the equation; a bounded homogeneous solution vanishing at zero is zero, proving uniqueness. More general forcing is allowed when the integrals converge and the resulting function has the required growth. Arbitrary unbounded forcing need not admit a bounded solution; this distinction is relevant in part (b).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
