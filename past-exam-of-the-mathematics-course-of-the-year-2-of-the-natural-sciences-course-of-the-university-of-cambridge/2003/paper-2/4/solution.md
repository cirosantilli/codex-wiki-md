<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Compute the [complex derivative](../../../../complex-derivative.md) along horizontal and vertical increments. Along the real direction, $f'=u_x+iv_x$; along the imaginary direction, $f'=(u_y+iv_y)/i=v_y-iu_y$. Equality gives the [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md)

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

The real and imaginary parts of a [holomorphic function](../../../../holomorphic-function-split.md) are smooth. Equality of their [mixed partial derivatives](../../../../mixed-partial-derivative.md) then gives $u_{xx}+u_{yy}=v_{yx}-v_{xy}=0$ and $v_{xx}+v_{yy}=-u_{yx}+u_{xy}=0$, proving that both are [harmonic functions](../../../../harmonic-function.md).

For the first real part, $u_x=2x$ and $u_y=-2y$. The [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) require $v_y=2x$ and $v_x=2y$, so its [harmonic conjugate](../../../../harmonic-conjugate.md) is $v=2xy+C$. Therefore

$$
\boxed{f(z)=z^2+iC,\qquad C\in\mathbb R.}
$$

For the second real part, $u=x/(x^2+y^2)$ is the real part of $1/z$. Its [harmonic conjugate](../../../../harmonic-conjugate.md) is $-y/(x^2+y^2)+C$, giving

$$
\boxed{f(z)=\frac1z+iC,\qquad C\in\mathbb R,\quad z\ne0.}
$$

These are the most general answers on a connected open [domain](../../../../domain-mathematical-analysis.md): the difference of two candidates has zero real part, so the [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) make its imaginary part constant. The second [function](../../../../function-split.md) cannot extend [holomorphically](../../../../holomorphic-function-split.md) through zero.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
