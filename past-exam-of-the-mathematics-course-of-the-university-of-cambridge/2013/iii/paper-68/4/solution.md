<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take $\Delta\rho>0$ and $\tau>0$, with $x$ pointing along the imposed [shear stress](../../../../../shear-stress.md), and put $G=\Delta\rho g$. Relative to the upper fluid's hydrostatic reference, the [hydrostatic pressure](../../../../../hydrostatic-pressure.md) in the current is $p=G(h-z)$. Thus the horizontal [pressure gradient](../../../../../pressure-gradient.md) is $G\nabla h$. The [lubrication theory](../../../../../lubrication-theory.md) momentum balance, lower [no-slip boundary condition](../../../../../no-slip-boundary-condition.md), and imposed upper [shear stress](../../../../../shear-stress.md) give

$$
\mathbf u_{\parallel}(z)=-\frac{G}{2\mu}z(2h-z)\nabla h+\frac{\tau}{\mu}z\mathbf e_x.
$$

Its depth-integrated [volume flux](../../../../../volumetric-flow-rate.md) is

$$
\mathbf q=-\frac{G}{3\mu}h^3\nabla h+\frac{\tau}{2\mu}h^2\mathbf e_x.
$$

Define $D=G/(3\mu)$ and $A=\tau/(2\mu)$. The [continuity equation](../../../../../continuity-equation.md) gives the [shear-driven viscous gravity current](../../../../../shear-driven-viscous-gravity-current.md) equation

$$
\boxed{h_t+A\partial_x(h^2)=D\nabla\cdot(h^3\nabla h).}
$$

The two terms have opposite roles: imposed [shear stress](../../../../../shear-stress.md) carries fluid downstream, whereas the [hydrostatic pressure](../../../../../hydrostatic-pressure.md) gradient spreads it from thick regions towards thin ones.

For the approximation, a representative horizontal [velocity](../../../../../velocity.md) is $U\sim\tau H/\mu+GH^3/(\mu L)$, with vertical [velocity](../../../../../velocity.md) $UH/L$. Small slopes require $H/L\ll1$. Horizontal fluid inertia relative to vertical viscous resistance is $\rho_c UH^2/(\mu L)$, where $\rho_c=\rho+\Delta\rho$. Hence sufficient small parameters, expressed without an unknown [velocity](../../../../../velocity.md), are

$$
\boxed{\frac HL\ll1,\qquad
\frac{\rho_c\tau H^3}{\mu^2L}\ll1,\qquad
\frac{\rho_c GH^5}{\mu^2L^2}\ll1.}
$$

For the [hydrostatic pressure](../../../../../hydrostatic-pressure.md) and normal-stress approximation also require $\mu U/(GHL)\ll1$. Its gravity-driven part is already $(H/L)^2$; its shear-driven part adds

$$
\boxed{\frac{\tau}{GL}\ll1.}
$$

This condition controls viscous normal stress, vertical viscous corrections and the normal projection of shear at a slightly tilted interface relative to $GH$. With it and the previous inertia bounds, vertical inertia is small as well. Time variations here are on the transport timescale $L/U$; separately imposed rapid forcing would need its own unsteady inertia bound. A small ordinary [Reynolds number](../../../../../reynolds-number.md) is a stronger sufficient restriction, but the reduced inertia ratios above are what the thin-layer momentum balance directly requires.

In the steady far-downstream regime, cross-stream derivatives dominate gravity-driven spreading. Dropping the smaller downstream gravity flux leaves

$$
A(h^2)_x=D(h^3h_y)_y.
$$

Write $Y=y_N(x)$ and let $h_c$ be a typical central thickness. Balance gives $Y^2\sim(D/A)h_c^2x$, while conservation of the source [volume flux](../../../../../volumetric-flow-rate.md) gives $Q\sim Ah_c^2Y$. Therefore the [downstream similarity of a shear-driven gravity current](../../../../../downstream-similarity-of-a-shear-driven-gravity-current.md) has

$$
\boxed{Y\sim\left(\frac{DQx}{A^2}\right)^{1/3},\qquad h_c\propto x^{-1/6}.}
$$

The omitted downstream gravity flux relative to the imposed shear flux is $Dh_c^2/(Ax)\sim(Y/x)^2\ll1$, so this approximation is self-consistent in the stated regime.

