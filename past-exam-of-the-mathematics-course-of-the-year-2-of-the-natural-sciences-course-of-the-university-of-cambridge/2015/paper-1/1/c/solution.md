<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Only the quartic term contributes to the [Laplacian](../../../../../laplacian.md). The mixed cubic has zero second [derivative](../../../../../derivative.md) in each coordinate, while the exponential–trigonometric pairs are harmonic:

$$
\Delta(z^4)=12z^2,\quad\Delta(xyz)=0,\quad\Delta(e^{-3y}\cos3x)=0,\quad\Delta(e^{2x}\sin2y)=0.
$$

Using $z=r\cos\alpha$ and the [Jacobian determinant](../../../../../jacobian-determinant.md) from part (a), the [divergence theorem](../../../../../divergence-theorem.md) gives

$$
\begin{aligned}
I&=12\int_0^{2\pi}\int_{-\pi}^{\pi}\int_0^R r^3\cos^2\alpha(1+r\sin\alpha)\,dr\,d\alpha\,d\beta\\
&=12(2\pi)\left(\int_{-\pi}^{\pi}\cos^2\alpha\,d\alpha\right)\frac{R^4}{4}=\boxed{6\pi^2R^4}.
\end{aligned}
$$

The term containing $\sin\alpha\cos^2\alpha$ integrates to zero. Equivalently, the [second vertical moment of a solid ring torus](../../../../../second-vertical-moment-of-a-solid-ring-torus.md) with major radius one is $\int_Vz^2dV=\pi^2R^4/2$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
