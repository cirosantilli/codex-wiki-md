<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [derivative](../../../../../derivative.md) of an [analytic function](../../../../../holomorphic-function-split.md) must be independent of the direction of approach. Taking a real increment gives $f'(z)=u_x+iv_x$; taking an imaginary increment gives

$$
f'(z)=\frac{u_y+iv_y}{i}=v_y-iu_y.
$$

Equality of real and imaginary parts proves the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md):

$$
\boxed{u_x=v_y,\qquad u_y=-v_x}.
$$

A real [harmonic function](../../../../../harmonic-function.md) is a twice continuously differentiable function whose [Laplacian](../../../../../laplacian.md) vanishes. For the given logarithmic function and $x^2+y^2>0$,

$$
u_x=\frac{2x}{x^2+y^2},\quad u_y=\frac{2y}{x^2+y^2},\quad
u_{xx}+u_{yy}=\frac4{x^2+y^2}-\frac{4(x^2+y^2)}{(x^2+y^2)^2}=0.
$$

It is therefore harmonic everywhere on the [punctured complex plane](../../../../../punctured-complex-plane.md).

On any domain admitting a [branch of the complex logarithm](../../../../../branch-of-the-complex-logarithm.md), choose

$$
\boxed{v(x,y)=2\operatorname{Arg}(x+iy)+C,\qquad u+iv=2\operatorname{Log}z+iC}.
$$

Its [derivatives](../../../../../derivative.md) are $v_x=-2y/(x^2+y^2)$ and $v_y=2x/(x^2+y^2)$, as required. For example, the principal [complex logarithm](../../../../../complex-logarithm.md) gives such a [harmonic conjugate](../../../../../harmonic-conjugate.md) on the plane cut along the negative real axis.

There is no single-valued [harmonic conjugate](../../../../../harmonic-conjugate.md) on the whole punctured plane. Indeed its putative differential would satisfy

$$
\oint_{|z|=1}dv=\oint_{|z|=1}\left(-\frac{2y}{x^2+y^2}\,dx+\frac{2x}{x^2+y^2}\,dy\right)=4\pi,
$$

whereas a globally defined function has zero integral of its differential around a closed curve. This is the [log modulus has no global harmonic conjugate on the punctured plane](../../../../../log-modulus-has-no-global-harmonic-conjugate-on-the-punctured-plane.md) obstruction. Thus the conjugate requested in the question must be interpreted locally or on a cut plane.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
