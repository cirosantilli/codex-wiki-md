<h1 id="15/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Substitute $x=r\cos\phi$, $y=r\sin\phi$ and include the [Jacobian determinant](../../../../../../jacobian-determinant.md) factor $r$. The integrand times the area element becomes

$$
\big(\cos\phi+\sin\phi+r\cos\phi\sin\phi\big)dr\,d\phi.
$$

Both terms containing one factor $\sin\phi$ are odd in $\phi$, while the radial bounds and angular interval are even. They therefore integrate to zero. The remaining [double integral](../../../../../../double-integral.md) is

$$
\begin{aligned}
I&=\int_{-\pi/3}^{\pi/3}\cos\phi\left(1+\cos\phi-\frac32\right)d\phi\\
&=\int_{-\pi/3}^{\pi/3}\left(\cos^2\phi-\frac12\cos\phi\right)d\phi
=\boxed{\frac\pi3-\frac{\sqrt3}{4}.}
\end{aligned}
$$

The domain stays away from $r=0$, so the denominator of the original integrand causes no singularity in this region.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [15](../../../15.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
