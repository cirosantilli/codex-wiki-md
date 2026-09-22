<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The flat plate moves tangentially and the curved plate is stationary. The [no-slip boundary condition](../../../../no-slip-boundary-condition.md) and [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md) give

$$
\boxed{u=-U,\quad w=0\quad(z=0),\qquad
u=0,\quad w=0\quad(z=h(x)).}
$$

At the curved plate, impermeability can also be written $w=u h_x$; together with zero tangential [velocity](../../../../velocity.md), this gives both components zero. The native PDF writes $v'=0$ in the scaled wall conditions although the normal component is defined as $w'$. We use $w'$ consistently.

The [parabolic lubrication gap](../../../../parabolic-lubrication-gap.md) changes by order $h_0$ when $x^2/R$ is order $h_0$. Its natural horizontal scale is therefore

$$
\boxed{L=\sqrt{Rh_0},\qquad \delta=\frac{h_0}{L}=\sqrt{\frac{h_0}{R}}\ll1.}
$$

The proposed normal [velocity](../../../../velocity.md) scale $h_0U/L$ then makes the two terms of the [continuity equation](../../../../continuity-equation.md) comparable. Balancing the horizontal [pressure gradient](../../../../pressure-gradient.md) against the transverse viscous term in the [Navier-Stokes equation](../../../../navier-stokes-equation.md) requires $P/L=\mu U/h_0^2$, so

$$
\boxed{P=\frac{\mu UL}{h_0^2}.}
$$

Here [pressure](../../../../pressure-split.md) is measured from a common reference value, which is chosen at the outer fluid in part (b).

For clarity, define the dimensionless [material derivative](../../../../material-derivative.md)

$$
\mathcal D'=\partial_{t'}+u'\partial_{x'}+w'\partial_{z'},
\qquad \mathrm{Re}=\frac{\rho LU}{\mu}.
$$

Substitution of all the scalings gives the exact dimensionless equations

$$
\begin{aligned}
u'_{x'}+w'_{z'}&=0,\\
\delta^2\mathrm{Re}\,\mathcal D'u'&=-p'_{x'}+u'_{z'z'}+\delta^2u'_{x'x'},\\
\delta^4\mathrm{Re}\,\mathcal D'w'&=-p'_{z'}+\delta^2w'_{z'z'}+\delta^4w'_{x'x'}.
\end{aligned}
$$

For example, the factor in the last left side is obtained by dividing the vertical [acceleration](../../../../acceleration.md) scale $\rho h_0U^2/L^2$ by the vertical [pressure gradient](../../../../pressure-gradient.md) scale $P/h_0$.

Taking $\delta\ll1$ and $\delta^2\mathrm{Re}\ll1$ leaves the [lubrication approximation](../../../../lubrication-theory.md)

$$
\boxed{u'_{x'}+w'_{z'}=0,\qquad
0=-p'_{x'}+u'_{z'z'},\qquad 0=-p'_{z'}.}
$$

The scaled gap and [boundary conditions](../../../../boundary-condition.md) are

$$
\boxed{h'(x')=1+\frac{x'^2}{2},\qquad
(u',w')=(-1,0)\ (z'=0),\qquad
(u',w')=(0,0)\ (z'=h'(x')).}
$$

The [Reynolds number](../../../../reynolds-number.md) itself need not be small: it is $\delta^2\mathrm{Re}$ that measures inertia relative to transverse viscous resistance in this thin geometry.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the viscous flow course of the University of Oxford](../../../split.md)
5. [Viscous flow course of the University of Oxford](../../../../viscous-flow-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
