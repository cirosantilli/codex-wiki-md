<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

For fixed endpoints and a regular integral constraint, [Lagrange multipliers](../../../../lagrange-multiplier.md) replace the constrained stationarity problem by stationarity of $I-\lambda J$, with constant $\lambda$. Writing $H=F-\lambda G$, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is $H_y-(d/dx)H_{y'}=0$. Regularity here means the [first variation](../../../../first-variation.md) of $J$ is not identically zero; abnormal constraint extrema otherwise need separate consideration.

If $H$ has no explicit $x$ dependence, then

$$
\frac d{dx}(y'H_{y'}-H)=y'\left(\frac d{dx}H_{y'}-H_y\right)=0.
$$

This is the [Beltrami identity](../../../../beltrami-identity.md), giving the required constant of integration.

For the chain, $ds=\sqrt{1+y'^2}\,dx$, so its fixed [arc length](../../../../arc-length.md) is exactly $J[y]=L$, and its gravitational [energy](../../../../energy-split.md) is $\rho g\int_{-a}^a y\sqrt{1+y'^2}\,dx$. The positive constant $\rho g$ can be suppressed in minimization. Use

$$
H=(y-\lambda)\sqrt{1+y'^2}.
$$

The equation, with a consistent sign convention for the multiplier, is

$$
\boxed{\sqrt{1+y'^2}-\frac d{dx}\left(\frac{(y-\lambda)y'}{\sqrt{1+y'^2}}\right)=0}.
$$

The first integral becomes $(y-\lambda)/\sqrt{1+y'^2}=c$. It implies $y''=(1+y'^2)/(y-\lambda)$; solving gives

$$
y=\lambda+c\cosh((x-x_0)/c).
$$

The equal endpoint heights force $x_0=0$, by evenness and strict increase of $\cosh$ on the positive half-line. Thus the extrema have the asserted [catenary](../../../../catenary.md) form. The length and height conditions give

$$
\boxed{L=2c\sinh(a/c),\qquad\lambda=b-c\cosh(a/c)}.
$$

For the hanging minimum choose $c>0$, the upward-convex branch lying below its endpoints. For $L>2a$ this positive $c$ is unique: writing $t=a/c$, the ratio $L/(2a)=\sinh(t)/t$ increases continuously from one to infinity. The negative-$c$ branch describes an upward arch, not the hanging minimum. If $L=2a$, only the horizontal straight chain is admissible and is the limiting degenerate case; $L<2a$ is impossible.

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
