<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $x^\mu(\tau)$ denote the spacetime coordinates, with dots meaning differentiation with respect to an [affine parameter](../../../../affine-parameter.md); for a massive particle take [proper time](../../../../proper-time.md) $\tau$. The [metric tensor](../../../../metric-tensor.md) determines the quadratic [geodesic Lagrangian](../../../../geodesic-lagrangian.md) $L=g_{\mu\nu}\dot x^\mu\dot x^\nu$. The [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
\frac d{d\tau}\frac{\partial L}{\partial\dot x^\mu}-\frac{\partial L}{\partial x^\mu}=0.
$$

Symmetry of the [metric tensor](../../../../metric-tensor.md) gives $\partial L/\partial\dot x^\mu=2g_{\mu\nu}\dot x^\nu$. Hence the covariant [four-momentum](../../../../four-momentum.md) is $p_\mu=mg_{\mu\nu}\dot x^\nu=(m/2)\partial L/\partial\dot x^\mu$. If $x^\mu$ is a [cyclic coordinate](../../../../cyclic-coordinate.md), its [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) immediately gives $\dot p_\mu=0$.

For the rotating metric, $t,\phi,z$ are all cyclic. Thus

$$
\boxed{\begin{aligned}
p_t&=m[(c^2-\omega^2r^2)\dot t-\omega r^2\dot\phi],\\
p_\phi&=-mr^2(\dot\phi+\omega\dot t),\qquad p_z=-m\dot z.
\end{aligned}}
$$

Combining the first two equations cancels their $r$ dependence:

$$
\boxed{\dot t=\frac{p_t-\omega p_\phi}{mc^2}=\mathrm{constant}.}
$$

The radial [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is $-2\ddot r=-2r(\dot\phi+\omega\dot t)^2$, so

$$
\boxed{\ddot r=r(\dot\phi+\omega\dot t)^2=\frac{p_\phi^2}{m^2r^3}.}
$$

This is the [geodesic equation in a uniformly rotating Minkowski chart](../../../../geodesic-equation-in-a-uniformly-rotating-minkowski-chart.md). With inertial angle $\Phi=\phi+\omega t$, $-p_\phi$ is the inertial axial [angular momentum](../../../../angular-momentum.md). The outward radial-coordinate acceleration expresses the familiar centrifugal term associated with angular motion: the underlying free trajectory is a straight line in [Minkowski spacetime](../../../../minkowski-spacetime.md). It does not imply an external radial force. Holding a particle at rest in the [rotating reference frame](../../../../rotating-reference-frame.md) instead requires a real inward force.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
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
