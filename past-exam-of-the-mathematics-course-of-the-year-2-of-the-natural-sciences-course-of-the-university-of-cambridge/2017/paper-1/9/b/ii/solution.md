<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the density $1/y$ on the physical region $y>0$. It is singular at zero and would not describe a nonnegative density for $y<0$. The first integral gives $y\sqrt{1+y'^2}=R$ for a positive constant $R$. To handle the horizontal tangent without dividing by $y'$, use the full [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md):

$$
yy''+y'^2+1=0,\qquad (yy')'=-1.
$$

Two integrations give $y^2=-(x-x_0)^2+R^2$. The equal endpoint heights force $x_0=0$, and either endpoint then gives $R^2=2$. Thus

$$
\boxed{y(x)=\sqrt{2-x^2},\qquad -1\leq x\leq1.}
$$

The path is the upper circular arc. A constant horizontal path solves the differentiated first integral trivially but fails $yy''+y'^2+1=0$, so is not another extremum.

One can prove global minimality, rather than only stationarity. Define $\Phi(x,y)=\operatorname{arsinh}(x/y)$ on the upper half-plane. Then

$$
\nabla\Phi=\frac{(1,-x/y)}{\sqrt{x^2+y^2}},\qquad |\nabla\Phi|=\frac1y.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives, along any admissible path from $A$ to $B$,

$$
D=\int\frac{ds}{y}\geq\int\nabla\Phi\cdot d\mathbf r
=\Phi(1,1)-\Phi(-1,1)=2\operatorname{arsinh}1.
$$

Our circle has tangent $(1,-x/y)$ for increasing $x$, so equality holds pointwise. This [calibration for semicircular hyperbolic geodesics](../../../../../../calibration-for-semicircular-hyperbolic-geodesics.md) proves

$$
\boxed{D_{\min}=2\operatorname{arsinh}1=2\ln(1+\sqrt2).}
$$

The geometry is that of a [hyperbolic geodesic](../../../../../../geodesic-in-the-poincare-half-plane-model.md) in the [Poincaré half-plane model](../../../../../../poincare-half-plane-model.md). The proof even allows competing upper-half-plane paths beyond the class of monotonic graphs.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
