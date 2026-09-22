<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Take fixed-endpoint variations $y_\varepsilon=y+\varepsilon\eta$ with $\eta(a)=\eta(b)=0$. The [first variation](../../../../first-variation.md) is

$$
\delta I=\int_a^b(f_y\eta+f_{y'}\eta')dx=\int_a^b\left(f_y-\frac d{dx}f_{y'}\right)\eta\,dx.
$$

The boundary term vanishes by the endpoint conditions. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) $f_y-d(f_{y'})/dx=0$. Along its solutions,

$$
\frac d{dx}(f-y'f_{y'})=f_x+y'\left(f_y-\frac d{dx}f_{y'}\right)=f_x.
$$

When $f_x=0$, this proves the [Beltrami identity](../../../../beltrami-identity.md) $f-y'f_{y'}=\text{constant}$.

For the surface $z=F(y)$, the [line element](../../../../line-element.md) is $ds^2=dx^2+[1+F'(y)^2]dy^2$. The arc-length integrand for a graph $y(x)$ is $\mathcal L=\sqrt{1+[1+F'(y)^2]y'^2}$. It has no explicit $x$ dependence and satisfies $\mathcal L-y'\mathcal L_{y'}=1/\mathcal L$. Thus $[1+F'(y)^2]y'^2$ is constant. Choosing the fixed direction along a smooth nonconstant segment and integrating yields

$$
\boxed{\int^y\sqrt{1+F'(s)^2}\,ds=ax+b.}
$$

The same result follows by defining the transverse arc coordinate $u(y)=\int^y\sqrt{1+F'(s)^2}ds$, which changes the metric to $ds^2=dx^2+du^2$. Its [geodesics](../../../../geodesic.md) are straight lines in $(x,u)$ coordinates. This proves the formula for [geodesics on a generalized cylinder](../../../../geodesics-on-a-generalized-cylinder.md) and shows it gives locally shortest paths. The additional straight lines $x=\text{constant}$ in the unrolled plane are also geodesics, but cannot be represented as graphs $y(x)$. Classical differential-geometric statements assume the surface has sufficient smoothness; the arc-length coordinate itself only requires the displayed integral to be well defined.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
