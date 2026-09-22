<h1 id="a/1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

On the selected [steepest descent contour](../../../../../steepest-descent-contour.md) put $t=e^{i\pi/6}r$, $r\geq0$. Then $it^3=-r^3$ and $dt=e^{i\pi/6}\,dr$. Its exact contribution is

$$
I_0(x)=e^{i\pi/6}\int_0^\infty e^{-xr^3}\,dr
=\frac{e^{i\pi/6}}{3x^{1/3}}\int_0^\infty e^{-s}s^{-2/3}\,ds.
$$

Use the [Gamma function](../../../../../gamma-function.md) integral and its recurrence $\Gamma(4/3)=\Gamma(1/3)/3$ to obtain

$$
\boxed{I_0(x)=e^{i\pi/6}\Gamma(4/3)x^{-1/3}.}
$$

There is no remainder here: the complete infinite descent ray was integrated exactly.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
