<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [pressure](../../../../../pressure.md) scale $\rho\widehat U^2$, and denote the scaled transverse [velocity](../../../../../velocity.md) by $v$. The steady [incompressible flow](../../../../../incompressible-flow.md) equations under the prescribed coordinate scaling are

$$
\begin{aligned}
u_x+v_y&=0,\\
uu_x+vu_y&=-p_x+\frac\lambda R\left(u_{yy}+\lambda^{-2}u_{xx}\right),\\
\lambda^{-2}(uv_x+vv_y)&=-p_y+\frac1{\lambda R}\left(v_{yy}+\lambda^{-2}v_{xx}\right).
\end{aligned}
$$

The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) is $u=v=0$ at $y=1$ and at the lower wall $y=\epsilon F(x)$, taking $F=0$ upstream. Far upstream, $u\to U_0=6y(1-y)$, $v\to0$, and $p_x\to-12\lambda/R$. These are the dimensional [Navier-Stokes equations](../../../../../navier-stokes-equation.md) divided by the streamwise and transverse inertial scales, respectively; the transverse equation's $\lambda^{-2}$ is essential.

A consistent nonlinear wall-layer regime can be chosen as

$$
\boxed{\frac\lambda R=\epsilon^3,\qquad R^{1/7}\ll\lambda\ll R,\qquad\epsilon\ll1.}
$$

Near a wall the oncoming [plane Poiseuille flow](../../../../../plane-poiseuille-flow.md) is linear in distance, so a layer of thickness $\epsilon$ has $u=O(\epsilon)$ and $v=O(\epsilon^2)$. Its inertia is $O(\epsilon^2)$; its transverse viscous term is $(\lambda/R)O(\epsilon^{-1})=O(\epsilon^2)$, explaining the distinguished balance. The resulting [pressure](../../../../../pressure.md) perturbation is $O(\epsilon^2)$. In the core the induced transverse [pressure](../../../../../pressure.md) variation is $O(\epsilon/\lambda^2)$, negligible compared with that [pressure](../../../../../pressure.md) perturbation when $\lambda^2\epsilon\gg1$, equivalently $\lambda\gg R^{1/7}$. Also $\lambda\ll R$ makes both the indentation and the [viscous boundary layer](../../../../../viscous-boundary-layer.md) thin. Streamwise viscous derivatives are smaller still. Thus the core perturbation is inviscid at first order and [pressure](../../../../../pressure.md) is common to the two wall layers at their leading order.

Write $u=U_0+\epsilon u_1+\cdots$ and $v=\epsilon v_1+\cdots$. The core [pressure gradient](../../../../../pressure-gradient.md) only enters at order $\epsilon^2$, so first-order [continuity equation](../../../../../continuity-equation.md) and streamwise momentum give

$$
u_{1x}+v_{1y}=0,\qquad U_0u_{1x}+U'_0v_1=0.
$$

Eliminating $u_{1x}$ shows $(v_1/U_0)_y=0$. Let that ratio be $-A'(x)$; integration in $x$, with the unperturbed upstream condition, then gives

$$
\boxed{u=U_0(y)+\epsilon A(x)U'_0(y)+O(\epsilon^2),\qquad
v=-\epsilon A'(x)U_0(y)+O(\epsilon^2).}
$$

This displacement form automatically has zero first-order change in total core flux, because $\int_0^1 U'_0\,dy=0$.

For the lower [boundary layer](../../../../../boundary-layer.md), use

$$
y=\epsilon[z+F(x)],\quad u=\epsilon U(x,z),\quad
v=\epsilon^2[V(x,z)+F'(x)U(x,z)],\quad p=p_0(x)+\epsilon^2P(x),
$$

where $p'_0=-12\epsilon^3$ is the smaller upstream [pressure gradient](../../../../../pressure-gradient.md). The extra term in $v$ removes the [velocity](../../../../../velocity.md) induced by the moving coordinate surface. The chain rule gives $\partial_x|_y=\partial_x|_z-F'\partial_z$ and $\partial_y=\epsilon^{-1}\partial_z$; the wall-slope terms cancel from both [continuity equation](../../../../../continuity-equation.md) and convection. At leading order the [Prandtl boundary-layer equation](../../../../../prandtl-boundary-layer-equation.md) is

$$
\boxed{U_x+V_z=0,\qquad UU_x+VU_z=-P'(x)+U_{zz},\qquad U=V=0\text{ at }z=0.}
$$

Matching to the core near the lower wall gives $U\sim6[z+F+A]$, so $H_{\rm lower}=F+A$.

For the upper [boundary layer](../../../../../boundary-layer.md), set $y=1-\epsilon z$, $u=\epsilon U$, $v=-\epsilon^2V$. The same equations, wall data and common $P(x)$ result, but the core matching gives $U\sim6[z-A]$, so $H_{\rm upper}=-A$. The two [pressure](../../../../../pressure.md)-driven wall-layer problems have the same upstream shear, wall conditions and [pressure](../../../../../pressure.md) forcing. Under the question's uniqueness assumption their solutions coincide, and their displacement limits must coincide. Thus the [symmetric viscous interaction in an indented Poiseuille channel](../../../../../symmetric-viscous-interaction-in-an-indented-poiseuille-channel.md) gives

$$
F+A=-A,\qquad \boxed{A=-F/2,\qquad H_{\rm lower}=H_{\rm upper}=F/2.}
$$

For $F=bx^{1/3}$, one has $A=-(b/2)x^{1/3}$ and $H=(b/2)x^{1/3}$. Matching $U\sim6[z+H(x)]$ in a [similarity solution](../../../../../similarity-solution.md) $U=x^\beta G'(zx^{-\gamma})$ requires $\beta=\gamma=1/3$. Equating the powers in convection $x^{2\beta-1}$, viscosity $x^{\beta-2\gamma}$ and [pressure gradient](../../../../../pressure-gradient.md) $x^{\sigma-1}$ gives $\sigma=2/3$. Hence

$$
\boxed{\alpha=\beta=\gamma=\frac13,\qquad\sigma=\frac23,\qquad\bar a=-b/2.}
$$

Use the [stream function](../../../../../stream-function.md) $\psi=x^{2/3}G(\eta)$, with $\eta=zx^{-1/3}$. Then

$$
U=x^{1/3}G',\qquad V=-x^{-1/3}\left(\frac23G-\frac13\eta G'\right).
$$

Direct differentiation gives $UU_x+VU_z=x^{-1/3}[(G')^2/3-2GG''/3]$, whereas $-P'+U_{zz}=x^{-1/3}[-2\bar p/3+G''']$. The [one-third-power similarity of an indented channel boundary layer](../../../../../one-third-power-similarity-of-an-indented-channel-boundary-layer.md) is therefore governed by

$$
\boxed{G'''+\frac23GG''-\frac13(G')^2=\frac23\bar p,\qquad
G(0)=G'(0)=0,\qquad G'(\eta)\sim6\eta+3b.}
$$

The original PDF has $(G')^2$ in this equation; the converted TeX loses the derivative and gives $G^2$. Existence remains conditional on a value of $\bar p$ for which this [boundary value problem](../../../../../boundary-value-problem.md) has a solution, as stipulated in the question. The similarity describes the stated thin-indentation regime on $x>0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
