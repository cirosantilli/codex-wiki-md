<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Take a variation $y_\varepsilon=y+\varepsilon\eta$ with $\eta(a)=\eta(b)=0$. Differentiating the [functional](../../../../functional.md) at zero and using [integration by parts](../../../../integration-by-parts.md) gives

$$
\delta F=\int_b^a(f_y\eta+f_{y'}\eta')dx=\left[f_{y'}\eta\right]_b^a+\int_b^a\left(f_y-\frac d{dx}f_{y'}\right)\eta\,dx.
$$

The boundary term vanishes. Since the remaining [integral](../../../../integral-split.md) must vanish for every smooth endpoint-zero variation, the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) $d(f_{y'})/dx=f_y$.

For the mechanical problem put $A(r)=1-2m/r>0$. The [Lagrangian](../../../../lagrangian.md) is independent of $\theta$, a [cyclic coordinate](../../../../cyclic-coordinate.md), so its [conjugate momentum](../../../../canonical-momentum.md) $\partial L/\partial\dot\theta=2r^2\dot\theta=2J$ is conserved. Therefore $J$ is constant, including the factor of two between $J$ and the canonical momentum for this normalization of $L$.

For the radial coordinate, $\partial L/\partial\dot r=2\dot r/A$ and $\partial L/\partial r=-\dot r^2A'/A^2+2r\dot\theta^2-\mu A'/A^2$. Its [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
\frac{2\ddot r}{A}-\frac{A'\dot r^2}{A^2}-2r\dot\theta^2+\frac{\mu A'}{A^2}=0.
$$

For a [circular orbit](../../../../circular-orbit.md) $r=R>2m$, the radial [velocity](../../../../velocity.md) and [acceleration](../../../../acceleration.md) vanish. Using $A'(R)=2m/R^2$ and $\dot\theta=J/R^2$ leaves $2J^2/R^3=2m\mu/[R^2A(R)^2]$, hence

$$
\boxed{J^2=\frac{m\mu R}{(1-2m/R)^2}.}
$$

This is the [circular orbit condition for a radial kinetic Lagrangian](../../../../circular-orbit-condition-for-a-radial-kinetic-lagrangian.md) applied to the coefficients here.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
