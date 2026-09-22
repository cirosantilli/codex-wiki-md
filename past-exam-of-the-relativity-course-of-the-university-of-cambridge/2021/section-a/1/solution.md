<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $\alpha>0$, $t\ne0$, and the negative-norm convention for a [timelike curve](../../../../timelike-curve.md) used by the printed metric. Writing $v=dx/dt$ and $ds^2=-c^2d\tau^2$ gives

$$
\frac{d\tau}{dt}=\frac{|t|}{\sqrt\alpha}\sqrt{1-\frac{v^2}{c^2}}.
$$

Spatial translation is a [Killing vector field](../../../../killing-vector-field-split.md). Equivalently, the [geodesic Lagrangian](../../../../geodesic-lagrangian.md) has the [cyclic coordinate](../../../../cyclic-coordinate.md) $x$, so its conserved momentum is

$$
P=\frac{t^2}{\alpha}\frac{dx}{d\tau}
=\frac{|t|}{\sqrt\alpha}\frac{v}{\sqrt{1-v^2/c^2}}.
$$

Therefore the correct [first integral](../../../../first-integral.md) for this metric is

$$
\boxed{\frac{|t|\,v}{\sqrt{1-v^2/c^2}}=\text{constant}.}
$$

**The first-integral assertion in the PDF is false.** Its dimensionless square root requires $v/c$, and even after setting $c=1$ it is missing the factor $|t|$. For example, the nonvertical geodesics below have $v/\sqrt{1-v^2/c^2}$ proportional to $1/|t|$.

Set $b=\sqrt\alpha P/c$. Solving for the velocity, with increasing $t$ as the time orientation, gives $v=cb/\sqrt{t^2+b^2}$. The complete unparametrized family of [timelike geodesics of a quadratic-time conformal metric](../../../../timelike-geodesics-of-a-quadratic-time-conformal-metric.md) is

$$
\boxed{x(t)=x_c+cb\,\operatorname{arsinh}\!\left(\frac{t}{|b|}\right)\quad(b\ne0),\qquad
x(t)=x_c\quad(b=0).}
$$

Each curve is restricted to a connected positive- or negative-$t$ patch; $t=0$ is excluded because the metric becomes degenerate. For $t\ne0$, $|v|<c$, and the two independent constants are $x_c$ and $b$. If an explicit affine parametrization is desired,

$$
\tau-\tau_c=\frac{t\sqrt{t^2+b^2}-b^2\operatorname{arsinh}(t/|b|)}{2\sqrt\alpha}\quad(b\ne0),
$$

while the vertical family has $d\tau=|t|dt/\sqrt\alpha$. A reversal of the time orientation reverses the parameter without changing these paths.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
