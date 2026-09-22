<h1 id="d/d4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The function $h$ is measurable and nonnegative. In first-quadrant polar coordinates, including the Jacobian, its integral is

$$
\left(\int_0^\infty e^{-r^2}r^3dr\right)\left(\int_0^{\pi/2}(\cos\theta)^{3/2}(\sin\theta)^{1/2}d\theta\right).
$$

The radial factor is $1/2$ by the supplied fact and the angular integrand is at most one, giving finiteness. The nonnegative change-of-variables formula is valid before finiteness is known, and this bound proves $h\in L^1$.

Fubini may now factor the Cartesian integral. Substituting $u=x^2$, $v=y^2$ in the respective factors gives

$$
\iint h\,dxdy=\frac14\left(\int_0^\infty e^{-u}u^{1/4}du\right)\left(\int_0^\infty e^{-v}v^{-1/4}dv\right).
$$

Both are finite: their powers at zero exceed $-1$, and the exponential controls infinity. Comparing with the polar expression proves

$$
\boxed{\int_0^{\pi/2}(\cos\theta)^{3/2}(\sin\theta)^{1/2}d\theta=\frac12\Gamma(5/4)\Gamma(3/4),}
$$

which is exactly the product of integrals requested.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
