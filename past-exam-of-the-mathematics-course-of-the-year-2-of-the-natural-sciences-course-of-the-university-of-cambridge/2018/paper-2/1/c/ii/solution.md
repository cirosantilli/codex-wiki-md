<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the integral's multiplier in the [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) basis:

$$
(1-x^2)^{-1/2}+(1-x^2)^{1/2}
=w(2-x^2)=w\left(\frac32y_0-\frac12y_2\right).
$$

At $\gamma^2=5$, part (i) gives

$$
Z=\left(\frac15+\frac{\varepsilon^2}{20}\right)y_0
+\frac\varepsilon4y_1+\frac{\varepsilon^2}{4}y_2+O(\varepsilon^3).
$$

By [orthogonality](../../../../../../orthogonal-vectors.md), the $y_1$ term and all cross terms vanish. Using $I_0=\pi$ and $I_2=\pi/2$, the integral is

$$
\frac32\pi\left(\frac15+\frac{\varepsilon^2}{20}\right)
-\frac12\frac\pi2\frac{\varepsilon^2}{4}+O(\varepsilon^3)
=\boxed{\frac{3\pi}{10}+\frac{\pi}{80}\varepsilon^2+O(\varepsilon^3)}.
$$

The remainder can be integrated against this integrable weight in the regular expansion, so it retains the stated order.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
