<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [hyperbolic cotangent](../../../../hyperbolic-cotangent.md) is

$$
\coth x=\frac{e^x+e^{-x}}{e^x-e^{-x}}=\frac{e^{2x}+1}{e^{2x}-1},\qquad x\ne0.
$$

Expand the numerator and denominator using the exponential [Maclaurin series](../../../../maclaurin-series.md):

$$
\coth x=\frac1x\frac{1+x^2/2+x^4/24+O(x^6)}{1+x^2/6+x^4/120+O(x^6)}
=\boxed{\frac1x+\frac x3-\frac{x^3}{45}+O(x^5).}
$$

This is a [Laurent series](../../../../laurent-series.md), rather than an ordinary [Maclaurin series](../../../../maclaurin-series.md): $\coth x$ has a simple [pole](../../../../pole.md) at zero. The printed request should be understood as the expansion obtained from the exponential series, including this unavoidable $x^{-1}$ term.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
