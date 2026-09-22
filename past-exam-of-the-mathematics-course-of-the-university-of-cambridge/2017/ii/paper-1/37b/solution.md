<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

The unit normal pointing out of the fluid at its lower boundary is $-\mathbf e_y$. Since impermeability gives $v(x,0)=0$, also $v_x(x,0)=0$, and the tangential viscous traction exerted on the fluid is $t_x=-\mu u_y(x,0)$. The cilia do positive work at rate $t_xu=\rho P$, so

$$
\boxed{u\,u_y\big|_{y=0}=-\rho P/\mu=-P/\nu}.
$$

For positive downstream velocity this requires $u_y<0$, as expected when the wall-driven flow slows away from the cilia. The wall velocity is not prescribed independently; the driving condition prescribes power.

In a laminar [boundary layer](../../../../../boundary-layer.md), momentum diffuses over a thickness $\delta$ during the downstream advection time $x/U$, giving $\delta^2\sim\nu x/U$. The wall power condition gives $U^2/\delta\sim P/\nu$. With these balances the downstream Reynolds number grows and $\delta/x\propto x^{-3/5}$ tends to zero. This explains the thin layer for large $x$ within the laminar approximation. Pressure is uniform across it and has no imposed streamwise [gradient](../../../../../gradient.md) because the outer fluid is at rest. The [two-dimensional boundary-layer equations](../../../../../two-dimensional-boundary-layer-equations.md) are

$$
u u_x+v u_y=\nu u_{yy},\qquad u_x+v_y=0.
$$

Choose the scales to satisfy the balances exactly:

$$
\boxed{U(x)=\left(\frac{P^2x}{\nu}\right)^{1/5},\qquad
\delta(x)=\left(\frac{\nu^3x^2}{P}\right)^{1/5}}.
$$

The [stream function](../../../../../stream-function.md) $\psi=U\delta f(\eta)$, $\eta=y/\delta$, enforces [continuity equation](../../../../../continuity-equation.md) and gives

$$
u=U f',\qquad v=\frac{U\delta}{5x}(2\eta f'-3f),\qquad
u_x=\frac U{5x}(f'-2\eta f'').
$$

Thus the advective term is $U^2[\tfrac15f'^2-\tfrac35ff'']/x$, while $\nu u_{yy}=\nu U f'''/\delta^2=U^2f'''/x$. Hence

$$
\boxed{f'''=\tfrac15f'^2-\tfrac35ff''}.
$$

Impermeability, imposed wall power and matching to resting outer fluid give

$$
\boxed{f(0)=0,\qquad f'(0)f''(0)=-1,\qquad f'(\eta)\to0\quad(\eta\to\infty)}.
$$

A regular decaying profile also has $f''\to0$ and finite positive $f_\infty$; no arbitrary additional wall value for $f'$ should be imposed.

The volume flux per unit span is $Q=\int_0^\infty u\,dy=U\delta f_\infty\propto x^{3/5}$, so [continuity equation](../../../../../continuity-equation.md) gives $v_\infty=-dQ/dx<0$: outer fluid is entrained toward the wall. In the physical positive decaying similarity profile, $f'>0$ and $f''<0$. To justify monotonicity, $f''(0)<0$ by the power condition; if $f''$ first crossed zero with $f'>0$, the equation would give $f'''=f'^2/5>0$, after which $f''>0$ cannot cross back and $f'$ could not decay to zero. Therefore $f(\eta)=\int_0^\eta f'(s)ds\ge\eta f'(\eta)$, and the velocity formula gives $2\eta f'-3f<0$ for $\eta>0$. Consequently **the transverse velocity is negative throughout that physical layer, and zero at the wall**. This pointwise conclusion uses the positive decaying branch; the flux argument already establishes [entrainment](../../../../../fluid-entrainment.md) of the exterior.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
