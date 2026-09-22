# Paper 332

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_332.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_332.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 332](paper-332.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put ice in $x<a(t)$ and ocean in $x>a(t)$, with $x$ increasing into the ocean. This is a [saline Stefan problem](../../../geophysics.md#saline-stefan-problem). The ice and liquid temperatures satisfy

$$
T_{s,t}=\kappa T_{s,xx},
\qquad
T_{l,t}=\kappa T_{l,xx},
$$

and the ocean salinity satisfies $C_t=DC_{xx}$. The far-field and interfacial conditions are

$$
T_s(-\infty,t)=T_{-\infty},
\quad T_l(+\infty,t)=T_m,
\quad C(+\infty,t)=C_0,
$$



$$
T_s(a,t)=T_l(a,t)=T_i=T_m-mC_i,
\quad C(a,t)=C_i,
$$



$$
\rho L_f\dot a=k_T(T_{s,x}-T_{l,x})_{x=a},
\qquad
-D C_x(a^+,t)=C_i\dot a.
$$

The last two equations are the [Stefan condition](../../../geophysics.md#stefan-condition) and solute conservation. Salt is taken to be absent from the ice. The field sketch has two broad thermal boundary layers of width $O(\sqrt{\kappa t})$ and a liquid-side salinity layer of width $O(\sqrt{Dt})$.

The [diffusion equation](../../../diffusion-equation.md) is invariant under $(x,t)\mapsto(cx,c^2t)$, so a solution with constant far-field data and no fixed length has $a/\sqrt{Dt}$ constant. Write

$$
a(t)=2\lambda\sqrt{Dt},
\qquad \epsilon=\sqrt{D/\kappa}.
$$

The [Neumann solution of the Stefan problem](../../../geophysics.md#neumann-solution-of-the-stefan-problem) becomes

$$
T_s=T_{-\infty}+(T_i-T_{-\infty})
\frac{1+\operatorname{erf}(x/(2\sqrt{\kappa t}))}
{1+\operatorname{erf}(\epsilon\lambda)},
$$



$$
T_l=T_m+(T_i-T_m)
\frac{\operatorname{erfc}(x/(2\sqrt{\kappa t}))}
{\operatorname{erfc}(\epsilon\lambda)},
$$



$$
C=C_0+(C_i-C_0)
\frac{\operatorname{erfc}(x/(2\sqrt{Dt}))}
{\operatorname{erfc}(\lambda)}.
$$

Substitution into the salt balance and the [Stefan condition](../../../geophysics.md#stefan-condition) gives the required pair of equations. With $c_p=k_T/(\rho\kappa)$ and

$$
F(z)=\sqrt\pi z e^{z^2}\operatorname{erfc}z,
$$

they are

$$
\boxed{F(\lambda)=1-\frac{C_0}{C_i}
=1-\frac{mC_0}{T_m-T_i},}
$$



$$
\boxed{
\sqrt\pi\frac{L_f}{c_p}\epsilon\lambda e^{\epsilon^2\lambda^2}
=\frac{T_i-T_{-\infty}}{1+\operatorname{erf}(\epsilon\lambda)}
-\frac{T_m-T_i}{\operatorname{erfc}(\epsilon\lambda)}.}
$$

When $\epsilon\ll1$, heat diffuses much farther than salt. The leading heat-flux balance gives

$$
\boxed{T_i\sim\frac{T_m+T_{-\infty}}2,}
\qquad
\boxed{F(\lambda)\sim1-\frac{2mC_0}{T_m-T_{-\infty}}.}
$$

Since $F$ has the sign of $\lambda$, ice grows when $T_m-T_{-\infty}>2mC_0$, is stationary at equality, and ablates when $T_m-T_{-\infty}<2mC_0$.

During growth, salt rejection gives $C_i>C_0$. Moving from the interface into the ocean, the phase-diagram trajectory first moves rapidly toward lower $C$ at nearly fixed $T$ and can fall below the [liquidus](../../../thermodynamics.md#liquidus); this is [constitutional supercooling](../../../geophysics.md#constitutional-supercooling). During ablation, $C_i<C_0$, so the near-interface trajectory moves toward larger $C$ and into the stable liquid region above the liquidus. Ablation occurs because the heat conducted from the warmer ocean to the interface exceeds the heat that the colder ice can remove; melting and salt diffusion then maintain local liquidus equilibrium.

## 2

↑ **Parent:** [Paper 332](paper-332.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $K=k\Delta\rho g/\mu$. [Hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) continuity at the lower boundary of the light current gives

$$
p(x,z,t)=p_H-\rho g(H-z)+\Delta\rho g\,[h(x,t)-z]
$$

inside the current, so $p_x=\Delta\rho g h_x$. [Darcy law](../../../porous-media-flow.md#darcy-law) gives the depth-integrated horizontal flux per unit transverse width

$$
q=-Kh h_x.
$$

Thus the [porous gravity current](../../../porous-media-flow.md#porous-gravity-current) satisfies

$$
\boxed{\phi h_t+q_x=0,
\qquad q=-\frac{k\Delta\rho g}{\mu}hh_x}
$$

away from the fracture. The boundary and front conditions are

$$
q(0,t)=Q,
\quad h(x_N,t)=0,
\quad q(x_N,t)=0.
$$

At $x=L$, the pressure excess at the base of the fracture is $\Delta\rho g h_L$. Taking upward leakage as positive,

$$
Q_l=\frac{W\alpha k\Delta\rho g}{\mu b}h_L,
\qquad
\boxed{q(L^+,t)=q(L^-,t)-Q_l.}
$$

This jump is the local [mass conservation](../../../continuum-mechanics.md#mass-conservation) law for a [leaky porous gravity current](../../../porous-media-flow.md#leaky-porous-gravity-current).

At late times, $q=Q$ to leading order on $0<x<L$, while $Q_l\simeq Q$. Integrating $q=-K(h^2)_x/2$ gives

$$
\boxed{
h(x)=\left[h_0^2-(h_0^2-h_L^2)\frac{x}{L}\right]^{1/2}.}
$$

Leakage balance and the pressure-driven drop determine

$$
\boxed{h_L=\frac{\mu bQ}{W\alpha k\Delta\rho g},}
\qquad
\boxed{h_0=\left(h_L^2+\frac{2\mu QL}{k\Delta\rho g}\right)^{1/2}.}
$$

In the far field, $h(L,t)\simeq h_L$ and

$$
\phi h_t=K(hh_x)_x.
$$

Balancing the two sides with $h=O(h_L)$ gives

$$
\boxed{x_N-L=O\left[\left(\frac{k\Delta\rho g h_L}{\phi\mu}t\right)^{1/2}\right].}
$$

More precisely, set

$$
h=h_L f(\eta),
\qquad
\eta=\frac{x-L}{(Kh_Lt/\phi)^{1/2}}.
$$

The [self-similar solution](../../../partial-differential-equation.md#similarity-solution) is determined by

$$
(ff')'+\frac\eta2f'=0,
\qquad
f(0)=1,
\quad f(\eta_N)=0,
\quad ff'(\eta_N)=0,
$$

and $x_N=L+\eta_N(Kh_Lt/\phi)^{1/2}$.

## 3

↑ **Parent:** [Paper 332](paper-332.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [shelfy stream](../../../geophysics.md#shelfy-stream) is grounded ice with nearly depth-independent horizontal velocity. If the lubricating till has thickness $d$ and viscosity $\mu_t$, its simple-shear traction is approximately $\mu_tu/d$. Comparison with $\tau_b=\mu u/\lambda$ gives

$$
\boxed{\lambda\sim\frac{\mu}{\mu_t}d,}
$$

so $\lambda$ has dimensions of length.

Hydrostatic pressure contributes the depth-integrated longitudinal force $-\rho gh^2/2$, while the Newtonian extensional stress contributes $4\mu h u_x$ by the [shallow-shelf approximation](../../../geophysics.md#shallow-shelf-approximation). Balancing the change of their sum against basal drag on a slice gives

$$
\boxed{4\mu(hu_x)_x-\rho ghh_x-\mu\frac u\lambda=0.}
$$

For a freely floating [ice shelf](../../../geophysics.md#ice-shelf), hydrostatic flotation reduces the gravitational driving by $1-\rho/\rho_w$ and removes basal drag:

$$
\boxed{4\mu(hu_x)_x-
ho g\left(1-\frac\rho{\rho_w}\right)hh_x=0.}
$$

Depth-integrated [mass conservation](../../../continuum-mechanics.md#mass-conservation) is

$$
\boxed{h_t+(hu)_x=0}
$$

in the absence of accumulation or ablation.

In a thin stream with horizontal scale $L_x$, the ratio of extensional resistance to basal drag is $O(\lambda h/L_x^2)$, which is small when the thin-film condition $h/L_x\ll1$ is combined with $\lambda\ll h_G$. For steady flux $hu=q$, neglecting extension gives

$$
\rho ghh_x=-\frac{\mu q}{\lambda h}.
$$

At the [grounding line](../../../geophysics.md#grounding-line), flotation over a bed depth $b$ gives

$$
\boxed{h_G=\frac{\rho_w}{\rho}b.}
$$

Integration yields

$$
\boxed{
h=h_G\left(1-\frac x\delta\right)^{1/3},
\qquad
\delta=\frac{\rho g\lambda h_G^3}{3\mu q},
\qquad \alpha=\frac13.}
$$

The grounding-line slope is $|h_x(0)|=\mu q/(\rho g\lambda h_G^2)$. Thin-film theory therefore also requires

$$
\boxed{\lambda\gg\frac{\mu q}{\rho g h_G^2}.}
$$

This and $\lambda\ll h_G$ are compatible precisely when $\mu q/(\rho gh_G^3)\ll1$.

The total horizontal force resultant in the stream is

$$
N=4\mu h u_x-\frac12\rho gh^2.
$$

The floating shelf equations and its ocean-front traction imply that the force it exerts at the grounding line is the ocean's hydrostatic force, so

$$
N(0)=-\frac12\rho_wgb^2.
$$

Using flotation and the approximate stream solution,

$$
u_x(0)=-\frac q{h_G^2}h_x(0)
=\frac{\mu q^2}{\rho g\lambda h_G^4}.
$$

Consequently

$$
4\mu h_Gu_x(0)
=\frac12\rho gh_G^2\left(1-\frac\rho{\rho_w}\right),
$$

and the grounding-line flux-thickness relation is

$$
\boxed{
q=\frac{\rho g}{2\sqrt2\,\mu}
\left[\lambda h_G^5\left(1-\frac\rho{\rho_w}\right)\right]^{1/2}.}
$$

## 4

↑ **Parent:** [Paper 332](paper-332.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Because the wavelength is much smaller than the shelf thickness, the [ice-shelf corrugation relaxation](../../../geophysics.md#ice-shelf-corrugation-relaxation) may be treated as [Stokes flow](../../../stokes-flow.md) in the half-space $z>0$, with the mean ice-ocean boundary at $z=0$. Let

$$
\eta=\widehat\eta e^{ikx+\sigma t},
\qquad
\mathbf u=\nabla\times(\psi\widehat{\mathbf y}),
$$

so $u=-\psi_z$ and $w=\psi_x$. Taking the curl of the Stokes equation gives the [biharmonic stream function for planar Stokes flow](../../../stokes-flow.md#biharmonic-stream-function-for-planar-stokes-flow) equation $\nabla^4\psi=0$. Decay as $z\to\infty$ removes the growing modes, leaving

$$
\boxed{\psi=(A+Bz)e^{-kz}e^{ikx+\sigma t}.}
$$

Thus

$$
u=(kA-B+kBz)e^{-kz}e^{ikx+\sigma t},
\qquad
w=ik(A+Bz)e^{-kz}e^{ikx+\sigma t},
$$

and the perturbation pressure obtained from the Stokes equation is

$$
\boxed{p'=2i\mu kB e^{-kz}e^{ikx+\sigma t}.}
$$

The linearized zero-[shear stress](../../../viscous-fluid-flow.md#shear-stress) condition at $z=0$ is

$$
\mu(u_z+w_x)=2\mu k(B-kA)e^{ikx+\sigma t}=0,
$$

so $B=kA$. The water is hydrostatic, and displacement of the density interface gives the normal-stress condition

$$
-p'+2\mu w_z=(\rho_w-\rho)g\eta.
$$

After $B=kA$, one has $w_z(0)=0$, so

$$
-2i\mu k^2A=(\rho_w-\rho)g\widehat\eta.
$$

The [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) $\eta_t=w(0)$ gives $\sigma\widehat\eta=ikA$. Eliminating $A$ yields

$$
\boxed{\sigma=-\frac{(\rho_w-\rho)g}{2\mu k}<0.}
$$

Hence a corrugation of wavelength $\lambda=2\pi/k$ decays on the timescale

$$
\boxed{\tau(\lambda)=\frac1{|\sigma|}
=\frac{4\pi\mu}{(\rho_w-\rho)g\lambda}.}
$$

Hydrostatic buoyancy supplies the restoring stress, while viscous deformation over depth $O(k^{-1})$ supplies the resistance. Shorter wavelengths deform a shallower but more strongly sheared layer and therefore have a longer decay time in this gravity-only model. As ice is advected away from the grounding line, long corrugations should disappear first, leaving progressively shorter-wavelength structure farther downstream.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
