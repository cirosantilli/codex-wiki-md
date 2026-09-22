<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $G=\Delta\rho g>0$ and take $\tau>0$ in the positive $x$ direction. Removing the ambient hydrostatic pressure leaves excess pressure $G(h-z)$, so the horizontal pressure gradient in the dense [gravity current](../../../../../gravity-current.md) is $G\nabla h$. The [lubrication approximation](../../../../../lubrication-theory.md) gives

$$
\mu u_{zz}=Gh_x,\qquad\mu v_{zz}=Gh_y.
$$

The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) at $z=0$ and the imposed upper [shear stress](../../../../../shear-stress.md) require $u(0)=v(0)=0$, $\mu u_z(h)=\tau$ and $\mu v_z(h)=0$. Integration yields

$$
u=\frac\tau\mu z+\frac G\mu h_x\left(\frac{z^2}2-hz\right),\qquad
v=\frac G\mu h_y\left(\frac{z^2}2-hz\right).
$$

Consequently the depth-integrated [volume flux](../../../../../volumetric-flow-rate.md) is

$$
\boldsymbol q=\frac{\tau h^2}{2\mu}e_x-\frac{Gh^3}{3\mu}\nabla h.
$$

Using [conservation of mass](../../../../../mass-conservation.md), $h_t+\nabla\cdot\boldsymbol q=0$, proves the **evolution equation** for a [shear-driven viscous gravity current](../../../../../shear-driven-viscous-gravity-current.md):

$$
\boxed{h_t+\frac\tau{2\mu}(h^2)_x=\frac G{3\mu}\nabla\cdot(h^3\nabla h).}
$$

The gravity term smooths thickness gradients, while the imposed shear transports the current downstream.

The approximations need more than a small ordinary [Reynolds number](../../../../../reynolds-number.md). With thickness $H$, horizontal scale $L$, dense-fluid density $\rho_c=\rho+\Delta\rho$ and typical horizontal speed $V$, sufficient small parameters are

$$
\boxed{\frac HL\ll1,\qquad
\frac{\rho_cVH^2}{\mu L}\ll1,\qquad
\frac{\mu V}{GHL}\ll1.}
$$

The first neglects horizontal viscous derivatives relative to vertical ones. The second compares convective inertia with vertical viscous stress: it is the reduced [Reynolds number](../../../../../reynolds-number.md), $\operatorname{Re}_H(H/L)$, rather than a requirement that $\operatorname{Re}_H$ itself be small. The third keeps viscous normal stress small relative to the excess [hydrostatic pressure](../../../../../hydrostatic-pressure.md) $GH$. Here $V$ is of order $\tau H/\mu+GH^3/(\mu L)$, so this last condition requires $\tau/(GL)\ll1$ together with $(H/L)^2\ll1$. Explicit sufficient inertia conditions are $\rho_c\tau H^3/(\mu^2L)\ll1$ and $\rho_cGH^5/(\mu^2L^2)\ll1$. If an independently imposed unsteady time scale is $T$, also require $\rho_cH^2/(\mu T)\ll1$; for $T\sim L/V$ this is the same reduced-inertia condition.

Set $A=\tau/(2\mu)$ and $D=G/(3\mu)$. Far downstream, the transverse scale $Y=y_N$ is much smaller than $x$, so the downstream gravity-flux divergence is smaller than the transverse one by order $(Y/x)^2$. For the steady flow, away from the source,

$$
A(h^2)_x=D(h^3h_y)_y,\qquad Q=A\int_{-Y}^Yh^2dy.
$$

The latter expresses conservation of the prescribed point-source [volume flux](../../../../../volumetric-flow-rate.md). In scaling form, $Q\sim AH^2Y$ and $AH^2/x\sim DH^4/Y^2$. Eliminating $H$ gives $Y^3\sim DQx/A^2$, proving **$y_N\propto x^{1/3}$** and $H\propto x^{-1/6}$.

For the exact downstream [similarity solution](../../../../../similarity-solution.md), put $w=h^2$. Since $h^3h_y=(w^2)_y/4$, the reduced equation is the [porous medium equation](../../../../../porous-medium-equation.md)

$$
w_x=\frac D{4A}(w^2)_{yy}.
$$

Seek $w=x^{-1/3}F(\eta)$ with $\eta=y/x^{1/3}$. Substitution gives

$$
-\frac A3(F+\eta F')=\frac D4(F^2)''.
$$

Integrate once, using symmetry and zero transverse flux at $\eta=0$, to obtain $-A\eta F/3=DF F'/2$. Where $F>0$, this gives $F'=-2A\eta/(3D)$, hence $F=A(\eta_N^2-\eta^2)/(3D)$. Vanishing thickness fixes its support. The volume-flux condition then reads

$$
Q=\frac{A^2}{3Dx}\int_{-Y}^Y(Y^2-y^2)dy
=\frac{4A^2Y^3}{9Dx}.
$$

Thus the **downstream profile and half-width** are

$$
\boxed{\begin{aligned}
y_N(x)&=\left(\frac{3\mu\Delta\rho gQ}{\tau^2}x\right)^{1/3},\\
h(x,y)&=\left[\frac\tau{2\Delta\rho gx}\bigl(y_N(x)^2-y^2\bigr)\right]^{1/2}
\quad (|y|<y_N),
\end{aligned}}
$$

with $h=0$ outside that interval. This is the [downstream similarity of a shear-driven gravity current](../../../../../downstream-similarity-of-a-shear-driven-gravity-current.md). The square-root edge is the formal outer thin-layer solution; arbitrarily close to that edge its slope is not small, so the local front requires a separate description. This does not change the downstream scaling and flux calculation.

Near the source the two horizontal scales are comparable, say $\ell$, so the far-downstream reduction cannot locate the upstream nose. In the upstream direction the downstream shear flux $AH^2$ must balance the upstream gravity flux of order $DH^4/\ell$. Hence $\ell\sim(D/A)H^2$. The total discharge through a region of width $\ell$ is $Q\sim AH^2\ell$, giving $H^4\sim Q/D$. Combining these estimates gives the **upstream reach scale**

$$
\boxed{\ell_{\mathrm{up}}\ \text{is of order}\ \frac{\sqrt{\mu\Delta\rho gQ}}\tau.}
$$

The shear advects liquid toward positive $x$, while the hydrostatic thickness gradient drives liquid back toward negative $x$; their balance stops further upstream spreading. A numerical prefactor requires the full two-dimensional near-source free-boundary solution and cannot be fixed by these scaling arguments alone.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