For the full profile put $w=h^2$. Then $h^3h_y=(w^2)_y/4$ and

$$
w_x=\frac{D}{4A}(w^2)_{yy}.
$$

This is a [porous medium equation](../../../../../porous-medium-equation.md) with downstream distance as its evolution coordinate. Conservation of $\int w\,dy=Q/A$ and a [similarity solution](../../../../../similarity-solution.md) $w=x^{-1/3}f(\eta)$, $\eta=y/x^{1/3}$, give

$$
-\frac A3(f+\eta f')=\frac D4(f^2)'',\qquad
-\frac A3\eta f=\frac D2ff',
$$

where symmetry gives zero integration constant at $\eta=0$. Inside the positive region, $f'= -2A\eta/(3D)$, so $f=(A/(3D))(\eta_N^2-\eta^2)$. Requiring the total downstream [volume flux](../../../../../volumetric-flow-rate.md) to be $Q$ fixes the coefficient:

$$
Q=A\int_{-Y}^Yh^2\,dy=\frac{4A^2Y^3}{9Dx}.
$$

Consequently

$$
\boxed{y_N(x)=\left(\frac{3\mu\Delta\rho gQ}{\tau^2}x\right)^{1/3},\qquad
h(x,y)=\left[\frac{\tau}{2\Delta\rho gx}\bigl(y_N(x)^2-y^2\bigr)\right]^{1/2}}
$$

for $|y|<y_N$, with $h=0$ outside. The squared height is a parabolic [Barenblatt solution](../../../../../barenblatt-solution.md); the height cross-section is a semicircular profile after rescaling its axes. The cross-stream [volume flux](../../../../../volumetric-flow-rate.md) vanishes at the edges even though the height slope becomes singular there. The profile describes the outer [lubrication theory](../../../../../lubrication-theory.md) region, not a resolved microscopic front.

Near the point source the two horizontal dimensions are comparable, say $\ell$. Upstream spreading arrests where outward gravity-driven [volume flux](../../../../../volumetric-flow-rate.md) balances downstream shear-driven [volume flux](../../../../../volumetric-flow-rate.md):

$$
\frac{Dh_*^4}{\ell}\sim Ah_*^2,\qquad Q\sim Ah_*^2\ell.
$$

Eliminating $h_*$ gives

$$
\boxed{x_N\sim\frac{\sqrt{DQ}}A\sim\frac{\sqrt{\mu\Delta\rho gQ}}{\tau}.}
$$

This is a scaling estimate, not a determination of a numerical prefactor. The associated depth is $h_*\sim(\mu Q/(\Delta\rho g))^{1/4}$. The same horizontal scale is obtained by setting $y_N\sim x$ in the downstream [similarity solution](../../../../../similarity-solution.md), confirming where that solution fails.

For the line source the steady [volume flux per unit width](../../../../../volume-flux-per-unit-width.md) is $q=Ah^2-Dh^3h_x$. On the downstream constant-height branch, $q=Q_{2d}$ gives $h_d^2=Q_{2d}/A$. Upstream there is no net flux through the finite nose, so $q=0$. Thus $h h_x=A/D$, and continuity of height at the source gives

$$
h^2(x)=h_d^2+\frac{2A}{D}x=\frac{2\mu Q_{2d}}{\tau}+\frac{3\tau}{\Delta\rho g}x.
$$

The [line-source upstream reach under imposed shear](../../../../../line-source-upstream-reach-under-imposed-shear.md) is therefore

$$
\boxed{x_N=\frac{DQ_{2d}}{2A^2}=\frac{2\mu\Delta\rho gQ_{2d}}{3\tau^2},\qquad
h(x)=\begin{cases}
0,&x\leq-x_N,\\
\sqrt{\dfrac{3\tau}{\Delta\rho g}(x+x_N)},&-x_N<x<0,\\
\sqrt{\dfrac{2\mu Q_{2d}}\tau},&x>0.
\end{cases}}
$$

In the upstream part, shear-driven and gravity-driven [volume fluxes](../../../../../volumetric-flow-rate.md) cancel. The [volume flux per unit width](../../../../../volume-flux-per-unit-width.md) jumps by exactly $Q_{2d}$ at the source. As in the point-source profile, the square-root nose is a formal outer solution with an unresolved steep front; its finite upstream reach follows from flux balance, not from assuming a small slope all the way to the nose.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
