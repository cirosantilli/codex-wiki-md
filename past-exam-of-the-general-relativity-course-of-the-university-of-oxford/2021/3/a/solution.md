<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The intended orbit is a freely falling [timelike circular Schwarzschild geodesic](../../../../timelike-circular-schwarzschild-geodesic.md). Use the [Schwarzschild metric](../../../../schwarzschild-spacetime-split.md) with $t$ rather than $ct$ as the zeroth coordinate, and put the orbit at $\theta=\pi/2$. Thus $g_{tt}=-fc^2$, $g_{rr}=1/f$, $g_{\phi\phi}=r^2$, with $f=1-2GM/(rc^2)$. The radial [geodesic equation](../../../../geodesic-equation.md) at constant $r$ is

$$
\Gamma^r_{tt}(u^t)^2+\Gamma^r_{\phi\phi}(u^\phi)^2=0,
\qquad \Gamma^r_{tt}=\frac{GMf}{r^2},\qquad \Gamma^r_{\phi\phi}=-rf.
$$

Consequently $\Omega^2=(u^\phi/u^t)^2=GM/r^3$. The [four-velocity](../../../../four-velocity.md) normalization gives

$$
-c^2=-fc^2(u^t)^2+r^2\Omega^2(u^t)^2
=-c^2\left(1-\frac{3GM}{rc^2}\right)(u^t)^2,
$$

and hence

$$
\boxed{u^0=u^t=\frac{dt}{d\tau}=\left(1-\frac{3GM}{rc^2}\right)^{-1/2}.}
$$

Here $t$ is [Schwarzschild time](../../../../schwarzschild-time.md), $\tau$ the orbiting clock's [proper time](../../../../proper-time.md), $G$ the [gravitational constant](../../../../gravitational-constant.md), $M$ the central [mass](../../../../mass.md), $r$ the constant [areal radius](../../../../areal-radius.md), and $c$ the [speed of light](../../../../speed-of-light.md). The dimensionless $u^0$ follows the question's time-valued zeroth-coordinate convention; with $x^0=ct$ the zeroth [four-velocity](../../../../four-velocity.md) component would be $c\,dt/d\tau$.

The condition is $r>3GM/c^2$ for a massive circular [geodesic](../../../../geodesic.md); radial stability further requires $r>6GM/c^2$, with equality marginal. The phrase “any circular orbit” is false without free fall: a powered circular trajectory has $dt/d\tau=[f-r^2\Omega^2/c^2]^{-1/2}$ with independently chosen $\Omega$. For example, at $r=10GM/c^2$ choose $\Omega=\tfrac12\sqrt{GM/r^3}$; this valid accelerated circular trajectory has $dt/d\tau=\sqrt{40/31}$, instead of the displayed $\sqrt{10/7}$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
