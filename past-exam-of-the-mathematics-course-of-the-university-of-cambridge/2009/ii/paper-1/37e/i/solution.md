<h1 id="37e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here $\ell\sim\sqrt{ab}$, so the geometric condition is $b/a\ll1$. Let $U$ be the signed roller velocity near its top, with magnitude $a|\Omega|$; choose the rotation sense making $U=a\Omega$ positive in the $x$ direction. The small-inertia condition is

$$
\frac{\rho U b^{3/2}}{\mu\sqrt a}\ll1
$$

with $|U|$ understood for a reversed rotation. The roller's slope and change of tangential speed are small in the gap region. The liquid is Newtonian, the roller imposes no slip and the free surface is shear-free; surface tension is neglected as in the gravity-only model.

For the leading flat film geometry, use $y=-d(x)$ as the roller boundary and $y=0$ as the free surface. The [lubrication approximation](../../../../../../lubrication-theory.md) gives $\mu u_{yy}=p_x$, $u(-d)=U$, $u_y(0)=0$, hence

$$
\boxed{u(x,y)=U+\frac{p_x}{2\mu}(y^2-d^2),\qquad
Q=Ud-\frac{d^3p_x}{3\mu}.}
$$

The corresponding vertical velocity is determined by incompressibility, for example $v(x,y)=\int_y^0u_x(x,s)\,ds$, so that $v(0)=0$ and $v(-d)=-Ud'$ by differentiating the constant-flux equation. This is the leading tangency condition at the roller. Steadiness makes $Q$ independent of $x$.

For the [rotating roller under a nearly flat free surface](../../../../../../rotating-roller-under-a-nearly-flat-free-surface.md), the excess pressure tends to zero in the outer fluid on both sides of the gap. Consequently

$$
0=\int_{-\infty}^{\infty}p_x\,dx
=3\mu\left[U\int d^{-2}dx-Q\int d^{-3}dx\right].
$$

Set $x=\sqrt{2ab}\,s$. The supplied recurrence gives $I_2=\pi/2$ and $I_3=3\pi/8$, so

$$
\boxed{Q=\frac43Ub=\frac43a\Omega b,\qquad
p_x=\frac{\mu U(3d-4b)}{d^3}
=\frac{\mu U}{b^2}\frac{3s^2-1}{(1+s^2)^3}.}
$$

The extension of the parabolic gap integrals to infinity is the usual matched thin-gap approximation; their dominant contribution comes from $x=O(\sqrt{ab})\ll a$. Taking the surface flat refers to this leading geometry, not setting its small hydrostatic displacement identically to zero in the pressure balance. An exactly flat stress-free surface at exactly constant pressure could not sustain this variable pressure gradient; the displacement needed to do so is checked in part (ii).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [37E](../../37e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
