<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Inside the unit circle, use the [geometric series](../../../../geometric-series.md) for $1/(1-z)$:

$$
\boxed{\frac1{z^2(z-1)}=-\sum_{n=0}^{\infty}z^{n-2}=-\frac1{z^2}-\frac1z-1-z-z^2-\cdots,\qquad0<|z|<1.}
$$

Outside the unit circle, expand in powers of $1/z$ instead:

$$
\boxed{\frac1{z^2(z-1)}=\frac1{z^3}\frac1{1-z^{-1}}=\sum_{n=0}^{\infty}z^{-n-3},\qquad |z|>1.}
$$

The different [Laurent series](../../../../laurent-series.md) reflect different annuli separated by the [pole](../../../../pole.md) at one. Both follow from absolutely convergent [geometric series](../../../../geometric-series.md) in their stated regions.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
