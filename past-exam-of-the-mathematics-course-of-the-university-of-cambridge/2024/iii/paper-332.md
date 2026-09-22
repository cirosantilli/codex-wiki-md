# Paper 332

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_332.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_332.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
  - [vi](#2/vi)
    - [Solution](#2/vi/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 332](paper-332.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write the given pressure-dependent ratio of [permeability of a porous medium](../../../porous-media-flow.md#permeability-of-a-porous-medium) to sponge thickness as

$$
\frac{k(p)}{h(p)}=Kp^{-\beta},
$$

where $K$ is constant. The [fluid pressure](../../../fluid-mechanics.md#fluid-pressure) drop across the sponge is the [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) of the current,

$$
p=\rho gH,
$$

because the air pressures above and below are equal. Therefore [Darcy's law](../../../porous-media-flow.md#darcy-law) gives the downward [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) per unit horizontal area as

$$
w=\frac{k(p)}{\mu h(p)}p
=\frac K\mu p^{1-\beta}
=\boxed{D H^{1-\beta}},
\qquad
D=\frac K\mu(\rho g)^{1-\beta}.
$$

**Thus the sponge drainage obeys a [power law](../../../analysis.md#power-law) in the current thickness, as described by [pressure-dependent Darcy drainage](../../../porous-media-flow.md#pressure-dependent-darcy-drainage).**

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $z$ measure height above the sponge. Under the [long-wave approximation](../../../viscous-fluid-flow.md#long-wave-approximation), [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) gives $p_x=\rho gH_x$, and the horizontal balance for [viscous fluid flow](../../../viscous-fluid-flow.md) is

$$
\mu u_{zz}=\rho gH_x.
$$

The [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) $u(0)=0$ and [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition) $u_z(H)=0$ give

$$
u=\frac{\rho g}{\mu}H_x
\left(\frac{z^2}{2}-Hz\right).
$$

Integrating this [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) profile gives the horizontal [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) per unit span

$$
q=\int_0^H u\,dz
=-AH^3H_x,
\qquad
A=\frac{\rho g}{3\mu}.
$$

Local [mass conservation](../../../continuum-mechanics.md#mass-conservation) includes the downward loss found in part i:

$$
H_t+q_x=-DH^{1-\beta}.
$$

Consequently the required nonlinear [partial differential equation](../../../partial-differential-equation.md) is

$$
\boxed{H_t=A(H^3H_x)_x-DH^{1-\beta}}.
$$

If the imposed inlet flux is $Q_0t^\alpha$ and the moving front is $x=x_N(t)$, sufficient [boundary conditions](../../../differential-equation.md#boundary-condition) are

$$
-AH(0,t)^3H_x(0,t)=Q_0t^\alpha,
$$



$$
H(x_N(t),t)=0,
\qquad
q(x_N(t),t)=0.
$$

For a current released onto a dry substrate one also takes the [initial condition](../../../differential-equation.md#initial-condition) $H(x,0)=0$ away from the source. The front position is part of this [moving-boundary problem](../../../partial-differential-equation.md#moving-boundary-problem).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Seek a [similarity solution](../../../partial-differential-equation.md#similarity-solution) in the dimensionally completed form

$$
H=H_*\left(\frac t{t_*}\right)^aF(\eta),
\qquad
\eta=\frac{x}{x_*(t/t_*)^b},
$$

where the fixed scales absorb $A,D$, and $Q_0$. Its inlet [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) scales as

$$
H^3H_x\sim t^{4a-b},
$$

so the prescribed source requires

$$
4a-b=\alpha.
$$

The time derivative, horizontal [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) term, and [pressure-dependent Darcy drainage](../../../porous-media-flow.md#pressure-dependent-darcy-drainage) term scale respectively as

$$
t^{a-1},
\qquad
t^{4a-2b},
\qquad
t^{a(1-\beta)}.
$$

Equating the three exponents gives

$$
a-1=4a-2b=a(1-\beta).
$$

Solving these [linear equations](../../../linear-algebra.md#linear-equation) together with the inlet condition yields the [similarity exponents of a draining gravity current](../../../reduced-gravity.md#similarity-exponents-of-a-draining-gravity-current)

$$
\boxed{
a=\frac{2\alpha+1}{5},
\qquad
b=\frac{3\alpha+4}{5},
\qquad
\beta=\frac5{2\alpha+1}}.
$$

Equivalently,

$$
\boxed{\alpha=\frac12\left(\frac5\beta-1\right)},
$$

and, up to constant dimensional scales,

$$
\boxed{
H=t^{(2\alpha+1)/5}
F\!\left(\frac{x}{t^{(3\alpha+4)/5}}\right)}.
$$

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

For $\alpha=2$, part iii gives $a=1$, $b=2$, and $\beta=1$. Put

$$
H=tF(\eta),
\qquad
\eta=\frac{x}{t^2},
\qquad
x_N(t)=\eta_Nt^2.
$$

Substitution into the nonlinear [partial differential equation](../../../partial-differential-equation.md) gives the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation)

$$
\boxed{
A(F^3F')'+2\eta F'-F-D=0}
$$

with [boundary conditions](../../../differential-equation.md#boundary-condition)

$$
\boxed{-AF(0)^3F'(0)=Q_0,
\qquad F(\eta_N)=0,
\qquad F^3F'\longrightarrow0
\ \text{as }\eta\uparrow\eta_N}.
$$

To find the leading edge, set $y=\eta_N-\eta$ and suppose $F\sim Cy^p$. The two singular terms in the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) have orders $y^{4p-2}$ and $y^{p-1}$. Their exponents agree only when $p=1/3$. Their leading coefficients then satisfy

$$
\frac{AC^4}{9}-\frac{2\eta_NC}{3}=0,
$$

whereas $F$ and the constant drainage $D$ are lower-order terms. Hence

$$
\boxed{
F(\eta)\sim
\left(\frac{6\eta_N}{A}\right)^{1/3}
(\eta_N-\eta)^{1/3}}
\qquad(\eta\uparrow\eta_N).
$$

The [draining gravity current](../../../reduced-gravity.md#draining-gravity-current) therefore has a one-third-power leading edge and its flux vanishes there.

## 2

↑ **Parent:** [Paper 332](paper-332.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [density anomaly of water](../../../geophysics.md#density-anomaly-of-water) makes [mass density](../../../fluid-mechanics.md#density) increase with temperature up to $T_m$ and decrease above $T_m$. Since temperature increases with depth in the stated layer, the density profile first increases to its maximum $\rho_m$ at the $T=T_m$ isotherm and then decreases toward the warm bottom.

The upper region has denser water below lighter water and hence [stable density stratification](../../../gravity-wave.md#stable-density-stratification). Below the density maximum, density decreases downward, so lighter water lies beneath denser water and gives [unstable density stratification](../../../gravity-wave.md#unstable-density-stratification). The lower region therefore overturns by [thermal convection](../../../fluid-mechanics.md#thermal-convection), while the cold upper region remains a stagnant cap. This coexistence is [penetrative convection](../../../geophysics.md#penetrative-convection).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $\delta_T$ be the thickness of the [thermal boundary layer](../../../continuum-mechanics.md#thermal-boundary-layer) immediately below $z=h$, let $\nu$ be the [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity), let $\kappa$ be the [thermal diffusivity](../../../thermodynamics.md#thermal-diffusivity), and let $\operatorname{Ra}_c$ be the critical local [Rayleigh number](../../../geophysics.md#rayleigh-number). The density contrast driving the boundary layer follows from the [density anomaly of water](../../../geophysics.md#density-anomaly-of-water):

$$
\Delta\rho
=\rho(T_h)-\rho(T_w)
=\rho_m\alpha
\left[(T_w-T_m)^2-(T_h-T_m)^2\right].
$$

A [Local Rayleigh-number closure](../../../geophysics.md#local-rayleigh-number-closure) sets

$$
\frac{g\Delta\rho\,\delta_T^3}
{\rho_m\nu\kappa}
=\operatorname{Ra}_c,
$$

and therefore

$$
\delta_T=
\left[
\frac{\operatorname{Ra}_c\nu\kappa}
{g\alpha\{(T_w-T_m)^2-(T_h-T_m)^2\}}
\right]^{1/3}.
$$

By [Fourier's law](../../../thermodynamics.md#fourier-s-law), the upward [heat flux](../../../thermodynamics.md#heat-flux-density) through this layer is

$$
\boxed{
F_c=k(T_w-T_h)
\left[
\frac{g\alpha\{(T_w-T_m)^2-(T_h-T_m)^2\}}
{\operatorname{Ra}_c\nu\kappa}
\right]^{1/3}},
$$

where $k$ is the water's [thermal conductivity](../../../thermodynamics.md#thermal-conductivity). This expression applies while the quantity inside braces is positive.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Set

$$
\Delta=T_w-T_m>0,
\qquad
x=T_m-T_h,
$$

so $0<x<\Delta$. Apart from material constants, the [heat flux](../../../thermodynamics.md#heat-flux-density) in part ii is

$$
F_c\propto
(\Delta+x)(\Delta^2-x^2)^{1/3}
=(\Delta+x)^{4/3}(\Delta-x)^{1/3}.
$$

The [derivative](../../../calculus.md#derivative) of its logarithm vanishes when

$$
\frac4{3(\Delta+x)}-
\frac1{3(\Delta-x)}=0,
$$

which gives the maximizing interface temperature

$$
\boxed{x=\frac35\Delta},
\qquad
\boxed{T_m-T_h=\frac35(T_w-T_m)}.
$$

Substitution into the flux law gives

$$
\boxed{
F_{\max}=C_0k
\left(\frac{g\alpha}
{\operatorname{Ra}_c\nu\kappa}\right)^{1/3}
(T_w-T_m)^{5/3}},
$$

where

$$
C_0=\frac85\left(\frac{16}{25}\right)^{1/3}.
$$

Thus the proportionality coefficient depends on the [thermal conductivity](../../../thermodynamics.md#thermal-conductivity), nonlinear thermal-expansion coefficient $\alpha$, [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity), [thermal diffusivity](../../../thermodynamics.md#thermal-diffusivity), gravity, and critical [Rayleigh number](../../../geophysics.md#rayleigh-number). This is the maximum-flux law for [penetrative convection in an ice-covered lake](../../../geophysics.md#penetrative-convection-in-an-ice-covered-lake).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

The stagnant layer transports [heat](../../../thermodynamics.md#heat) by [thermal conduction](../../../thermodynamics.md#thermal-conduction), so its upward [heat flux](../../../thermodynamics.md#heat-flux-density) is

$$
F_s=\frac{k(T_h-T_s)}h.
$$

At the maximum-flux interface from part iii,

$$
T_h-T_s=(T_m-T_s)-\frac35(T_w-T_m).
$$

Equating $F_s$ to $F_{\max}$ gives

$$
\boxed{
h=\frac1{C_0}
\left(\frac{\operatorname{Ra}_c\nu\kappa}{g\alpha}\right)^{1/3}
\frac{(T_m-T_s)-\frac35(T_w-T_m)}
{(T_w-T_m)^{5/3}}}.
$$

The stagnant layer has positive thickness only if

$$
T_w<T_m+\frac53(T_m-T_s).
$$

For an ice-covered freshwater lake, take $T_s\simeq0\,{}^\circ\mathrm C$ and $T_m\simeq4\,{}^\circ\mathrm C$. The largest interior temperature compatible with this [penetrative convection in an ice-covered lake](../../../geophysics.md#penetrative-convection-in-an-ice-covered-lake) model is therefore

$$
\boxed{T_{w,\max}\simeq4+\frac53(4)
=10.7\,{}^\circ\mathrm C}.
$$

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

Define the dimensionless stagnant-layer depth and time by

$$
\eta=\frac hH,
\qquad
\tau=\frac{\kappa t}{H^2},
$$

so $H^2/\kappa$ is the [thermal diffusion time](../../../thermodynamics.md#thermal-diffusion-time). The maximizing interface temperature gives

$$
T_h-T_s=\Delta T\left(1-\frac35\theta\right).
$$

Equating conductive and convective [heat fluxes](../../../thermodynamics.md#heat-flux-density) therefore gives the algebraic relation

$$
\boxed{
\frac{1-3\theta/5}{\eta}
=\mathcal F\theta^{5/3}}.
$$

Since $k=\rho c_p\kappa$, where $c_p$ is the [specific heat capacity](../../../thermodynamics.md#specific-heat-capacity), the bulk heat balance in the convecting depth $H-h$ becomes

$$
\boxed{
(1-\eta)\frac{d\theta}{d\tau}
=-\mathcal F\theta^{5/3}}.
$$

Retaining the heat capacity of the thin stagnant layer changes this only by relative order $\eta$.

For $\mathcal F\gg1$ and $\theta=O(1)$, the flux relation gives $\eta=O(\mathcal F^{-1})$. The leading equation is consequently

$$
\frac{d\theta}{d\tau}
=-\mathcal F\theta^{5/3}.
$$

Separating variables and using $\theta(0)=1$ gives

$$
\theta^{-2/3}=1+\frac23\mathcal F\tau,
$$

hence

$$
\boxed{
\theta(\tau)=
\left(1+\frac23\mathcal F\tau\right)^{-3/2}}.
$$

<h3 id="2/vi">vi</h3>

↑ **Parent:** [2](#2)

<h4 id="2/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#2/vi)

The approximation in part v requires the dimensionless stagnant depth

$$
\eta=
\frac{1-3\theta/5}
{\mathcal F\theta^{5/3}}
$$

to remain small. Since $0<\theta\leq1$ makes the numerator order one, this condition is

$$
\boxed{\theta\gg\mathcal F^{-3/5}}.
$$

Using the solution from part v, the equivalent time range is

$$
1+\frac23\mathcal F\tau
\ll\mathcal F^{2/5},
$$

or, at the level of [asymptotic equivalence](../../../real-analysis.md#asymptotic-equivalence),

$$
\boxed{0\leq\tau\ll\mathcal F^{-3/5}}.
$$

The cooling becomes appreciable on the shorter scale $\tau=O(\mathcal F^{-1})$, so these ranges overlap widely when $\mathcal F\gg1$.

The [Rayleigh number](../../../geophysics.md#rayleigh-number) based on the convecting depth is

$$
\operatorname{Ra}
=\frac{g\alpha(T_w-T_m)^2(H-h)^3}{\nu\kappa}.
$$

The definition of $\mathcal F$ implicit in part iii gives

$$
\mathcal F
=C_0H
\left(\frac{g\alpha\Delta T^2}
{\operatorname{Ra}_c\nu\kappa}\right)^{1/3}.
$$

It follows that

$$
\boxed{
\operatorname{Ra}
=\operatorname{Ra}_c
\left(\frac{\mathcal F}{C_0}\right)^3
\theta^2(1-\eta)^3}.
$$

If $1-\eta=O(1)$ and $\theta\gg\mathcal F^{-3/5}$, then $\operatorname{Ra}\gg O(\mathcal F^{9/5})$. The [thermal convection](../../../fluid-mechanics.md#thermal-convection) therefore remains strongly supercritical throughout the range in which the thin stagnant-layer approximation is valid.

## 3

↑ **Parent:** [Paper 332](paper-332.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $d(z,t)$ be the local water-film thickness. To first order in the interface amplitudes,

$$
d=h+(\eta_2-\eta_1)e^{i\alpha z+\sigma t}.
$$

The [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) flux down the vertical surface, with a [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) at the ice and a [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition) at the water-air interface, is

$$
q=\frac{d^3}{3\nu}
\left(g-\frac1\rho p_z\right).
$$

For the unperturbed film $p_z=0$, so

$$
q=\frac{gh^3}{3\nu},
\qquad
\boxed{h=\left(\frac{3\nu q}{g}\right)^{1/3}}.
$$

The linearized [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) gives the capillary-pressure perturbation

$$
p'=\gamma\alpha^2\eta_2e^{i\alpha z+\sigma t},
\qquad
p'_z=i\gamma\alpha^3\eta_2e^{i\alpha z+\sigma t}.
$$

Because the prescribed [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) is uniform, its first-order perturbation must vanish. [Linearization](../../../algebra.md#linearization) of the flux law gives

$$
0=\frac{gh^2}{\nu}(\eta_2-\eta_1)
-\frac{ih^3\gamma\alpha^3}{3\rho\nu}\eta_2.
$$

Thus, with $\Gamma=\gamma/(3\rho g)$,

$$
\eta_2(1-i\Gamma\alpha^3h)=\eta_1,
$$

and hence

$$
\boxed{
\eta_2=\frac{\eta_1}
{1-i\Gamma\alpha^3h}}.
$$

The complex amplitude ratio records the phase shift caused by [surface tension](../../../fluid-mechanics.md#surface-tension) in the [long-wave approximation](../../../viscous-fluid-flow.md#long-wave-approximation).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The unperturbed [temperature](../../../thermodynamics.md#temperature) is linear in each material. Continuity of the conductive [heat flux](../../../thermodynamics.md#heat-flux-density) at $x=h$ gives

$$
k_w\frac{T_m-T_h}{h}
=k_a\frac{T_h-T_a}{\delta}.
$$

On defining

$$
\epsilon=\frac{k_a}{k_w}\frac h\delta,
$$

this becomes $T_m-T_h=\epsilon(T_h-T_a)$. Therefore

$$
\boxed{
T_m-T_h=
\frac{\epsilon}{1+\epsilon}(T_m-T_a)}.
$$

Let $\rho_i$ be the ice [mass density](../../../fluid-mechanics.md#density) and $L_f$ its [latent heat](../../../thermodynamics.md#latent-heat) of fusion per unit mass. The ice is isothermal in this model, so the [Stefan condition](../../../geophysics.md#stefan-condition) equates latent-heat production to the [heat flux](../../../thermodynamics.md#heat-flux-density) conducted through the water:

$$
\rho_iL_fV
=k_w\frac{T_m-T_h}{h}.
$$

Consequently the unperturbed lateral solidification speed is

$$
\boxed{
V=\frac{k_w}{\rho_iL_fh}
\frac{\epsilon}{1+\epsilon}(T_m-T_a)
=\frac{k_a}{\rho_iL_f\delta}
\frac{T_m-T_a}{1+\epsilon}}.
$$

The material parameters are the [thermal conductivities](../../../thermodynamics.md#thermal-conductivity) $k_w,k_a$, ice density $\rho_i$, and specific latent heat $L_f$; the geometric thermal length is $\delta$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Write the base-state gradients as

$$
G_w=\frac{T_h-T_m}{h},
\qquad
G_a=\frac{T_a-T_h}{\delta}.
$$

The base [heat flux](../../../thermodynamics.md#heat-flux-density) and [Stefan condition](../../../geophysics.md#stefan-condition) relations are

$$
k_wG_w=k_aG_a,
\qquad
-k_wG_w=\rho_iL_fV.
$$

Under the [quasi-stationary approximation](../../../mathematics.md#quasi-steady-approximation), and with advective heat transport neglected, each temperature perturbation satisfies the [Laplace equation](../../../partial-differential-equation.md#laplace-equation). The decaying normal-mode solutions are

$$
\widehat T_w=A\cosh(\alpha x)+B\sinh(\alpha x),
\qquad
\widehat T_a=Ce^{-\alpha(x-h)}.
$$

Keeping the displaced ice interface at $T_m$ omits the curvature correction described by the [Gibbs--Thomson relation](../../../fluid-mechanics.md#gibbs-thomson-relation).  
The fixed melting temperature at the displaced ice interface gives

$$
A=-\eta_1G_w.
$$

Expanding temperature and conductive [heat flux](../../../thermodynamics.md#heat-flux-density) continuity at the displaced outer interface gives

$$
A\cosh(\alpha h)+B\sinh(\alpha h)-C
=\eta_2(G_a-G_w),
$$



$$
k_w\left[A\sinh(\alpha h)+B\cosh(\alpha h)\right]
=-k_aC.
$$

Put $r=k_a/k_w$. Since $G_a=G_w/r$, the temperature condition in the limits $r\ll1$ and $\alpha h\ll1$ gives

$$
C\sim-\frac{\eta_2G_w}{r}.
$$

Although $r$ is small, the product $rC$ is therefore order one and cannot be discarded. The flux condition then gives

$$
B=-rC-A\alpha h+o(1)
\sim\eta_2G_w.
$$

This is why the stated asymptotic warning matters.

The perturbed [Stefan condition](../../../geophysics.md#stefan-condition) at $x=0$ is

$$
\rho_iL_f\sigma\eta_1
=-k_w\widehat T_w'(0)
=-k_w\alpha B.
$$

Using $B\sim\eta_2G_w$ and $-k_wG_w=\rho_iL_fV$ yields

$$
\sigma\eta_1=V\alpha\eta_2.
$$

Substitution of the interface-amplitude ratio from part i produces the [thin-film icicle-ripple instability](../../../geophysics.md#thin-film-icicle-ripple-instability) [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{
\frac{h\sigma}{V}
=\frac{\alpha h}{1-i\Gamma\alpha^3h}}.
$$

Set $b=\Gamma h\alpha^3$. Rationalizing this [complex number](../../../complex-analysis.md#complex-number) gives

$$
\sigma=\frac{V\alpha(1+ib)}{1+b^2},
$$

so its [growth rate](../../../wave-equation.md#growth-rate) and [imaginary part](../../../complex-analysis.md#imaginary-part) are

$$
\operatorname{Re}\sigma
=\frac{V\alpha}{1+(\Gamma h)^2\alpha^6},
\qquad
\operatorname{Im}\sigma
=\frac{V\alpha b}{1+b^2}.
$$

Differentiating the growth rate with respect to the [wavenumber](../../../wave-equation.md#wavenumber) shows that its positive [stationary point](../../../calculus-of-variations.md#stationary-point) satisfies

$$
1-5(\Gamma h)^2\alpha_m^6=0.
$$

It is the unique [global maximum](../../../function.md#global-maximum), and hence

$$
\boxed{
\alpha_m=5^{-1/6}(\Gamma h)^{-1/3}}.
$$

At this wavenumber $b=1/\sqrt5$. With the convention $e^{i\alpha z+\sigma t}$, a constant phase travels with [phase velocity](../../../wave-equation.md#phase-velocity)

$$
c_p=-\frac{\operatorname{Im}\sigma}{\alpha}
=-\frac{Vb}{1+b^2}.
$$

Therefore

$$
\boxed{c_p=-\frac{\sqrt5}{6}V}.
$$

Because $z$ increases downward, the negative sign means that the [icicle ripples](../../../geophysics.md#icicle-ripple) migrate upward with speed $\sqrt5V/6$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
