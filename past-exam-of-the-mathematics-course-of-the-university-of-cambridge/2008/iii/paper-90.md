# Paper 90

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper90.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper90.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 90](paper-90.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Assume the [shallow-water approximation](../../../physics.md#shallow-water-approximation): the horizontal scale is long compared with the depth, the [hydrostatic approximation](../../../fluid-mechanics.md#hydrostatic-approximation) applies, and the cross-section-averaged [velocity](../../../classical-mechanics.md#velocity) is approximately uniform. Neglect viscosity and drag for this part. [Volume conservation](../../../physics.md#volume-conservation) gives the constant discharge $Q=bhu$. The steady horizontal momentum equation is

$$
u u_x=-g(H+h)_x,
$$

so its integral is the [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) head $\mathcal H=H+h+u^2/(2g)$. The [shallow-water specific energy](../../../physics.md#shallow-water-specific-energy) measured above the bed is therefore

$$
\boxed{E(h;Q,b)=h+\frac{Q^2}{2gb^2h^2},\qquad E+H=\mathcal H.}
$$

The [Froude number](../../../reduced-gravity.md#froude-number) compares the flow [velocity](../../../classical-mechanics.md#velocity) with the long-wave speed $\sqrt{gh}$:

$$
\boxed{F=\frac{u}{\sqrt{gh}},\qquad E=h\left(1+\frac{F^2}{2}\right),\qquad
\left.\frac{\partial E}{\partial h}\right|_{Q,b}=1-F^2.}
$$

At fixed $Q,b$, the [shallow-water specific energy](../../../physics.md#shallow-water-specific-energy) tends to infinity as $h$ tends to zero or infinity. Its unique minimum occurs at the critical depth

$$
h_c=\left(\frac{Q^2}{gb^2}\right)^{1/3},\qquad F=1,\qquad E_c=\frac32h_c.
$$

The two depth branches above that minimum are [subcritical flow](../../../reduced-gravity.md#subcritical-flow), $F<1$ with $h>h_c$, and [supercritical flow](../../../reduced-gravity.md#supercritical-flow), $F>1$ with $h<h_c$. The long-wave [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed) relative to the bed are $u\pm\sqrt{gh}$. Thus a [subcritical flow](../../../reduced-gravity.md#subcritical-flow) can receive information from downstream, whereas both [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) travel downstream in a positive [supercritical flow](../../../reduced-gravity.md#supercritical-flow).

A [hydraulic control](../../../reduced-gravity.md#hydraulic-control) is a critical section where one [characteristic speed](../../../partial-differential-equation.md#characteristic-speed) vanishes and a smooth flow can pass between the two branches. Regularity there supplies a condition relating $Q$, the depth and the geometry; together with reservoir or inlet data, it can determine the discharge. Merely finding $F=1$ is not enough: a finite depth gradient also requires the geometric forcing to vanish in the critical momentum equation.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Differentiate the [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) at fixed discharge, using $u_x/u=-b_x/b-h_x/h$. This gives

$$
(1-F^2)h_x=F^2h\frac{b_x}{b}-H_x.
$$

At a smooth [hydraulic control](../../../reduced-gravity.md#hydraulic-control), $F=1$ and the right-hand side must vanish. For the specified geometry,

$$
-2\eta x_c=h_c\frac{2\beta(x_c-a)}{1+\beta(x_c-a)^2},\qquad
\boxed{h_c=\frac{\eta x_c[1+\beta(x_c-a)^2]}{\beta(a-x_c)}.}
$$

For the intended positive parameters $\beta,\eta,a>0$, positive finite depth requires

$$
\boxed{0<x_c<a.}
$$

The control lies between the bed summit and the width minimum, rather than necessarily at either one. For $a<0$ the corresponding interval is $a<x_c<0$. If $a=0$, the coincident summit and throat admit $x_c=0$ without imposing a depth through this first-derivative relation. The limiting cases $\beta=0$ or $\eta=0$ must be handled before division: their control is at the bed summit or throat, respectively.

At $x_c=a/2$, the critical-depth formula simplifies to

$$
\boxed{h_c=\frac{\eta}{\beta}\left(1+\frac{\beta a^2}{4}\right),\qquad
Q=b(x_c)\sqrt{g h_c^3}.}
$$

This establishes the requested depth without assuming that the bed summit and throat coincide.

There is a further regularity qualification if a critical candidate is to be a simple, smooth transcritical [hydraulic control](../../../reduced-gravity.md#hydraulic-control). At fixed $Q$, define the critical-head envelope

$$
T(x)=H(x)+\frac32\left(\frac{Q^2}{gb(x)^2}\right)^{1/3}.
$$

Real depths require $\mathcal H\ge T(x)$. At a control $\mathcal H=T(x_c)$, so $T$ must have a local maximum, not a local minimum. The first condition $T_x=0$ is precisely the compatibility equation above, and

$$
T_{xx}=H_{xx}-h_c\left[\frac{b_{xx}}b-\frac53\left(\frac{b_x}b\right)^2\right].
$$

For the positive-parameter case, a nondegenerate control therefore additionally satisfies

$$
\boxed{3a+\beta(a-x_c)^2(3a-10x_c)>0.}
$$

Indeed $T_{xx}=-2\eta[3a+\beta(a-x_c)^2(3a-10x_c)]/[3(a-x_c)b(x_c)]$. The interval $0<x_c<a$ gives all positive-depth candidates, while this inequality excludes candidates with no smooth critical crossing. At $a/2$ it becomes $\beta a^2<6$ for a simple control; the requested depth relation remains necessary whenever such a control exists. Equality is a degenerate critical point requiring higher-order analysis. For example, $a=1$, $\beta=16$ makes the midpoint a local minimum of $T$, so positivity of the depth alone would incorrectly identify it as a regular control.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Model the specified drag by a prescribed head loss, $(E+H)_x=-\gamma$. A modified conserved head is consequently

$$
\boxed{\mathcal E_\gamma=H+h+\frac{Q^2}{2gb^2h^2}+\gamma x,}
$$

with an arbitrary reference constant absorbed into $\mathcal E_\gamma$. More generally the last term is $\int_0^x\gamma(s)\,ds$. The effective bed elevation for the [shallow-water specific energy](../../../physics.md#shallow-water-specific-energy) calculation is $H+\gamma x$. The critical momentum equation becomes

$$
(1-F^2)h_x=F^2h\frac{b_x}b-H_x-\gamma.
$$

This is the [head-loss correction to hydraulic control](../../../reduced-gravity.md#head-loss-correction-to-hydraulic-control).

When $\beta=0$, $b=1$, and regularity at $F=1$ gives $-2\eta x_c+\gamma=0$. Therefore, for $\eta,\gamma>0$,

$$
\boxed{x_c=\frac{\gamma}{2\eta}.}
$$

The effective bed $-\eta x^2+\gamma x$ has a strict maximum there, with elevation increment $\Delta=\gamma^2/(4\eta)$ relative to $x=0$.

Let $d=h(0)$ and require $h_c=2d$. At the control $Q^2=g h_c^3=8gd^3$. At $x=0$ the [shallow-water specific energy](../../../physics.md#shallow-water-specific-energy) is $d+Q^2/(2gd^2)=5d$, while at the control it is $3h_c/2=3d$. Equality of the modified head gives $5d=3d+\Delta$. Hence

$$
\boxed{h(0)=\frac{\gamma^2}{8\eta},\qquad h_c=\frac{\gamma^2}{4\eta},\qquad
Q=\sqrt g\left(\frac{\gamma^2}{4\eta}\right)^{3/2}=\frac{\sqrt g\,\gamma^3}{8\eta^{3/2}}.}
$$

The inlet has $F(0)^2=8$ and is [supercritical flow](../../../reduced-gravity.md#supercritical-flow); the branch whose depth increases into the control makes the required smooth transition. At the control the increasing branch has slope $h_x=\sqrt{2\eta h_c/3}$, as follows by expanding the modified head to second order.

The numerical discharge uses a constant loss rate on the entire segment from $0$ to $x_c$. The wording specifies that rate only near the control, which is sufficient to locate $x_c$ but does not by itself determine the inlet-to-control head loss. If the loss elsewhere is unspecified, write $\Lambda_c=\int_0^{x_c}\gamma(s)\,ds$. The same calculation gives $h_c=H(x_c)-H(0)+\Lambda_c$ and $Q=\sqrt g\,h_c^{3/2}$; the boxed value is the constant-loss specialization.

## 2

↑ **Parent:** [Paper 90](paper-90.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [shallow-water approximation](../../../physics.md#shallow-water-approximation) assumes a horizontal length scale $\ell$ much greater than the current depth, $h/\ell\ll1$. Vertical acceleration is then small compared with gravity and pressure is given by the [hydrostatic approximation](../../../fluid-mechanics.md#hydrostatic-approximation). A depth-averaged model also assumes that the horizontal [velocity](../../../classical-mechanics.md#velocity) and excess [mass density](../../../fluid-mechanics.md#density) can be represented by nearly uniform cross-sectional values. Here the ambient fluid is deep or sufficiently undisturbed that its motion and interface-pressure perturbations can be neglected.

The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) assumes $|\rho-\rho_0|/\rho_0\ll1$: [mass density](../../../fluid-mechanics.md#density) differences are retained in gravitational forces but a common reference [mass density](../../../fluid-mechanics.md#density) is used for inertia. A dense bottom current has the positive [reduced gravity](../../../reduced-gravity.md)

$$
\boxed{g'=g\frac{\rho-\rho_0}{\rho_0}>0.}
$$

Thus the pressure excess over the ambient hydrostatic value at height $z$ within the current is $\rho_0g'(h-z)$. We neglect bed drag, molecular diffusion and horizontal turbulent stress in the leading balances, but retain the prescribed turbulent [entrainment](../../../fluid-mechanics.md#fluid-entrainment) across the interface. Negligible bed drag does not imply that [entrainment](../../../fluid-mechanics.md#fluid-entrainment) has no effect on the current's [velocity](../../../classical-mechanics.md#velocity) or [mass density](../../../fluid-mechanics.md#density).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The occupied cross-sectional area and interface width are

$$
A(h)=\int_0^h z\,dz=\frac{h^2}{2},\qquad b(h)=h.
$$

The incoming [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) per unit channel length is $hw_e$. [Volume conservation](../../../physics.md#volume-conservation) therefore gives $A_t+(Au)_x=hw_e$. Ambient fluid carries no excess [mass density](../../../fluid-mechanics.md#density), so integrating the excess-[mass density](../../../fluid-mechanics.md#density) balance gives $(Ag')_t+(Aug')_x=0$. These two equations imply dilution of the [reduced gravity](../../../reduced-gravity.md), even though total integrated [buoyancy](../../../fluid-mechanics.md#buoyancy) is conserved.

The integrated horizontal [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) force, divided by the reference [mass density](../../../fluid-mechanics.md#density), is

$$
\int_0^h g'(h-z)z\,dz=\frac{g'h^3}{6}.
$$

The prismatic walls contribute no axial component of pressure force. Since ambient fluid enters with zero horizontal [velocity](../../../classical-mechanics.md#velocity), it supplies no horizontal [momentum flux](../../../physics.md#momentum-flux). Thus the [entraining shallow-water current in a triangular channel](../../../reduced-gravity.md#entraining-shallow-water-current-in-a-triangular-channel) obeys the conservative equations

$$
\boxed{
\begin{aligned}
\partial_t\left(\frac{h^2}{2}\right)+\partial_x\left(\frac{h^2u}{2}\right)&=hw_e,\\
\partial_t\left(\frac{h^2u}{2}\right)+\partial_x\left(\frac{h^2u^2}{2}+\frac{g'h^3}{6}\right)&=0,\\
\partial_t\left(\frac{h^2g'}{2}\right)+\partial_x\left(\frac{h^2ug'}{2}\right)&=0.
\end{aligned}}
$$

To put them in primitive form, let $D=\partial_t+u\partial_x$ be the [material derivative](../../../continuum-mechanics.md#material-derivative). The volume equation gives $Dh+(h/2)u_x=w_e$. Subtracting $u$ times the volume equation from the momentum equation, and $g'$ times it from the [buoyancy](../../../fluid-mechanics.md#buoyancy) equation, yields

$$
\boxed{
\begin{aligned}
Dh+\frac h2u_x&=w_e,\\
Du+g'h_x+\frac h3g'_x&=-\frac{2uw_e}{h},\\
Dg'&=-\frac{2g'w_e}{h}.
\end{aligned}}
$$

The momentum source is the acceleration of newly entrained ambient fluid, not bed drag. The source in the [reduced gravity](../../../reduced-gravity.md) equation describes mixing with ambient fluid of zero excess [mass density](../../../fluid-mechanics.md#density). In particular, the rectangular-channel coefficients cannot be used: the triangular area produces both $h/2$ in the depth equation and $h/3$ in the [buoyancy](../../../fluid-mechanics.md#buoyancy)-gradient force.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the state vector $q=(h,u,g')^T$, the primitive equations are $q_t+\mathsf A q_x=S$, with

$$
\mathsf A=\begin{pmatrix}u&h/2&0\\g'&u&h/3\\0&0&u\end{pmatrix},\qquad
S=\begin{pmatrix}w_e\\-2uw_e/h\\-2g'w_e/h\end{pmatrix}.
$$

The [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is

$$
\det(\mathsf A-\lambda I)=(u-\lambda)\left[(u-\lambda)^2-\frac{g'h}{2}\right].
$$

Consequently the three [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed) are

$$
\boxed{\frac{dx}{dt}=u,\quad u+c,\quad u-c,\qquad c=\sqrt{\frac{g'h}{2}}.}
$$

For $h>0$ and $g'>0$, the [hyperbolic system](../../../partial-differential-equation.md#hyperbolic-system) has three distinct real [eigenvalues](../../../linear-operator-theory.md#eigenvalue). The long-wave speed relative to the current is $c$, while $u$ transports a [buoyancy](../../../fluid-mechanics.md#buoyancy)/contact disturbance.

A left [eigenvector](../../../linear-operator-theory.md#eigenvector) for the material characteristic is $(0,0,1)$, giving

$$
\boxed{\frac{dg'}{dt}=-\frac{2g'w_e}{h}\quad\text{along}\quad\frac{dx}{dt}=u.}
$$

For $u\pm c$, left [eigenvectors](../../../linear-operator-theory.md#eigenvector) can be chosen as

$$
\ell_\pm=\left(\pm\frac{2c}{h},1,\pm\frac{h}{3c}\right).
$$

Multiplying $q_t+\mathsf A q_x=S$ by these rows gives the [characteristic compatibility for an entraining triangular-channel current](../../../reduced-gravity.md#characteristic-compatibility-for-an-entraining-triangular-channel-current). With all differentials evaluated along the indicated characteristic,

$$
\boxed{du\pm\frac{2c}{h}\,dh\pm\frac{h}{3c}\,dg'
=-\frac{2w_e}{h}\left(u\mp\frac c3\right)dt,
\qquad \frac{dx}{dt}=u\pm c.}
$$

The source follows directly from $\ell_\pm S=-2uw_e/h\pm2cw_e/h\mp2g'w_e/(3c)$ and $g'/c=2c/h$.

Since $4\,dc=(2c/h)dh+(h/c)dg'$, an equivalent form is

$$
d(u\pm4c)\mp\frac{4c}{3g'}\,dg'
=-\frac{2w_e}{h}\left(u\mp\frac c3\right)dt.
$$

Combining it with the material [buoyancy](../../../fluid-mechanics.md#buoyancy) equation also gives

$$
D_\pm(u\pm4c)=\frac{2h}{3}g'_x-\frac{2w_e}{h}(u\pm c),\qquad
D_\pm=\partial_t+(u\pm c)\partial_x.
$$

Only when [entrainment](../../../fluid-mechanics.md#fluid-entrainment) vanishes and $g'$ is spatially constant do $u\pm4c$ become constant [Riemann invariants](../../../compressible-flow.md#riemann-invariant) on these [characteristic curves](../../../partial-differential-equation.md#characteristic-curve). Dropping the [buoyancy](../../../fluid-mechanics.md#buoyancy) differential in the general problem would lose one of the required transport couplings. The characteristic formulas with $1/c$ apply to the nondegenerate region $g'h>0$; dry or neutrally buoyant limits require their conservative form instead.

## 3

↑ **Parent:** [Paper 90](paper-90.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Hindered settling](../../../fluid-mechanics.md#hindered-settling) is the reduction of the particle [settling velocity](../../../fluid-mechanics.md#settling-velocity) by displaced-fluid backflow and interactions with other particles. In the specified model, the downward speed is $V_s$ at vanishing [concentration](../../../physics.md#concentration) and falls to zero at the maximum packing fraction $\phi_{\max}$. The [characteristic speed](../../../partial-differential-equation.md#characteristic-speed) of a [concentration](../../../physics.md#concentration) disturbance will differ from this individual-particle speed.

Take $z$ positive upwards. For a locally uniform horizontal suspension without diffusion or bulk fluid motion, the upward particle flux is

$$
j(\phi)=-\phi V(\phi)=-V_s\phi+\frac{V_s}{\phi_{\max}}\phi^2.
$$

Particle [volume conservation](../../../physics.md#volume-conservation) gives the [scalar conservation law](../../../partial-differential-equation.md#scalar-conservation-law)

$$
\boxed{\phi_t+\partial_zj(\phi)=0,\qquad
\phi_t+\left(-V_s+\frac{2V_s\phi}{\phi_{\max}}\right)\phi_z=0.}
$$

This is the [quadratic hindered-settling flux](../../../fluid-mechanics.md#quadratic-hindered-settling-flux). Along its [characteristic curves](../../../partial-differential-equation.md#characteristic-curve),

$$
\boxed{\frac{d\phi}{dt}=0,\qquad\frac{dz}{dt}=c(\phi)=-V_s+\frac{2V_s\phi}{\phi_{\max}}.}
$$

For a smooth initial profile $\phi_0(\zeta)$, the map is $z=\zeta+c(\phi_0(\zeta))t$. Its Jacobian is $1+(2V_s/\phi_{\max})\phi_0'(\zeta)t$. A [shock](../../../partial-differential-equation.md#shock-wave) develops where this first reaches zero: the compressive condition is $\phi_0'<0$, and

$$
t_s=-\frac{\phi_{\max}}{2V_s\min_\zeta\phi_0'(\zeta)}
$$

when the minimum is negative and no earlier boundary discontinuity is imposed. A discontinuous compressive initial state can instead contain a [shock](../../../partial-differential-equation.md#shock-wave) from $t=0$.

Let $z=s(t)$ separate states $\phi_L$ below the [shock](../../../partial-differential-equation.md#shock-wave) and $\phi_R$ above it. Integrating the [conservation law](../../../physics.md#conservation-law) across a moving thin interval gives the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions)

$$
\dot s(\phi_R-\phi_L)=j(\phi_R)-j(\phi_L).
$$

Equivalently, the flux relative to the [shock](../../../partial-differential-equation.md#shock-wave) agrees on both sides. For this quadratic flux,

$$
\boxed{\dot s=-V_s+\frac{V_s}{\phi_{\max}}(\phi_L+\phi_R)
=\frac{c(\phi_L)+c(\phi_R)}2.}
$$

Since $j''=2V_s/\phi_{\max}>0$, a physical compression [shock](../../../partial-differential-equation.md#shock-wave) has $\phi_L>\phi_R$ and satisfies $c(\phi_L)>\dot s>c(\phi_R)$: [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) enter it from both sides. These conditions select the [shock](../../../partial-differential-equation.md#shock-wave) over a nonphysical expansive discontinuity.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the upward coordinate of the preceding [kinematic sedimentation](../../../fluid-mechanics.md#kinematic-sedimentation) calculation, with the given smooth profile on $0\le\zeta\le h$ and clear fluid above. This asks for the first characteristic breaking of that profile; a separately imposed packed-bed discontinuity would be a different boundary problem.

Substitution of the initial [concentration](../../../physics.md#concentration) into the [characteristic speed](../../../partial-differential-equation.md#characteristic-speed) gives

$$
c_0(\zeta)=-\frac{V_s}{3}-\frac{2V_s\zeta^2}{3h^2},\qquad
z(\zeta,t)=\zeta+c_0(\zeta)t.
$$

The characteristic Jacobian is

$$
\frac{\partial z}{\partial\zeta}=1-\frac{4V_s\zeta t}{3h^2}.
$$

It first vanishes at the upper edge $\zeta=h$. That edge has zero [concentration](../../../physics.md#concentration) and descends initially at $V_s$, so

$$
\boxed{t_s=\frac{3h}{4V_s},\qquad z_s=h-V_st_s=\frac h4.}
$$

Although the derivative of the initial profile jumps to zero in the clear region, the [concentration](../../../physics.md#concentration) itself is continuous there. The [shock](../../../partial-differential-equation.md#shock-wave) starts with vanishing amplitude. Both limiting concentrations at onset are zero, and the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions) consequently gives

$$
\boxed{\dot s(t_s^+)=-V_s.}
$$

This is a downward speed $V_s$.

After formation the upper state remains clear, $\phi_R=0$, and the lower state is positive. The [parabolic-profile sedimentation shock](../../../fluid-mechanics.md#parabolic-profile-sedimentation-shock) has

$$
\dot s=-V_s\left(1-\frac{\phi_L}{\phi_{\max}}\right).
$$

It therefore initially slows down in magnitude: its signed upward-coordinate speed increases from $-V_s$. One can also verify that its captured left state increases. Write $r=\zeta_L/h$, where $\zeta_L$ labels the incident lower characteristic. Conservation of the particle volume initially above that characteristic gives

$$
\frac{V_s t}{\phi_{\max}}\phi_0(\zeta_L)^2=\int_{\zeta_L}^h\phi_0(\zeta)\,d\zeta,
\qquad
\frac{V_st}{h}=\frac{r+2}{(r+1)^2}.
$$

The derivative of the right-hand side with respect to $r$ is $-(r+3)/(r+1)^3<0$. Thus $r$ decreases as time increases, and $\phi_L=\phi_{\max}(1-r^2)/3$ increases. The downward [shock](../../../partial-differential-equation.md#shock-wave) speed continues to decrease on this branch until a bed or another boundary interacts with it. No later boundary behavior is needed for the requested conclusion.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Assume the carrier fluid has ambient [mass density](../../../fluid-mechanics.md#density) $\rho_0$, the particles have [mass density](../../../fluid-mechanics.md#density) $\rho_p>\rho_0$, and volumes add. The well-mixed current then has

$$
\boxed{\rho=(1-\phi)\rho_0+\phi\rho_p,\qquad
g'=g\frac{\rho-\rho_0}{\rho_0}=g_0'\phi,\qquad
g_0'=g\frac{\rho_p-\rho_0}{\rho_0}.}
$$

Here $g_0'$ is the particle-fluid reference [reduced gravity](../../../reduced-gravity.md) per unit volume fraction, which is the convention needed in the requested expansion. The initial current [reduced gravity](../../../reduced-gravity.md) is $g_0'\phi_0$; it should not be confused with $g_0'$ itself. The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) requires $\phi(\rho_p-\rho_0)/\rho_0\ll1$.

For particles to remain well mixed, the turbulent vertical mixing time must be short compared with the settling time. In a [turbulent diffusion](../../../turbulence.md#eddy-diffusion) description with diffusivity $K_z$, require $h^2/K_z\ll h/[V_s(1-\phi)]$, or $K_z\gg hV_s(1-\phi)$. Equivalently, characteristic turbulent vertical speeds should substantially exceed the particle [settling velocity](../../../fluid-mechanics.md#settling-velocity). [Turbulence](../../../turbulence.md) can maintain an approximately uniform [concentration](../../../physics.md#concentration) in the body while particles still settle relative to the fluid. At the impermeable bed, fluid has no normal transport into the solid boundary, but particles can reach and be captured by it. Assume no resuspension after capture.

Use a [gravity-current box model](../../../reduced-gravity.md#gravity-current-box-model) of length $L(t)$, uniform depth $h(t)$ and uniform [concentration](../../../physics.md#concentration) $\phi(t)$. Neglect ambient [entrainment](../../../fluid-mechanics.md#fluid-entrainment) and the small volume change caused by depositing dilute solids, so $Lh=M$ remains constant. Take a constant front [Froude number](../../../reduced-gravity.md#froude-number) $F>0$ and the [gravity-current front condition](../../../reduced-gravity.md#gravity-current-front-condition) $\dot L=F\sqrt{g'h}$. With $\phi_{\max}=1$, the deposition flux is $V_s\phi(1-\phi)$ per unit bed area. The particle-volume budget is

$$
\frac{d}{dt}(M\phi)=-LV_s\phi(1-\phi).
$$

Hence the integral model is

$$
\boxed{h=\frac ML,\qquad
\dot L=F\sqrt{\frac{g_0'M\phi}{L}},\qquad
\dot\phi=-\frac{V_sL}{M}\phi(1-\phi),\qquad
L(0)=L_0,\quad\phi(0)=\phi_0.}
$$

The model assumes a fixed rear boundary, one advancing front, a deep stationary ambient, negligible drag during the inertial spreading regime, and a perfectly absorbing bed. The supplied hindered-settling law is retained in the deposition closure.

For $0<\phi<1$, eliminating time gives

$$
\frac{d\phi}{\sqrt\phi(1-\phi)}=-\frac{V_s}{F\sqrt{g_0'}M^{3/2}}L^{3/2}\,dL.
$$

The [concentration](../../../physics.md#concentration) integral is $2\operatorname{artanh}\sqrt\phi$. Therefore

$$
L^{5/2}=L_0^{5/2}+\frac{5FM^{3/2}\sqrt{g_0'}}{V_s}
\left(\operatorname{artanh}\sqrt{\phi_0}-\operatorname{artanh}\sqrt\phi\right).
$$

As the particle [concentration](../../../physics.md#concentration) tends to zero, the current [reduced gravity](../../../reduced-gravity.md) and front speed tend to zero. The [hindered-settling runout in a rectangular channel](../../../reduced-gravity.md#hindered-settling-runout-in-a-rectangular-channel) is

$$
\boxed{L_\infty=\left[L_0^{5/2}+\frac{5FM^{3/2}\sqrt{g_0'}}{V_s}
\operatorname{artanh}\sqrt{\phi_0}\right]^{2/5}.}
$$

It is a finite limiting distance; in this idealized model, the exponential tail of particle loss makes complete stopping asymptotic in time. For $L_\infty\gg L_0$, omit $L_0^{5/2}$. Using $\operatorname{artanh}x=x+x^3/3+O(x^5)$ gives

$$
\boxed{L_\infty^5\approx\frac{25F^2M^3g_0'}{V_s^2}
\left(\phi_0+\frac23\phi_0^2+O(\phi_0^3)\right).}
$$

The original PDF has $V_s^2$ in this expression; the TeX aid's $V_s^3$ is a transcription error. Dimensions independently confirm the square: $M^3g_0'/V_s^2$ has dimensions of length to the fifth power. If one instead names the initial current [reduced gravity](../../../reduced-gravity.md) $G_{\mathrm{init}}=g_0'\phi_0$, the same expansion is $25F^2M^3G_{\mathrm{init}}[1+2\phi_0/3+O(\phi_0^2)]/V_s^2$. Late loss of [turbulent mixing](../../../turbulence.md#turbulent-mixing), viscous resistance or bed resuspension can change the physical runout beyond this specified box model.

## 4

↑ **Parent:** [Paper 90](paper-90.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [entrainment coefficient](../../../turbulent-plume.md#entrainment-coefficient) $\alpha$ is the ratio of the inward ambient-fluid [velocity](../../../classical-mechanics.md#velocity) normal to a [buoyant plume](../../../fluid-mechanics.md#buoyant-plume) edge to the characteristic [buoyant plume](../../../fluid-mechanics.md#buoyant-plume) [velocity](../../../classical-mechanics.md#velocity). For an upward [buoyant plume](../../../fluid-mechanics.md#buoyant-plume), take $u_e=\alpha w>0$. There are two edges at half-width $b$, so the full-section volume source is $2u_e$. Dividing every integral balance by two gives consistent half-section equations.

For [top-hat plume](../../../turbulent-plume.md#top-hat-plume-model) profiles, [volume conservation](../../../physics.md#volume-conservation) and [mass conservation](../../../continuum-mechanics.md#mass-conservation) are

$$
\boxed{b_t+(bw)_z=\alpha w,\qquad
(\rho b)_t+(\rho bw)_z=\rho_0(z)\alpha w.}
$$

The mass entering the [buoyant plume](../../../fluid-mechanics.md#buoyant-plume) is ambient mass with local [mass density](../../../fluid-mechanics.md#density) $\rho_0(z)$. The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) uses a common reference [mass density](../../../fluid-mechanics.md#density) in inertia while retaining the [mass density](../../../fluid-mechanics.md#density) deficit in [buoyancy](../../../fluid-mechanics.md#buoyancy). The mass equation may be kept to the first order in that deficit to derive its transport.

Multiply the volume equation by the time-independent ambient [mass density](../../../fluid-mechanics.md#density). The product rule gives

$$
(\rho_0b)_t+(\rho_0bw)_z=\rho_0\alpha w+\rho_0'(z)bw.
$$

Subtract the mass equation and multiply by $g$. The [entrainment](../../../fluid-mechanics.md#fluid-entrainment) sources cancel exactly, leaving

$$
\boxed{\partial_t[(\rho_0-\rho)gb]+\partial_z[(\rho_0-\rho)gbw]
=g\rho_0'(z)bw=-\rho_0N^2bw,}
$$

where

$$
\boxed{N^2=-\frac{g}{\rho_0}\frac{d\rho_0}{dz}.}
$$

For stable [stratification](../../../gravity-wave.md#density-stratification), $\rho_0'<0$ and the [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency) $N$ is real. Rising fluid moves into lighter ambient fluid and loses its [mass density](../../../fluid-mechanics.md#density) deficit relative to that local ambient. Thus environmental [stratification](../../../gravity-wave.md#density-stratification) reduces the [buoyant plume](../../../fluid-mechanics.md#buoyant-plume)'s [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux), even though the ambient fluid entering by [entrainment](../../../fluid-mechanics.md#fluid-entrainment) contributes no [mass density](../../../fluid-mechanics.md#density) deficit at its own height.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Keep the half-section convention of part (a). Define the [mass density](../../../fluid-mechanics.md#density)-weighted [mass flux](../../../physics.md#mass-flux), [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) and [momentum flux](../../../physics.md#momentum-flux) by

$$
\boxed{Q=\rho bw,\qquad F=(\rho_0-\rho)gbw,\qquad M=\rho bw^2.}
$$

The full-section fluxes are $2Q,2F,2M$. These factors must be changed consistently if full fluxes are used; mixing a full-width flux with a half-width [entrainment](../../../fluid-mechanics.md#fluid-entrainment) source would introduce a spurious factor two.

For positive $Q,M$, $w=M/Q$, $\rho b=Q^2/M$, and $(\rho_0-\rho)gb=FQ/M$. The mass equation in part (a), the momentum equation, and the [buoyancy](../../../fluid-mechanics.md#buoyancy) equation therefore become

$$
\boxed{
\begin{aligned}
\partial_t(Q^2/M)+Q_z&=\rho_0\alpha M/Q,\\
Q_t+M_z&=FQ/M,\\
\partial_t(FQ/M)+F_z&=-\frac{\rho_0}{\rho}N^2Q.
\end{aligned}}
$$

These are direct algebraic rewritings with the [mass density](../../../fluid-mechanics.md#density) factors retained. In particular, $FQ/M$ is the [buoyancy](../../../fluid-mechanics.md#buoyancy) inventory per unit height as well as the integrated [buoyancy](../../../fluid-mechanics.md#buoyancy) force. If desired, $\rho$ can be reconstructed from $F/(gQ)=\rho_0/\rho-1$.

At leading [Boussinesq](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) order use a constant reference [mass density](../../../fluid-mechanics.md#density) $R$ in the inertial fluxes, $Q=Rbw$, $M=Rbw^2$, and write $g'=g(\rho_0-\rho)/R$ so $F=Rg'bw$. Set $\rho_0/\rho=1$ in the [stratification](../../../gravity-wave.md#density-stratification) source and use $N^2\simeq-g\rho_0'/R$. The [unsteady top-hat line-plume balances](../../../turbulent-plume.md#unsteady-top-hat-line-plume-balances) are then

$$
\boxed{\partial_t(Q^2/M)+Q_z=R\alpha M/Q,\qquad
Q_t+M_z=FQ/M,\qquad
\partial_t(FQ/M)+F_z=-N^2Q.}
$$

Equivalently the kinematic fluxes $q=Q/R=bw$, $m=M/R=bw^2$ and $f=F/R=g'bw$ obey the same equations with $R$ removed from the first source. This explicit distinction between [mass density](../../../fluid-mechanics.md#density)-weighted and kinematic fluxes fixes the normalization for the power-law solution.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

In a homogeneous ambient fluid, $N=0$ and $R=\rho_0$ is constant. Use kinematic fluxes or, equivalently, the primitive form of the [unsteady top-hat line-plume balances](../../../turbulent-plume.md#unsteady-top-hat-line-plume-balances):

$$
b_t+(bw)_z=\alpha w,\qquad
(bw)_t+(bw^2)_z=bg',\qquad
(bg')_t+(bg'w)_z=0.
$$

Here $g'=g(\rho_0-\rho)/R>0$ is the positive buoyant [reduced gravity](../../../reduced-gravity.md). Seek a nonsteady separable [power-law ansatz](../../../differential-equation.md#power-law-ansatz) with both time differentiation and vertical transport retained. Matching powers in the volume equation forces $b\propto z$ with no time dependence. Matching the two momentum terms then gives $w\propto z/\tau$, and the [buoyancy](../../../fluid-mechanics.md#buoyancy) force has $g'\propto z/\tau^2$, where $\tau=t+t_*>0$ is a shifted age. Thus write

$$
b=Bz,\qquad w=A\frac z\tau,\qquad g'=C\frac z{\tau^2}.
$$

Substitution determines the constants rather than just the exponents. The volume equation gives $2BA=\alpha A$, so for a nonzero [buoyant plume](../../../fluid-mechanics.md#buoyant-plume) $B=\alpha/2$. The momentum equation gives $C=-A+3A^2$, while the [buoyancy](../../../fluid-mechanics.md#buoyancy) equation gives $C(-2+3A)=0$. The buoyant nontrivial branch has $A=2/3$ and $C=2/3$. Consequently the [separable decaying top-hat line plume](../../../turbulent-plume.md#separable-decaying-top-hat-line-plume) is

$$
\boxed{b=\frac{\alpha z}{2},\qquad
w=\frac{2z}{3\tau},\qquad
g'=\frac{2z}{3\tau^2},\qquad
\rho=R\left(1-\frac{2z}{3g\tau^2}\right).}
$$

The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) requires $2z/(3g\tau^2)\ll1$. The corresponding [mass density](../../../fluid-mechanics.md#density)-weighted fluxes, to this order, are

$$
\boxed{Q=\frac{R\alpha z^2}{3\tau},\qquad
M=\frac{2R\alpha z^3}{9\tau^2},\qquad
F=\frac{2R\alpha z^3}{9\tau^3}.}
$$

For a direct check, $Q^2/M=R\alpha z/2$ is time independent and $FQ/M=R\alpha z^2/(3\tau^2)$. Hence $(Q^2/M)_t+Q_z=2R\alpha z/(3\tau)=R\alpha M/Q$, $Q_t+M_z=R\alpha z^2/(3\tau^2)=FQ/M$, and $(FQ/M)_t+F_z=0$. This verifies all three balances and the required width coefficient.

This nonsteady branch is not the steady, continuously supplied, constant-flux [line plume](../../../turbulent-plume.md#line-plume). The latter has constant $w$ and half-width $b=\alpha z$ in the same top-hat convention. Also, the unshifted [power law](../../../analysis.md#power-law) has $Q,F\to0$ as $z\to0$ and is singular at $\tau=0$. It is therefore an interior separable solution, not by itself a solution with a nonzero continuously operating point-source flux at the origin. A finite-width source boundary, a virtual origin, or a matching region is needed to connect it to physical source and initial data. For example, replacing $z$ by $z+z_*$ supplies a finite base width and time-varying positive base fluxes when $z_*>0$. No source or initial flux history is specified in the question to select that matching; the requested power-law width follows from the local balances above.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
