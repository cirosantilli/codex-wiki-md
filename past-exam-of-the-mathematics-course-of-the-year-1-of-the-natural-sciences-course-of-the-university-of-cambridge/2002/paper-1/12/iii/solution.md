<h1 id="12/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Expand the constant right-edge value in a [Fourier sine series](../../../../../fourier-sine-series.md). Its coefficients are

$$
b_n=\frac2\pi\int_0^\pi\sin(ny)dy=\frac{2[1-(-1)^n]}{n\pi}.
$$

The [superposition principle](../../../../../superposition-principle.md) combines the normalized modes, giving

$$
\boxed{f(x,y)=\frac4\pi\sum_{m=0}^\infty\frac{\sinh[(2m+1)x]}{(2m+1)\sinh[(2m+1)\pi]}\sin[(2m+1)y].}
$$

This is a [harmonic function in a rectangle with one constant boundary value](../../../../../harmonic-function-in-a-rectangle-with-one-constant-boundary-value.md), with the coordinate roles interchanged. The series and its derivatives converge uniformly on compact subsets of $0<x<\pi$, so it satisfies [Laplace's equation](../../../../../laplace-equation.md) there. It vanishes on the other three edges and approaches one at every interior point of the right edge. At the two right corners the one-sided prescribed values disagree; no continuous extension can satisfy both. The stated open-edge condition avoids that incompatibility, and isolated corner assignments do not change the bounded interior [Dirichlet problem](../../../../../dirichlet-problem.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
