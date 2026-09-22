<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

The [flatness problem](../../../../../flatness-problem.md) is that the observed [cosmological density parameter](../../../../../cosmological-density-parameter.md) is close to $\Omega=1$, although in an ordinary decelerating universe any departure from one grows with time. Extrapolation backward therefore requires implausibly precise early cancellation of the curvature term.

The [cosmological perfect-fluid continuity equation](../../../../../cosmological-perfect-fluid-continuity-equation.md) is

$$
\dot\rho+3H(\rho+P)=0.
$$

Consequently

$$
\frac d{dt}(\rho a^2)
=a^2\dot\rho+2a\dot a\rho
=-Ha^2(\rho+3P).
$$

For an expanding universe $H>0$. If

$$
\rho+3P<0,
$$

then $\rho a^2$ increases. The [Friedmann equation](../../../../../friedmann-equations.md) implies

$$
\left|\Omega^{-1}-1\right|
=\frac{\text{constant}\times |k|}{\rho a^2}.
$$

It therefore decreases during this period, driving $\Omega$ toward one. By the [Friedmann acceleration equation](../../../../../friedmann-acceleration-equation.md), the same condition gives $\ddot a>0$ when the cosmological constant is included in the effective fluid. This is the [inflationary solution of the flatness problem](../../../../../inflationary-solution-of-the-flatness-problem.md).

For the scalar field, the [slow-roll approximation](../../../../../slow-roll-approximation.md) means

$$
\dot\phi^2\ll V(\phi),
\qquad
|\ddot\phi|\ll3H|\dot\phi|.
$$

The equations reduce to

$$
3H^2\simeq m^2\phi^2,
\qquad
3H\dot\phi\simeq-2m^2\phi.
$$

Taking the positive-field branch gives $H\simeq m\phi/\sqrt3$, and therefore

$$
\dot\phi\simeq-\frac{2m}{\sqrt3}.
$$

With $\phi(0)=\phi_i$,

$$
\boxed{\phi(t)=\phi_i-\frac{2m}{\sqrt3}t.}
$$

Now integrate $H=\dot a/a\simeq m\phi/\sqrt3$:

$$
\log\frac{a(t)}{a_i}
=\int_0^t\frac m{\sqrt3}
\left(\phi_i-\frac{2m}{\sqrt3}s\right)ds
=\frac{m\phi_i}{\sqrt3}t-\frac{m^2t^2}{3}.
$$

Thus the [quadratic-potential slow-roll solution](../../../../../quadratic-potential-slow-roll-solution.md) is

$$
\boxed{
a(t)=a_i\exp\left[
\frac{m\phi_i}{\sqrt3}t-\frac{m^2t^2}{3}
\right].}
$$

Finally,

$$
\phi_i^2-\phi(t)^2
=\frac{4m\phi_i}{\sqrt3}t-\frac{4m^2}{3}t^2,
$$

so equivalently

$$
\boxed{
a(t)=a_i\exp\left[
\frac{\phi_i^2-\phi(t)^2}{4}
\right].}
$$

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
