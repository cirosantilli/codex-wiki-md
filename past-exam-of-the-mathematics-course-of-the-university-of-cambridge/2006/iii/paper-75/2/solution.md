<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work in the frame of the steadily advancing mush, so the rigid primary-crystal skeleton moves with $-V\mathbf e_z$. Let $\phi$ be [solid fraction](../../../../../solid-fraction.md), $C$ the pore-liquid [concentration](../../../../../concentration.md), $\mathbf q=(u,w)$ the [Darcy flux](../../../../../darcy-velocity.md) relative to that skeleton, and $K$ the common [thermal conductivity](../../../../../thermal-conductivity.md). Set $\kappa=K/(\rho c_p)$, the [thermal diffusivity](../../../../../thermal-diffusivity.md). The actual pore [velocity](../../../../../velocity.md) is $\mathbf q/(1-\phi)-V\mathbf e_z$. Primary crystals are taken to exclude solute; the residual pore liquid freezes into a two-solid eutectic product at the bottom. These are the standard binary [mushy layer](../../../../../mushy-layer.md) assumptions implicit in using a single [liquidus](../../../../../liquidus.md) and an eutectic floor.

It is convenient to use hydraulic [pressure](../../../../../pressure.md) $P=p+\rho gz$, absorbing the constant-density gravitational term. With equal phase properties, no solute [diffusion](../../../../../diffusion.md), negligible fluid inertia and local [liquidus](../../../../../liquidus.md) equilibrium, a complete mush model is

$$
\nabla\cdot\mathbf q=0,\qquad
\mathbf q=-\frac{\Pi}{\mu}\nabla P,\qquad T=-mC,
$$



$$
-V\partial_z[(1-\phi)C]+\nabla\cdot(\mathbf q C)=0,
$$



$$
(\mathbf q-V\mathbf e_z)\cdot\nabla T+\frac{VL}{c_p}\partial_z\phi=\kappa\nabla^2T.
$$

The last equation follows from [conservation of energy](../../../../../conservation-of-energy.md) with mixture [specific enthalpy](../../../../../specific-enthalpy.md) $c_pT-L\phi$. Sensible heat is transported by the total volume flux $\mathbf q-V\mathbf e_z$; the primary solid carries the latent-enthalpy flux $VL\phi\mathbf e_z$. In particular the sign of the latent-heat term is fixed by the downward-moving skeleton.

At the liquid roof, impose

$$
z=h:\quad T=T_0=-mC_0,\quad C=C_0,\quad\phi=0,\quad T_z=G,\quad P=P_0-\frac12E^2x^2.
$$

Here $P_0=p_0+\rho gh$. The gradient condition matches [heat flux](../../../../../heat-flux-density.md) into the imposed liquid field, since there is no phase-fraction jump at this roof and the phase conductivities are equal. The pore [velocity](../../../../../velocity.md) there equals the relative [Darcy velocity](../../../../../darcy-velocity.md). At the floor,

$$
z=0:\quad T=T_E,\quad C=C_E=-T_E/m,\quad w=0.
$$

There is no liquid penetration into fully solid material. The unspecified [solid fraction](../../../../../solid-fraction.md) at the floor is determined by the solute balance, not set to one: remaining eutectic liquid freezes as it crosses the floor. If $C_s$ denotes the bulk [concentration](../../../../../concentration.md) of the final solid product, the floor solute balance and [Stefan condition](../../../../../stefan-condition.md) are

$$
C_s=(1-\phi(0))C_E,\qquad
K[T_z(0^-)-T_z(0^+)]=\rho LV[1-\phi(0)].
$$

Maintaining the floor at $T_E$ permits the solid-side bath to remove this final [latent heat](../../../../../latent-heat.md). Equivalently its required gradient is $T_z(0^-)=T_z(0^+)+\rho LV[1-\phi(0)]/K$. No additional imposed solid-side gradient is specified. Laterally we take the quadratic-pressure strain solution, without sidewalls; finite sidewalls would require additional flow conditions and generally break this horizontal invariance.

For uniform [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md), [incompressible flow](../../../../../incompressible-flow.md) gives $\nabla^2P=0$. The roof [pressure](../../../../../pressure.md) and zero normal flow at the floor are satisfied by

$$
P=P_0-\frac{E^2}{2}(x^2+h^2-z^2),\qquad
\boxed{u=\alpha x,\quad w=-\alpha z,\quad \alpha=\frac{\Pi E^2}{\mu}.}
$$

Horizontal outflow is balanced by downward inflow. The parameter $\alpha$ is an inverse time; $E^2$ in the printed [pressure](../../../../../pressure.md) condition already has dimensions of [pressure](../../../../../pressure.md) divided by length squared, so no extra density factor belongs in this definition.

With $T=T(z)$, $C=C(z)$ and $\phi=\phi(z)$, the $x$-dependence disappears from both scalar balances. Although $u$ is nonzero, its horizontal divergence cancels $w_z$ in $\nabla\cdot(\mathbf q C)$. The exact [strain-driven steady mush](../../../../../strain-driven-steady-mush.md) equations become

