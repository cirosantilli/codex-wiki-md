<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $z$ increase upwards, so the bed is at $z=-b(x)$, the surface is at $z=h(x,t)$, and $H=h+b$. In the [shallow-shelf approximation](../../../../../shallow-shelf-approximation.md) the [incompressible flow](../../../../../incompressible-flow.md) has nearly depth-uniform horizontal speed $u$ and vertical strain $w_z=-u_x$. The [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md), together with the [hydrostatic approximation](../../../../../hydrostatic-approximation.md), then gives

$$
\sigma_{zz}=-\rho g(h-z),\qquad \sigma_{xx}=-\rho g(h-z)+4\mu u_x.
$$

The factor four includes both horizontal extension and the [pressure](../../../../../pressure.md) correction required by vertical compression. Integrating horizontal force balance over depth, using zero surface shear and the bed traction, gives the membrane-stress [derivative](../../../../../derivative.md) $\partial_x(4\mu Hu_x)$ and the gravitational driving force $-\rho gHh_x$. The thin [subglacial till](../../../../../subglacial-till.md) layer is idealized by [Newtonian till lubrication](../../../../../newtonian-till-lubrication.md) and undergoes [Couette flow](../../../../../couette-flow.md), with resisting basal stress $\lambda\mu u/l$. Hence force balance and [mass conservation](../../../../../mass-conservation.md) yield

$$
\boxed{4\mu\partial_x(Hu_x)-\rho gHh_x-\lambda\mu\frac ul=0,\qquad H_t+\partial_x(Hu)=0.}
$$

Since $b$ is fixed, $H_t=h_t$. No accumulation or ablation is included.

At the [grounding line](../../../../../grounding-line.md), the first boundary condition is [ice-sheet flotation](../../../../../ice-sheet-flotation.md):

$$
\boxed{\rho H_G=\rho_wb_G,\qquad H_G=\frac{\rho_w}{\rho}\alpha x_G.}
$$

For an unbuttressed [ice shelf](../../../../../ice-shelf.md), the second is the extensional stress required to balance the difference between the integrated [ice](../../../../../ice.md) and seawater [hydrostatic pressures](../../../../../hydrostatic-pressure.md). The [ice](../../../../../ice.md) contribution is $\rho gH_G^2/2$, while the [water](../../../../../water.md) contribution is $\rho_wgb_G^2/2$. On using [ice-sheet flotation](../../../../../ice-sheet-flotation.md), their difference is $\rho g'H_G^2/2$, with $g'=g(1-\rho/\rho_w)>0$. Equivalently, shelf force balance integrates to $4\mu Hu_x-\rho g'H^2/2=\text{constant}$; absence of a buttressing force sets this constant to zero. Thus the [unbuttressed Newtonian grounding-line stress](../../../../../unbuttressed-newtonian-grounding-line-stress.md) condition is

$$
\boxed{4\mu H_Gu_{x,G}=\frac12\rho g'H_G^2,\qquad u_{x,G}=\frac{g'H_G}{8\nu},\qquad \nu=\mu/\rho.}
$$

Here $\nu$ is [kinematic viscosity](../../../../../kinematic-viscosity.md); it appears in the printed target formula without an explicit definition.

The ratio of longitudinal stress divergence to till drag is of order $4lH/(\lambda L^2)$. The given small-parameter limit therefore yields the friction-dominated bulk relation

$$
\boxed{u=-\frac l\lambda\frac g\nu Hh_x,\qquad h_t=\frac l\lambda\frac g\nu\partial_x(H^2h_x).}
$$

The coefficient depends on the basal lubrication, and $h_x<0$ gives seaward motion. This is a bulk reduction: longitudinal stress has been neglected in the differential equation but its boundary traction remains specified. A complete uniformly valid approximation close to the [grounding line](../../../../../grounding-line.md) could require a membrane-stress [boundary layer](../../../../../boundary-layer.md). In the remainder, use the pointwise friction closure and retain the shelf stress condition as the boundary data, as requested in the paper.

Differentiate the [ice-sheet flotation](../../../../../ice-sheet-flotation.md) condition along the moving [grounding line](../../../../../grounding-line.md):

$$
H_t+H_x\dot x_G=\alpha\frac{\rho_w}{\rho}\dot x_G,\qquad \left(\alpha\frac{\rho_w}{\rho}-H_x\right)\dot x_G=H_t=-uH_x-Hu_x.
$$

Now $H_x=h_x+\alpha$. Substitution of the friction-dominated speed and the shelf stress boundary condition gives the [friction-dominated grounding-line evolution law](../../../../../friction-dominated-grounding-line-evolution-law.md):

$$
\boxed{\left(\alpha\frac{\rho_w}{\rho}-H_x\right)\dot x_G=\frac l\lambda\frac g\nu Hh_x(h_x+\alpha)-\frac{g'}{8\nu}H^2\quad\text{at }x=x_G(t).}
$$

The coefficient of $\dot x_G$ is the spatial [derivative](../../../../../derivative.md) of the flotation deficit, up to sign. If it vanishes, the implicit equation remains the correct compatibility condition but division to determine a finite speed is invalid; tangential contact needs separate analysis.

In a steady state, [volume flux per unit width](../../../../../volume-flux-per-unit-width.md) is constant: $Hu=q_0$. The friction relation gives

$$
h_x=-\frac{\lambda\nu q_0}{lgH^2},\qquad H_x=\alpha-\frac{\lambda\nu q_0}{lgH^2}.
$$

Differentiating $Hu=q_0$ and using $u_x=g'H/(8\nu)$ at the [grounding line](../../../../../grounding-line.md) gives

$$
\frac{q_0}{H}H_x+\frac{g'H^2}{8\nu}=0,\qquad \frac{g'H^5}{8\nu}=q_0\left(\frac{\lambda\nu q_0}{lg}-\alpha H^2\right).
$$

Put $\beta=l/\lambda$, $\mathcal H=H/\beta$ and $\mathcal Q=\nu q_0/(g\beta^3)$. Substitution and cancellation of $g\beta^5/\nu$ yield the [steady friction-dominated grounding-line thickness relation](../../../../../steady-friction-dominated-grounding-line-thickness-relation.md):

$$
\boxed{\frac{g'}{8g}\mathcal H^5=\mathcal Q(\mathcal Q-\alpha\mathcal H^2).}
$$

For $q_0>0$ and a bed deepening seaward ($\alpha\ge0$), the polynomial $(g'/8g)\mathcal H^5+\alpha\mathcal Q\mathcal H^2-\mathcal Q^2$ is strictly increasing for $\mathcal H>0$, starts negative and tends to infinity, so it has exactly one positive root. At that root $\mathcal Q>\alpha\mathcal H^2$ and $H_x<0$, as required by steady outward extension. The relation belongs to the specified friction closure; it is not a flux law for arbitrary till rheology or arbitrary membrane-stress matching.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
