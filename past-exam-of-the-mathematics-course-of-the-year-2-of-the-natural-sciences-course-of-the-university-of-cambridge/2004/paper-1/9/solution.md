<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

For variations $y+\epsilon\eta$ with $\eta(a)=\eta(b)=0$, [integration by parts](../../../../integration-by-parts.md) gives $\delta I=\int_a^b[f_y-d(f_{y'})/dx]\eta\,dx$. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md)

$$
\boxed{\frac d{dx}f_{y'}-f_y=0.}
$$

For the ramp, use [conservation of energy](../../../../conservation-of-energy.md) from rest at the rim. The vertical drop is $R\cos\theta$, so $v=\sqrt{2gR\cos\theta}$. The spherical surface [arc length](../../../../arc-length.md) is $ds=R\sqrt{d\theta^2+\sin^2\theta\,d\phi^2}$. On a monotone segment described by $\phi(\theta)$, the [travel time](../../../../travel-time.md) is consequently

$$
\boxed{T=\sqrt{\frac R{2g}}\int\sqrt{\frac{1+\sin^2\theta\,\phi'^2}{\cos\theta}}\,|d\theta|.}
$$

For increasing $\theta$ this has the printed limits $\theta_0$ to $\theta_1$; for a descent, reverse the decreasing angular limits to keep time positive. The azimuth is a [cyclic coordinate](../../../../cyclic-coordinate.md) of this integrand. Its conserved derivative gives the [first integral](../../../../first-integral.md) for the [brachistochrone on a hemispherical ramp](../../../../brachistochrone-on-a-hemispherical-ramp.md):

$$
\boxed{\frac{\sin^2\theta\,\phi'}{\sqrt{\cos\theta}\sqrt{1+\sin^2\theta\,\phi'^2}}=C.}
$$

Solving for its square yields

$$
\phi'^2=\frac{C^2\cos\theta}{\sin^2\theta(\sin^2\theta-C^2\cos\theta)}.
$$

For a regular stationary path with finite $C$, this tends to zero as the rim $\theta\to\pi/2$ is approached. The ratio of azimuthal to meridional displacements is $\sin\theta\,\phi'$, which also tends to zero. Hence **the initial direction is along a meridian toward the bottom**. This conclusion concerns the initial heading; the later route can turn before reaching the bottom when its rim endpoints require a nonzero azimuthal displacement.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