$$
\boxed{\kappa T''+(V+\alpha z)T'-\frac{VL}{c_p}\phi'=0,\qquad
[V(1-\phi)C]'=-\alpha zC',\qquad C=-T/m.}
$$

Together with $T(0)=T_E$, $T(h)=T_0$, $T'(h)=G$ and $\phi(h)=0$, they determine the scalar fields and the unknown thickness. This reduction proves that the equations admit horizontally invariant scalar solutions despite the imposed straining flow. An equivalent useful form, obtained by differentiating the solute equation, is

$$
\phi'=\frac{1-\phi+\alpha z/V}{C}C',\qquad
\kappa T''+\left[V+\alpha z+\frac{L}{c_pmC}\{V(1-\phi)+\alpha z\}\right]T'=0.
$$

This exact form also shows why one must not silently discard [latent heat](../../../../../latent-heat.md) in an arbitrary strong-flow calculation.

Define $\Delta T=T_0-T_E>0$, $R=\alpha h/V$ and $S=L/(c_p\Delta T)$. For the stated regular ordering $R\gg S\gg1$, strain transport dominates skeleton transport and the bounded phase-change enthalpy contribution. More precisely, at fixed finite thermal strain number $\alpha h^2/\kappa$, the dimensionless energy equation is

$$
T_{\zeta\zeta}+\frac{Vh}{\kappa}(1+R\zeta)T_\zeta-\frac{VhL}{\kappa c_p}\phi_\zeta=0,\qquad\zeta=z/h,
$$

so its skeleton and integrated latent-heat corrections are small in $1/R$ and $S/R$ respectively. The leading [strain-dominated mush temperature profile](../../../../../strain-dominated-mush-temperature-profile.md) obeys $\kappa T''+\alpha zT'=0$. Put $\delta=\sqrt{2\kappa/\alpha}$ and $H=h/\delta$. Integrating first for $T'$ and then for $T$ gives

$$
T'=B e^{-z^2/\delta^2},\qquad
\boxed{T(z)\simeq T_E+\Delta T\frac{\operatorname{erf}(z/\delta)}{\operatorname{erf}H}.}
$$

The [error function](../../../../../error-function.md) profile follows from integrating a Gaussian, with $\operatorname{erf}x=(2/\sqrt\pi)\int_0^x e^{-s^2}\,ds$. Matching the roof gradient gives the requested transcendental thickness relation

$$
\boxed{G=\frac{2\Delta T}{\sqrt\pi\delta}\frac{e^{-H^2}}{\operatorname{erf}H},\qquad h=\delta H,\quad\delta=\sqrt{\frac{2\kappa\mu}{\Pi E^2}}.}
$$

For prescribed $G>0$ and $\Delta T>0$ the right side decreases continuously from infinity to zero as $H$ increases, so it fixes one positive leading-order thickness. The resulting $h$ must still satisfy the assumed ordering and the phase-fraction constraints.

To find the product composition, integrate the exact solute balance from the roof to an arbitrary depth. With $f=1-\phi$,

$$
f(z)C(z)=C_0-\frac\alpha V\left[z(C(z)-C_0)+\int_z^h(C(s)-C_0)\,ds\right].
$$

At $z=0$, the exact floor composition is therefore

$$
\boxed{C_s=C_0-\frac\alpha V\int_0^h(C-C_0)\,dz
=C_0-\frac\alpha{mV}\int_0^h(T_0-T)\,dz.}
$$

The minus sign has a direct physical meaning: the horizontal outflow removes more salt than arrives at the same depth from a uniform-$C_0$ liquid, leaving a depleted solid product. Using the leading [error function](../../../../../error-function.md) profile and

$$
\int_0^h\operatorname{erf}(z/\delta)\,dz
=h\operatorname{erf}H+\frac\delta{\sqrt\pi}(e^{-H^2}-1)
$$

yields

$$
\boxed{C_s\simeq C_0-\frac{\alpha\Delta T\delta}{mV\sqrt\pi}\frac{1-e^{-H^2}}{\operatorname{erf}H}.}
$$

The full [solid fraction](../../../../../solid-fraction.md) follows by substituting this same profile into the preceding [integral](../../../../../integral.md) formula for $f(z)$. It has $\phi(h)=0$ and $1-\phi(0)=C_s/C_E$. A physical branch requires $0\le C_s\le C_E$ and $0\le\phi\le1$. In this monotone profile, $C_s\ge0$ ensures a nonnegative [liquid fraction](../../../../../liquid-fraction.md) everywhere; it is not permissible to interpret a negative formal result as a material composition.

The error-function reduction is a regular leading approximation, not a uniform statement for every possible scaling of the thermal strain number. If $\alpha h^2/\kappa$ becomes singularly large along the ordering limit, a thin basal layer can amplify the discarded terms. The printed two inequalities alone do not specify that extra scaling. In such a regime the displayed exact scalar equations and boundary conditions, rather than an unqualified zero-latent-heat profile, provide the appropriate thickness and composition calculation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
