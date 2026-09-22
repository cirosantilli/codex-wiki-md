<h1 id="d/d2/solution">Solution</h1>

↑ **Parent:** [D2](../d2.md)

The annulus is open and hence [Lebesgue measurable](../../../../lebesgue-measurable-set.md); multiplying its indicator by the continuous Gaussian gives a measurable function. It is bounded by the indicator of $[-b,b]^2$, whose [Lebesgue integral](../../../../lebesgue-integral.md) is $4b^2$. Thus it is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) by comparison.

Use the [change of variables formula](../../../../change-of-variables-formula.md) with [polar coordinates](../../../../polar-coordinates.md) $x=r\cos\theta$, $y=r\sin\theta$. Removing one radial cut makes this a smooth one-to-one coordinate map; the cut is a [null set](../../../../null-set.md) and does not affect the integral. The absolute [Jacobian determinant](../../../../jacobian-determinant.md) is $r$. By [Fubini theorem](../../../../fubini-s-theorem.md),

$$
\int_V e^{-(x^2+y^2)/2}\,d(x,y)=\int_0^{2\pi}\int_a^b e^{-r^2/2}r\,dr\,d\theta
=\boxed{2\pi(e^{-a^2/2}-e^{-b^2/2})}.
$$

The antiderivative is $-e^{-r^2/2}$, which also makes the sign of the answer transparent.

## ↑ Ancestors (12)

1. [D2](../d2.md)
2. [D](../../d.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
