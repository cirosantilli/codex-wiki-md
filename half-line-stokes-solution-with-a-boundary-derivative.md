# Half-line Stokes solution with a boundary derivative

↑ **Parent:** [Stokes resolvent kernel with advection](stokes-resolvent-kernel-with-advection.md)

For the [linear dispersive Stokes equation](linear-dispersive-stokes-equation.md) on $x>0$, with sufficiently smooth decaying initial data and $\operatorname{Re}p>0$, define $V(x,p)=\int_0^\infty R_p(x-y)u_0(y)\,dy$ and let $G(p)$ be the time [Laplace transform](laplace-transform.md) of the prescribed derivative $u_x(0,t)$. Spatial decay and the one-dimensional decaying homogeneous space give

$$
U(x,p)=V(x,p)+\frac{e^{r_-x}}{r_-}\bigl[G(p)-V_x(0,p)\bigr].
$$

The [Neumann boundary condition](neumann-boundary-condition.md) follows by differentiating at zero. The initial forcing follows from the [Stokes resolvent kernel with advection](stokes-resolvent-kernel-with-advection.md). The [Bromwich inversion formula](bromwich-inversion-formula.md) gives an [integral representation](integral-representation.md) with no unknown boundary traces. Truncating or extending the prescribed boundary signal beyond a target time does not affect earlier values, by the [Laplace transform time-shift rule](laplace-transform-time-shift-rule.md) and causality of this [Green function](green-s-function.md).

## ↑ Ancestors (9)

1. [Stokes resolvent kernel with advection](stokes-resolvent-kernel-with-advection.md)
2. [Spatial root splitting for the dispersive Stokes resolvent](spatial-root-splitting-for-the-dispersive-stokes-resolvent.md)
3. [Linear dispersive Stokes equation](linear-dispersive-stokes-equation.md)
4. [Airy equation](airy-equation.md)
5. [Lax pair](lax-pair.md)
6. [Integrable systems](integrable-systems-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/1/solution.md)
