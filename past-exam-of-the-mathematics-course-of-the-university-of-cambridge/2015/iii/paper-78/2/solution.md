<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose $x=0$ at the contact line, with $x>0$ pointing into the mountains and the plate moving in the positive $x$ direction at speed $U>0$. Let $z=0$ be the plate. For [viscous mountain spreading over an underthrust plate](../../../../../viscous-mountain-spreading-over-an-underthrust-plate.md), the [lubrication approximation](../../../../../lubrication-theory.md) assumes slow horizontal variation, [hydrostatic pressure](../../../../../hydrostatic-pressure.md) $p=\rho g(h-z)$, and $\mu u_{zz}=p_x=\rho gh_x\equiv G$. Impose no slip at the plate and zero tangential traction at the free surface. Without sediment,

$$
\boxed{u(z)=U+\frac{G}{2\mu}(z^2-2hz),\qquad q=\int_0^hu\,dz=Uh-\frac{\rho g}{3\mu}h^3h_x.}
$$

The horizontal [mass flux](../../../../../mass-flux.md) is $\rho q$. For a steady mountain range with no mountain material entering across its contact line, $q=0$. Therefore $h_x=3\mu U/(\rho gh^2)$, and the vanishing height at the bare contact gives **the mountain profile**

$$
\boxed{h(x)=\left(\frac{9\mu U}{\rho g}x\right)^{1/3},\qquad x\geq0.}
$$

The large slope extremely close to $x=0$ is an inner region where the [lubrication approximation](../../../../../lubrication-theory.md) ceases to be quantitatively valid.

Now let sediment occupy $0<z<d$ and mountains $d<z<h$, with $H=h-d$ the mountain-material thickness and $M=\mu_s/\mu$. Equal densities make $G=\rho gh_x$ the same in both layers. Continuity of [velocity](../../../../../velocity.md) and shear stress at $z=d$, no slip at $z=0$ and zero shear at $z=h$ give the shear stress $G(z-h)$ throughout. Thus **the two [velocity](../../../../../velocity.md) profiles** are

$$
u_s(z)=U+\frac G{\mu_s}\left(\frac{z^2}2-hz\right),\quad 0\leq z\leq d,
$$



$$
u_m(d+\zeta)=U-\frac G{\mu_s}\left(dH+\frac{d^2}2\right)+\frac G\mu\left(\frac{\zeta^2}2-H\zeta\right),\quad0\leq\zeta\leq H.
$$

Their volume fluxes are

$$
q_s=Ud-\frac{G}{\mu_s}\left(\frac{d^2H}2+\frac{d^3}3\right),\qquad
q_m=UH-\frac{G}{\mu_s}\left(dH^2+\frac{d^2H}2\right)-\frac{G H^3}{3\mu}.
$$

Multiplying by $\rho$ gives the separate mass fluxes. The coupled [conservation of mass](../../../../../mass-conservation.md) equations are

$$
\boxed{\partial_td+\partial_xq_s=0,\qquad\partial_tH+\partial_xq_m=0,\qquad h=d+H.}
$$

This is the [sediment-lubricated viscous mountain model](../../../../../sediment-lubricated-viscous-mountain-model.md). It includes shear-driven transport by the plate and [pressure](../../../../../pressure.md)-driven gravitational spreading.

In steady state the mountain-material flux is zero, while the upstream uniform sediment layer has $q_s=Ud_\infty$. For $H>0$ this gives

$$
U=G\left[\frac{dH+d^2/2}{\mu_s}+\frac{H^2}{3\mu}\right],\qquad
G=\frac{\mu_sU(d-d_\infty)}{d^2H/2+d^3/3}.
$$

Eliminating $G$ proves **the algebraic thickness relation**:

$$
\boxed{H^2+\frac{3d}{2M}\left(2-\frac d{d-d_\infty}\right)H+\frac{d^2}M\left(\frac32-\frac d{d-d_\infty}\right)=0.}
$$

At the contact $H\to0^+$, the last coefficient must vanish. The nonzero physical solution is consequently

$$
\boxed{h(0)=d(0)=3d_\infty.}
$$

The condition comes from the limiting zero flux per unit mountain thickness, not merely the automatic vanishing of $q_m$ at $H=0$. The surface slope anywhere under the mountains is

$$
\boxed{h_x=\frac{3\mu U}{\rho g\left[H^2+3dH/M+3d^2/(2M)\right]},\qquad
h_x(0)=\frac{2\mu_sU}{9\rho g d_\infty^2}=\frac{2M\mu U}{9\rho g d_\infty^2}.}
$$

**Lower sediment [viscosity](../../../../../dynamic-viscosity.md) flattens the near-contact surface**, while its contact height remains $3d_\infty$. Far inside, where $H\gg d/M$, the mountains recover the bare-layer slope scaling. The formulas determine the mountain profile by the algebraic relation plus this first-order equation. For example, put $\delta=d/d_\infty$ and $w=H/d$; the physical root satisfies $2M(\delta-1)w^2+3(\delta-2)w+\delta-3=0$, taking $w\geq0$ for $1<\delta\leq3$. This selects the branch smoothly connected to the contact.

In front of the contact, $x<0$, there is only sediment, so $h=d$ and

$$
d_x=\frac{3\mu_sU}{\rho g}\frac{d-d_\infty}{d^3}.
$$

Define $\ell=\rho gd_\infty^3/(3\mu_sU)$ and $P(\delta)=\delta^3/3+\delta^2/2+\delta+\ln(\delta-1)$. Integrating from the contact yields **the [upstream basin profile of a sediment-lubricated mountain](../../../../../upstream-basin-profile-of-a-sediment-lubricated-mountain.md)**:

$$
\boxed{\frac x\ell=P\left(\frac{d(x)}{d_\infty}\right)-P(3),\qquad x\leq0.}
$$

Equivalently, $d(x)=d_\infty P^{-1}(P(3)+x/\ell)$ on $1<\delta\leq3$. The inverse is uniquely defined because $P'(\delta)=\delta^3/(\delta-1)>0$; an elementary explicit inverse is unnecessary. This profile tends to $d_\infty$ as $x\to-\infty$, approaches $3d_\infty$ at the contact and has the same surface slope there as the mountain branch. Its far-field excess decays exponentially on length scale $\ell$, which increases as the sediment [viscosity](../../../../../dynamic-viscosity.md) decreases.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
