<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $f=u+iv$ be analytic on a neighbourhood of a bounded planar region $\Omega$ and its piecewise smooth boundary $C$, oriented with $\Omega$ on the left. The [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) states

$$
\boxed{\oint_Cf(z)\,dz=0.}
$$

For a region with holes, $C$ includes the clockwise inner boundaries as well as the counterclockwise outer one. In particular, the integral around a closed contour bounding a region throughout which $f$ is analytic is zero.

To prove this classical form, expand the line integral and apply [Green's theorem](../../../../../green-theorem.md) to its real and imaginary parts:

$$
\begin{aligned}
\oint_C f\,dz
&=\oint_C(u\,dx-v\,dy)+i\oint_C(v\,dx+u\,dy)\\
&=\iint_\Omega(-v_x-u_y)\,dx\,dy+i\iint_\Omega(u_x-v_y)\,dx\,dy.
\end{aligned}
$$

Both integrands vanish by the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md), $u_x=v_y$ and $u_y=-v_x$. Analyticity supplies the continuous first partial derivatives needed by this [Green's theorem](../../../../../green-theorem.md) proof. The requirement that the enclosed region contain no singularities is essential.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
