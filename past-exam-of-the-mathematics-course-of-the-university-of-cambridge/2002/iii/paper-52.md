# Paper 52

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper52.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper52.pdf)

**Table of contents**

- [Section A](#section-a)
  - [1](#1)
    - [a](#1/a)
      - [Solution](#1/a/solution)
    - [b](#1/b)
      - [Solution](#1/b/solution)
  - [2](#2)
    - [Solution](#2/solution)
- [Section B](#section-b)
  - [3](#3)
    - [a](#3/a)
      - [Solution](#3/a/solution)
    - [b](#3/b)
      - [Solution](#3/b/solution)
    - [c](#3/c)
      - [Solution](#3/c/solution)
    - [d](#3/d)
      - [Solution](#3/d/solution)
    - [e](#3/e)
      - [Solution](#3/e/solution)
  - [4](#4)
    - [a](#4/a)
      - [Solution](#4/a/solution)
    - [b](#4/b)
      - [Solution](#4/b/solution)
    - [c](#4/c)
      - [Solution](#4/c/solution)
- [Section C](#section-c)
  - [5](#5)
    - [a](#5/a)
      - [Solution](#5/a/solution)
    - [b](#5/b)
      - [Solution](#5/b/solution)
    - [c](#5/c)
      - [Solution](#5/c/solution)
    - [d](#5/d)
      - [Solution](#5/d/solution)
    - [e](#5/e)
      - [Solution](#5/e/solution)
  - [6](#6)
    - [a](#6/a)
      - [Solution](#6/a/solution)
    - [b](#6/b)
      - [Solution](#6/b/solution)
    - [c](#6/c)
      - [Solution](#6/c/solution)

## Section A

↑ **Parent:** [Paper 52](paper-52.md)

### 1

↑ **Parent:** [Section A](#section-a)

<h4 id="1/a">a</h4>

↑ **Parent:** [1](#1)

<h5 id="1/a/solution">Solution</h5>

↑ **Parent:** [A](#1/a)

Take $z$ increasing upwards and write $s=\phi/\phi_{\max}$. The particles have downward [settling velocity](../../../fluid-mechanics.md#settling-velocity); their upward [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) is $\phi V$. Conservation of particle volume in any interval gives

$$
\frac{d}{dt}\int_{z_1}^{z_2}\phi\,dz=\phi V(z_1,t)-\phi V(z_2,t).
$$

Thus the [kinematic sedimentation](../../../fluid-mechanics.md#kinematic-sedimentation) equation and its [characteristic speed](../../../partial-differential-equation.md#characteristic-speed) are

$$
\boxed{s_t+\partial_zf(s)=0,\qquad f(s)=-V_0s(1-s)^\alpha,}
$$



$$
a(s)=f'(s)=-V_0(1-s)^{\alpha-1}\bigl[1-(\alpha+1)s\bigr].
$$

For $0<s<1$ this is a scalar [hyperbolic partial differential equation](../../../partial-differential-equation.md#hyperbolic-partial-differential-equation): its one [characteristic speed](../../../partial-differential-equation.md#characteristic-speed) is real. The [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics) gives $ds/dt=0$ and $dz/dt=a(s)$. A [concentration](../../../physics.md#concentration) disturbance need not descend at the particle [settling velocity](../../../fluid-mechanics.md#settling-velocity); $a(s)$ is the [derivative](../../../calculus.md#derivative) of the transported flux, not $V(s)$. In particular $a(s)$ can be positive even though every particle settles downwards. At $\alpha=0$, $a=-V_0$ and the equation is ordinary translation. At the packing endpoint $s=1$ the differentiability of the chosen constitutive law depends on $\alpha$; none of the initial values used below is at that endpoint.

<h4 id="1/b">b</h4>

↑ **Parent:** [1](#1)

<h5 id="1/b/solution">Solution</h5>

↑ **Parent:** [B](#1/b)

For $\alpha=1$, $f=V_0(s^2-s)$, so the [characteristic speed](../../../partial-differential-equation.md#characteristic-speed) is $a=V_0(2s-1)$ and the [conservation law flux](../../../partial-differential-equation.md#conservation-law-flux) is strictly convex. Let $\tau=V_0t$ and let $\xi$ be the initial vertical position of a [characteristic curve](../../../partial-differential-equation.md#characteristic-curve).

For the increasing ramp, the [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) within its sloping part satisfy $z=\xi(1+0.6\tau)$. They spread apart and never cross. The outer plateau [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed) are $-0.6V_0$ and $0.6V_0$, so the complete [entropy solution](../../../partial-differential-equation.md#entropy-solution) is

$$
\boxed{s(z,t)=\begin{cases}
0.2,&z<-1-0.6\tau,\\
\displaystyle\frac12+\frac{0.3z}{1+0.6\tau},&|z|\leq1+0.6\tau,\\
0.8,&z>1+0.6\tau.
\end{cases}}
$$

The transition widens linearly and its gradient decreases. At large time it approaches a [rarefaction wave](../../../partial-differential-equation.md#rarefaction-wave), with $s\simeq(1+z/\tau)/2$ inside its expanding transition.

For the decreasing ramp, $z=\xi(1-0.6\tau)$ and the [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) converge. Before they meet,

$$
s(z,t)=\begin{cases}
0.8,&z<-1+0.6\tau,\\
\displaystyle\frac12-\frac{0.3z}{1-0.6\tau},&|z|\leq1-0.6\tau,\\
0.2,&z>1-0.6\tau.
\end{cases}
$$

All the ramp [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) meet at $z=0$ at

$$
\boxed{t_*=\frac{5}{3V_0}.}
$$

Thereafter a stationary [sedimentation shock](../../../fluid-mechanics.md#sedimentation-shock) separates $s_L=0.8$ below from $s_R=0.2$ above. Indeed the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions) gives

$$
\dot z_s=\frac{f(0.2)-f(0.8)}{0.2-0.8}=0,
$$

and the incoming [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed) satisfy $a(0.8)=0.6V_0>0>a(0.2)=-0.6V_0$, which makes it an admissible [entropy shock](../../../partial-differential-equation.md#entropy-shock). The discontinuity transports no net excess particle flux because both plateau fluxes equal $-0.16V_0$. These are local solutions before a finite container's boundaries affect the transition.

<a id="1/b/image-spreading-and-shock-formation-for-quadratic-hindered-settling-flux"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52-settling-ramps.png)

**[Figure 1](#1/b/image-spreading-and-shock-formation-for-quadratic-hindered-settling-flux). Spreading and shock formation for quadratic hindered-settling flux**.

The dependence on $\alpha$ is controlled by the [hindered-settling flux inflection](../../../fluid-mechanics.md#hindered-settling-flux-inflection):

$$
f''(s)=V_0\alpha(1-s)^{\alpha-2}\bigl[2-(\alpha+1)s\bigr].
$$

For any smooth initial profile, the [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) has [derivative](../../../calculus.md#derivative)

$$
\frac{\partial z}{\partial\xi}=1+t f''(s_0(\xi))s'_0(\xi).
$$

This formula gives the first [characteristic crossing](../../../partial-differential-equation.md#characteristic-crossing): minimize the positive values of $-1/[f''(s_0)s'_0]$. At $\alpha=0$ neither ramp changes shape; both move down at $V_0$. For $0<\alpha\leq3/2$, the flux is convex throughout $0.2\leq s\leq0.8$: the increasing ramp spreads and the decreasing ramp steepens, although its entire ramp generally no longer focuses simultaneously. For $\alpha\geq9$, the flux is concave throughout that interval and these roles reverse. At the endpoint values the curvature vanishes at one plateau; it does not reverse sign inside the interval.

For $3/2<\alpha<9$, the inflection $s_i=2/(\alpha+1)$ lies between the plateau concentrations. Below $s_i$ the increasing ramp spreads, while above it that ramp compresses; the decreasing ramp has the opposite local behavior. After [characteristic crossing](../../../partial-differential-equation.md#characteristic-crossing), the [entropy solution](../../../partial-differential-equation.md#entropy-solution) can contain both a [shock wave](../../../partial-differential-equation.md#shock-wave) and a [rarefaction wave](../../../partial-differential-equation.md#rarefaction-wave). Quantitatively, an increasing step is selected by the lower convex envelope of $f$ on the interval between its states: curved portions supply [rarefaction waves](../../../partial-differential-equation.md#rarefaction-wave), and straight portions supply [shock waves](../../../partial-differential-equation.md#shock-wave). A decreasing step uses the upper concave envelope. A join between a fan and a [shock wave](../../../partial-differential-equation.md#shock-wave) at a state $s_*$ satisfies the tangent-chord relation $f'(s_*)=[f(s_b)-f(s_*)]/(s_b-s_*)$, where $s_b$ is the other shock state. Thus curvature, not simply the magnitude of $\alpha$, decides the wave pattern; the envelope may reduce to one shock if the tangent lies outside the state interval.

### 2

↑ **Parent:** [Section A](#section-a)

<h4 id="2/solution">Solution</h4>

↑ **Parent:** [2](#2)

Let $\theta=T-T_0>0$ and $\theta_1=T_1-T_0$. The aperture spans the enclosure's depth $H$, so the incoming [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate), equal to the outgoing [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate), is

$$
q=\frac{Hh}{2}\,c\sqrt{g\beta h\theta}.
$$

Only one of these equal exchange fluxes multiplies the [temperature](../../../thermodynamics.md#temperature) difference in the [heat](../../../thermodynamics.md#heat) budget: incoming fluid brings $qT_0$, outgoing fluid removes $qT$. With constant [mass density](../../../fluid-mechanics.md#density) and [specific heat capacity](../../../thermodynamics.md#specific-heat-capacity), those factors cancel and the [well-mixed ventilation temperature balance](../../../fluid-mechanics.md#well-mixed-ventilation-temperature-balance) is

$$
H^3\dot\theta=-q\theta,\qquad
\dot\theta=-k\theta^{3/2},\qquad
k=\frac{c h^{3/2}\sqrt{g\beta}}{2H^2}.
$$

Integrating from $\theta_1$ gives

$$
\boxed{T(t)=T_0+\frac{T_1-T_0}{\left[1+\dfrac{c h^{3/2}\sqrt{g\beta(T_1-T_0)}}{4H^2}\,t\right]^2}.}
$$

The cooling is algebraic rather than exponential because the buoyancy-driven [single-opening exchange flow](../../../fluid-mechanics.md#single-opening-exchange-flow) weakens as its driving [reduced gravity](../../../reduced-gravity.md) decreases. The formula assumes negligible wall [heat capacity](../../../thermodynamics.md#heat-capacity), no heat input, the specified aperture geometry, and a uniform interior [temperature](../../../thermodynamics.md#temperature) maintained by mixing.

With a low-level opening, the dense incoming cold fluid tends to spread along the floor instead of falling through the warm interior. A cold lower layer and warm upper layer develop, giving [stable density stratification](../../../gravity-wave.md#stable-density-stratification). The incoming fluid can short-circuit back out through the low opening after that layer occupies it, leaving warm fluid above poorly ventilated. Thus the uniform-temperature assumption is generally inappropriate: cooling becomes vertically nonuniform and substantially slower for the upper warm fluid. If mixing were artificially maintained, the same lumped budget would still apply; it is the loss of that assumption, rather than a reversal of [buoyancy](../../../fluid-mechanics.md#buoyancy), that changes the physical outcome.

## Section B

↑ **Parent:** [Paper 52](paper-52.md)

### 3

↑ **Parent:** [Section B](#section-b)

<h4 id="3/a">a</h4>

↑ **Parent:** [3](#3)

<h5 id="3/a/solution">Solution</h5>

↑ **Parent:** [A](#3/a)

Let $\ell$ and $\mathcal T$ denote longitudinal length and time scales, and let $U$ be a typical streamwise [velocity](../../../classical-mechanics.md#velocity). The [shallow water](../../../physics.md#shallow-water-approximation) approximation requires $h/\ell\ll1$, slow changes in the channel geometry $h|B'/B|\ll1$, and small longitudinal slopes. The vertical [velocity](../../../classical-mechanics.md#velocity) is then of order $Uh/\ell$; its acceleration must be small compared with the restoring acceleration, for example $Uh/(\mathcal T\ell)+U^2h/\ell^2\ll g'$ in a reduced-gravity layer. The leading [pressure](../../../thermodynamics.md#pressure) is [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure), and cross-sectional horizontal [velocity](../../../classical-mechanics.md#velocity) is approximated by $u(x,t)$. High [Reynolds number](../../../fluid-mechanics.md#reynolds-number) permits negligible interior viscous terms but does not itself guarantee the geometric or hydrostatic assumptions. We also require $B>0$ and $h>0$ in the wetted interior. The dimensionless $B$ need not be small: it measures the cross-section's opening angle, while the smallness condition concerns streamwise variation.

The cross-sectional area and volume transport are

$$
A(x,t)=\int_0^h B(x)z\,dz=\frac{Bh^2}{2},\qquad q=Au.
$$

For an impermeable bed and no [fluid entrainment](../../../fluid-mechanics.md#fluid-entrainment), [volume conservation](../../../physics.md#volume-conservation) gives

$$
\boxed{\partial_t\left(\frac{Bh^2}{2}\right)+\partial_x\left(\frac{Bh^2u}{2}\right)=0,}
$$

or, equivalently,

$$
h_t+uh_x+\frac h2u_x=-\frac{uh}{2}\frac{B'}B.
$$

The geometrical source term expresses the depth change needed when a moving layer encounters a wider or narrower triangular section.

<h4 id="3/b">b</h4>

↑ **Parent:** [3](#3)

<h5 id="3/b/solution">Solution</h5>

↑ **Parent:** [B](#3/b)

Write $g'=g(\rho_f-\rho_a)/\rho_f>0$. The [Saint-Venant dry-front condition](../../../reduced-gravity.md#saint-venant-dry-front-condition) describes a liquid advancing over a dry bed, or into an ambient whose inertia is negligible, as when $\rho_a/\rho_f\ll1$. The edge has $h_f=0$; its [velocity](../../../classical-mechanics.md#velocity) is obtained by continuing the appropriate [shallow water](../../../physics.md#shallow-water-approximation) [Riemann invariant](../../../compressible-flow.md#riemann-invariant) to zero depth. There is no independent universal finite-depth head [Froude number](../../../reduced-gravity.md#froude-number). In the triangular geometry a release of a resting layer gives $u_f=2\sqrt{2g'h_0}$, whereas a rectangular release gives $2\sqrt{g'h_0}$.

The [Benjamin deep-ambient front condition](../../../reduced-gravity.md#benjamin-deep-ambient-front-condition) includes the inertia of an ambient that must turn around a finite-depth [gravity current](../../../reduced-gravity.md#gravity-current) head. In the ideal deep-ambient [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation), $\rho_a/\rho_f$ is close to one and

$$
\boxed{u_f=F\sqrt{g'h_f},\qquad F=\sqrt2.}
$$

Here $h_f$ is the current depth just behind its head, $u_f$ its speed relative to the far ambient, and $F$ the ideal head [Froude number](../../../reduced-gravity.md#froude-number). The ambient is much deeper than $h_f$; a finite upper-layer depth changes the closure. The lower density must exceed the ambient density for a bottom current. A non-Boussinesq head requires an appropriate density-ratio correction rather than using $F=\sqrt2$ at every ratio. The Saint-Venant and Benjamin models therefore describe different front physics, even though both use the same long-wave equations in the interior.

<h4 id="3/c">c</h4>

↑ **Parent:** [3](#3)

<h5 id="3/c/solution">Solution</h5>

↑ **Parent:** [C](#3/c)

Constant density in each layer and negligible ambient acceleration far from the front give

$$
\boxed{u_t+uu_x+g'h_x=0.}
$$

This primitive [momentum conservation](../../../classical-mechanics.md#momentum-conservation) equation remains valid with slowly varying $B$. In conservative form it is

$$
\partial_t(Au)+\partial_x\left(Au^2+\frac{g'Bh^3}{6}\right)=\frac{g'h^3}{6}B',
$$

where the right side is the longitudinal component of the [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) force on the sloping sidewalls. Omitting that term while retaining variable $B$ would give the wrong acceleration.

Together with [volume conservation](../../../physics.md#volume-conservation), the principal coefficient matrix in $(h,u)$ is

$$
\begin{pmatrix}u&h/2\\g'&u\end{pmatrix}.
$$

Its real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) are

$$
\boxed{\frac{dx}{dt}=u\pm c,\qquad c=\sqrt{\frac{g'h}{2}}.}
$$

These are downstream and upstream [gravity waves](../../../gravity-wave.md) relative to the moving fluid. The factor $1/2$ is geometric: the hydraulic depth is $A/b(h)=h/2$. Both waves move downstream in a sufficiently fast current, whereas one can carry information upstream in a slower current.

For $B=1$, differentiate $c^2=g'h/2$ and combine the two equations. The [Riemann invariants](../../../compressible-flow.md#riemann-invariant) are

$$
\boxed{\left[\partial_t+(u\pm c)\partial_x\right](u\pm4c)=0.}
$$

For variable $B$ they instead obey

$$
\left[\partial_t+(u\pm c)\partial_x\right](u\pm4c)=\mp cu\frac{B'}B,
$$

which also checks that the invariant claim depends on a prismatic channel.

<h4 id="3/d">d</h4>

↑ **Parent:** [3](#3)

<h5 id="3/d/solution">Solution</h5>

↑ **Parent:** [D](#3/d)

Put $c_0=\sqrt{g'h_0/2}$. The undisturbed reservoir has $u=0$ and [Riemann invariants](../../../compressible-flow.md#riemann-invariant) $u\pm4c=\pm4c_0$. The right-going [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) supply the invariant $u+4c=4c_0$ throughout the release. The spreading disturbance is the other family, whose speed is $u-c$. In its [rarefaction wave](../../../partial-differential-equation.md#rarefaction-wave) let $\xi=x/t=u-c$. Then

$$
c=\frac{4c_0-\xi}{5},\qquad u=\frac{4(c_0+\xi)}5.
$$

At the reservoir edge $u=0,c=c_0$, so the back of the [rarefaction wave](../../../partial-differential-equation.md#rarefaction-wave) travels at $-c_0$. At the dry edge $c=0$ the [Saint-Venant dry-front condition](../../../reduced-gravity.md#saint-venant-dry-front-condition) gives

$$
\boxed{x_f(t)=4c_0t,\qquad u_f=4c_0=2\sqrt{2g'h_0}.}
$$

Thus the fan occupies $-c_0t\leq x\leq4c_0t$, while $x<-c_0t$ remains undisturbed. Its full length grows at $5c_0$; there is no finite-depth uniform shelf between the fan and the dry front. The optional interior depth is $h=h_0[(4c_0-x/t)/(5c_0)]^2$.

The fan's minus-family [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) are rays $x=\xi t$. For the plus family in the fan, $dx/dt=u+c=(8c_0+3x/t)/5$; [integration](../../../calculus.md#integral) gives $x=4c_0t+C t^{3/5}$, with constants selected at entry from the reservoir. These curved paths transport the constant plus [Riemann invariant](../../../compressible-flow.md#riemann-invariant).

<a id="3/d/image-triangular-channel-dry-bed-release-with-its-rarefaction-rays-and-right-going-characteristics"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52-triangular-dam-break.png)

**[Figure 2](#3/d/image-triangular-channel-dry-bed-release-with-its-rarefaction-rays-and-right-going-characteristics). Triangular-channel dry-bed release with its rarefaction rays and right-going characteristics**.

<h4 id="3/e">e</h4>

↑ **Parent:** [3](#3)

<h5 id="3/e/solution">Solution</h5>

↑ **Parent:** [E](#3/e)

Use a [gravity-current box model](../../../reduced-gravity.md#gravity-current-box-model): approximate the current by uniform depth $h(t)$ and length $L(t)$, with constant [reduced gravity](../../../reduced-gravity.md), no deposition and no [fluid entrainment](../../../fluid-mechanics.md#fluid-entrainment). The triangular cross-sectional area is $h^2/2$, so the fixed released volume is

$$
V_0=\frac12Lh^2,\qquad h=\left(\frac{2V_0}{L}\right)^{1/2}.
$$

The [Benjamin deep-ambient front condition](../../../reduced-gravity.md#benjamin-deep-ambient-front-condition) closes the integral model:

$$
\dot L=\sqrt{2g'h}=F\sqrt{g'}(2V_0)^{1/4}L^{-1/4},\qquad F=\sqrt2.
$$

For a finite initial length $L_0$, direct [integration](../../../calculus.md#integral) gives

$$
\boxed{L(t)=\left[L_0^{5/4}+\frac54F\sqrt{g'}(2V_0)^{1/4}t\right]^{4/5},\qquad h(t)=\sqrt{2V_0/L(t)}.}
$$

The ideal point-release limit takes $L_0=0$ and has $L\propto t^{4/5}$, $h\propto t^{-2/5}$. Its divergent initial depth is outside the [shallow water](../../../physics.md#shallow-water-approximation) approximation, so a real finite reservoir regularizes the early stage. This is the [finite-volume triangular-channel current](../../../reduced-gravity.md#finite-volume-triangular-channel-current) integral law; it does not assert a spatially uniform exact solution of the local equations.

### 4

↑ **Parent:** [Section B](#section-b)

<h4 id="4/a">a</h4>

↑ **Parent:** [4](#4)

<h5 id="4/a/solution">Solution</h5>

↑ **Parent:** [A](#4/a)

Let $W\geq0$ be the downward fluid suction speed and $V\geq0$ the downward particle [settling velocity](../../../fluid-mechanics.md#settling-velocity) relative to that fluid. Set $Q=uh$ and $g'=g'_0\phi$. The carrier [volume conservation](../../../physics.md#volume-conservation) and particle-volume balances per unit channel width are

$$
\boxed{Q'=-W,\qquad (Q\phi)'=-(W+V)\phi.}
$$

The particle sink includes suction as well as relative settling: the particles follow the well-mixed withdrawn fluid, in addition to settling through it. Subtracting $\phi Q'$ yields $Q\phi'=-V\phi$. Thus for $W>0$, as long as $Q>0$,

$$
\boxed{Q=Q_0-Wx,\qquad\phi=\left(1-\frac{Wx}{Q_0}\right)^{V/W}.}
$$

For $W=0$ the continuous limit is $Q=Q_0$ and $\phi=e^{-Vx/Q_0}$. In particular suction alone does not change the well-mixed particle fraction: $V=0$ implies $\phi=1$.

Withdrawn fluid carries its local horizontal [momentum](../../../classical-mechanics.md#momentum), so the [momentum flux](../../../physics.md#momentum-flux) and [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) force obey

$$
\boxed{\left(hu^2+\frac12g'_0\phi h^2\right)'=-Wu.}
$$

Expand this and use $Q'=-W$. The suction [momentum](../../../classical-mechanics.md#momentum) terms cancel in the primitive acceleration equation, leaving

$$
uu'+g'_0\phi h'+\frac12g'_0h\phi'=0.
$$

These are the governing equations for a [particle-laden current with suction](../../../reduced-gravity.md#particle-laden-current-with-suction). Substituting $u=Q/h$ and the [concentration](../../../physics.md#concentration) equation gives the convenient depth equation

$$
\boxed{(1-\operatorname{Fr}^2)h'=\frac{Wu}{g'_0\phi}+\frac{Vh}{2Q},\qquad \operatorname{Fr}^2=\frac{u^2}{g'_0\phi h}.}
$$

The steady carrier flux is exhausted at the formal length $\boxed{x_*=Q_0/W}$ when $W>0$. Positive $Q$ cannot continue beyond it. Near that limit a chosen depth branch, mixing or shallow-layer assumptions may fail, so this is the mass-budget extent, not a guarantee that every arbitrary inlet state has a regular shallow continuation to it. When $W=0$, settling makes the driving [reduced gravity](../../../reduced-gravity.md) exponentially small but does not remove carrier fluid; this ideal steady model has no finite mass-budget runout.

<h4 id="4/b">b</h4>

↑ **Parent:** [4](#4)

<h5 id="4/b/solution">Solution</h5>

↑ **Parent:** [B](#4/b)

At $V=0$, the particle budget gives $\phi=1$, so $g'=g'_0$ is constant. The primitive [momentum conservation](../../../classical-mechanics.md#momentum-conservation) equation integrates to

$$
\frac12u^2+g'_0h=\frac12u_0^2+g'_0h_0,\qquad u_0=Q_0/h_0.
$$

Introduce $q=Q/Q_0=1-Wx/Q_0$, $y=h/h_0$ and $\varepsilon=\operatorname{Fr}_0^2=Q_0^2/(g'_0h_0^3)\ll1$. The exact relation on the [subcritical flow](../../../reduced-gravity.md#subcritical-flow) branch is

$$
y+\frac{\varepsilon q^2}{2y^2}=1+\frac\varepsilon2.
$$

Expanding uniformly for $0\leq q\leq1$ gives

$$
\boxed{\frac{h}{h_0}=1+\frac{\operatorname{Fr}_0^2}{2}(1-q^2)+O(\operatorname{Fr}_0^4),\qquad h\sim h_0.}
$$

The depth increases slightly because horizontal kinetic energy decreases as fluid is removed. In fact the depth equation has $h'\geq0$ on this branch, and

$$
\operatorname{Fr}^2=\varepsilon\frac{q^2}{y^3}\leq\varepsilon\ll1.
$$

Thus the small-[Froude number](../../../reduced-gravity.md#froude-number) approximation becomes better downstream, including as the flux vanishes. At leading order $u=(Q_0-Wx)/h_0$.

<h4 id="4/c">c</h4>

↑ **Parent:** [4](#4)

<h5 id="4/c/solution">Solution</h5>

↑ **Parent:** [C](#4/c)

With $W=0$ and $V>0$, $Q=Q_0$ and $\phi=e^{-kx}$, where $k=V/Q_0$. No carrier [momentum](../../../classical-mechanics.md#momentum) is withdrawn; hence the integrated [momentum flux](../../../physics.md#momentum-flux) is exactly constant:

$$
\boxed{\frac{Q_0^2}{h}+\frac12g'_0e^{-kx}h^2=K,\qquad K=\frac{Q_0^2}{h_0}+\frac12g'_0h_0^2.}
$$

On an initially small-[Froude number](../../../reduced-gravity.md#froude-number) branch, the [pressure](../../../thermodynamics.md#pressure) term dominates. At leading order

$$
\boxed{h(x)\sim h_0e^{kx/2},\qquad u(x)\sim u_0e^{-kx/2}.}
$$

A slightly more accurate large-distance amplitude is $\sqrt{2K/g'_0}$, so $h\sim\sqrt{2K/g'_0}\,e^{kx/2}$. The [Froude number](../../../reduced-gravity.md#froude-number) satisfies $\operatorname{Fr}^2\sim\operatorname{Fr}_0^2e^{-kx/2}$ and remains small. The growing depth can eventually violate confinement or the [shallow water](../../../physics.md#shallow-water-approximation) assumption; this does not make the asymptotic [momentum](../../../classical-mechanics.md#momentum) calculation inconsistent within its intended regime.

On an initially large-[Froude number](../../../reduced-gravity.md#froude-number) branch, horizontal [momentum flux](../../../physics.md#momentum-flux) dominates instead. The leading depth is constant, $\boxed{h\sim h_0}$, while the decaying [reduced gravity](../../../reduced-gravity.md) makes the [Froude number](../../../reduced-gravity.md#froude-number) still larger. To resolve the small change, put $\delta=\operatorname{Fr}_0^{-2}\ll1$ and $y=h/h_0$:

$$
\frac1y+\frac\delta2e^{-kx}y^2=1+\frac\delta2,
$$

so

$$
\boxed{\frac h{h_0}=1+\frac\delta2(e^{-kx}-1)+O(\delta^2).}
$$

The depth decreases slightly and tends exactly to $h_\infty=Q_0^2/K=h_0/(1+\delta/2)$. Its [Froude number](../../../reduced-gravity.md#froude-number) grows like $\operatorname{Fr}_0e^{kx/2}$. Both approximations agree with the exact depth equation $h'=kh/[2(1-\operatorname{Fr}^2)]$: the [subcritical flow](../../../reduced-gravity.md#subcritical-flow) deepens, while the [supercritical flow](../../../reduced-gravity.md#supercritical-flow) thins.

## Section C

↑ **Parent:** [Paper 52](paper-52.md)

### 5

↑ **Parent:** [Section C](#section-c)

<h4 id="5/a">a</h4>

↑ **Parent:** [5](#5)

<h5 id="5/a/solution">Solution</h5>

↑ **Parent:** [A](#5/a)

Use $G=g\beta(T-T_0(z))$ for the plume [reduced gravity](../../../reduced-gravity.md), and take $z$ upwards. For a symmetric [line plume](../../../turbulent-plume.md#line-plume) define fluxes per unit source length,

$$
q=\int w\,dx,\qquad m=\int w^2\,dx,\qquad \mathcal B=\int wG\,dx.
$$

The integrals span the plume; its edges can move horizontally with $z$. The [fluid entrainment](../../../fluid-mechanics.md#fluid-entrainment) rate at one moving edge is the inward normal transport relative to that edge. For an edge $x=b(z)$ it is $E=wb'-u$; symmetry supplies equal transport through the other edge. The [Batchelor entrainment hypothesis](../../../turbulent-plume.md#batchelor-entrainment-hypothesis) closes its mean value as $E=\alpha w_c$, where $w_c$ is a representative vertical [velocity](../../../classical-mechanics.md#velocity) and $\alpha$ is the [entrainment coefficient](../../../turbulent-plume.md#entrainment-coefficient). The integrated [volume conservation](../../../physics.md#volume-conservation) equation is therefore $q'=2\alpha w_c$.

Using [volume conservation](../../../physics.md#volume-conservation), the vertical acceleration equation has conservative form $\partial_x(uw)+\partial_z(w^2)=G$. Incoming ambient has zero vertical [momentum](../../../classical-mechanics.md#momentum); the integrated [momentum conservation](../../../classical-mechanics.md#momentum-conservation) equation is consequently $m'=\int G\,dx$. For the [temperature](../../../thermodynamics.md#temperature) anomaly, $T_0$ depends on height and

$$
\partial_x(uG)+\partial_z(wG)=-N^2w,\qquad N^2=g\beta\frac{dT_0}{dz}.
$$

Ambient fluid enters with $G=0$, giving the [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) balance. The integral model is

$$
\boxed{q'=2\alpha w_c,\qquad m'=\int G\,dx,\qquad \mathcal B'=-N^2q.}
$$

Here $N$ is the [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency) when $N^2>0$; the same algebra permits unstable [temperature](../../../thermodynamics.md#temperature) gradients with $N^2<0$.

These are mean integral balances. The advective equations printed in the question omit explicit turbulent stresses and heat fluxes; a [turbulent plume](../../../turbulent-plume.md) interpretation requires the usual entrainment closure for that unresolved transverse transport. Assuming vanishing edge stresses and heat fluxes, and negligible additional axial turbulent-flux contributions, gives the displayed bulk model. It would be inconsistent to treat a discontinuous top-hat profile as a smooth exact pointwise solution of the inviscid temperature-advection equation.

<h4 id="5/b">b</h4>

↑ **Parent:** [5](#5)

<h5 id="5/b/solution">Solution</h5>

↑ **Parent:** [B](#5/b)

In the [top-hat plume model](../../../turbulent-plume.md#top-hat-plume-model), vertical [velocity](../../../classical-mechanics.md#velocity) $w(z)$ and [reduced gravity](../../../reduced-gravity.md) $G(z)$ are uniform over $-b<x<b$. The ambient has zero vertical [velocity](../../../classical-mechanics.md#velocity), negligible ambient turbulence and a prescribed $T_0(z)$. Then

$$
q=2bw,\qquad m=2bw^2,\qquad\mathcal B=2bwG,
$$

and the equations become

$$
\boxed{(bw)'=\alpha w,\qquad (bw^2)'=bG,\qquad (bwG)'=-bwN^2.}
$$

Equivalently, the [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation) for the three unknowns are

$$
\boxed{w'=\frac Gw-\frac{\alpha w}{b},\qquad b'=2\alpha-\frac{bG}{w^2},\qquad G'=-N^2-\frac{\alpha G}{b}.}
$$

The last equation displays dilution by [fluid entrainment](../../../fluid-mechanics.md#fluid-entrainment) as well as loss of relative [buoyancy](../../../fluid-mechanics.md#buoyancy) while rising through a stably stratified ambient. The model assumes a steady slender two-dimensional [turbulent plume](../../../turbulent-plume.md), large [Reynolds number](../../../fluid-mechanics.md#reynolds-number), the [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation), constant $\beta$ and $\alpha$, negligible heat loss, negligible imposed crossflow, and negligible [pressure](../../../thermodynamics.md#pressure) departure from ambient [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure). The factors of two count both entraining edges; $b$ is a half-width. A finite source also requires its volume, [momentum](../../../classical-mechanics.md#momentum) and [buoyancy fluxes](../../../turbulent-plume.md#buoyancy-flux) as boundary data.

<h4 id="5/c">c</h4>

↑ **Parent:** [5](#5)

<h5 id="5/c/solution">Solution</h5>

↑ **Parent:** [C](#5/c)

Let $\mathcal B_0>0$ be the source [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) per unit length. The conversion from the heat-source strength depends on its units: if $F$ is a kinematic temperature-volume flux, $\mathcal B_0=g\beta F$; if it is a physical heat power per unit length, $\mathcal B_0=g\beta F/(\rho_0c_p)$, where $c_p$ is [specific heat capacity at constant pressure](../../../thermodynamics.md#specific-heat-capacity-at-constant-pressure). This explicit convention avoids treating heat power as a [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) without conversion.

For uniform ambient $N^2=0$, so $\mathcal B=\mathcal B_0$. The ideal pure line-source limit has negligible initial volume and [momentum](../../../classical-mechanics.md#momentum) transport. The flux equations admit $w=w_*$ constant, $q=2\alpha w_*z$ and $b=\alpha z$. Substituting into the [momentum](../../../classical-mechanics.md#momentum) equation gives $2\alpha w_*^2=2bG$, and the conserved [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) then fixes $2\alpha w_*^3=\mathcal B_0$. Thus

$$
\boxed{2b=2\alpha z,\qquad w=w_* =\left(\frac{\mathcal B_0}{2\alpha}\right)^{1/3},\qquad g'=G=\frac{w_*^2}{z}=\frac{\mathcal B_0^{2/3}}{(2\alpha)^{2/3}z}.}
$$

This verifies all three differential equations, not just their dimensional exponents. The plume grows in width while maintaining constant upward [velocity](../../../classical-mechanics.md#velocity); its [temperature](../../../thermodynamics.md#temperature) anomaly decreases like $z^{-1}$. The zero-height singularity is the ideal point-source limit. A finite source or nonzero [momentum](../../../classical-mechanics.md#momentum) input introduces a [plume virtual origin](../../../turbulent-plume.md#plume-virtual-origin) or a forced near-source region; the heat strength alone cannot uniquely determine that finite-source region.

<h4 id="5/d">d</h4>

↑ **Parent:** [5](#5)

<h5 id="5/d/solution">Solution</h5>

↑ **Parent:** [D](#5/d)

Let the closed box have ceiling height $H$ above the source. The printed width $2R$ alone does not specify this height, so it must appear as an additional geometrical parameter. Take $t=0$ here when the plume has first reached the ceiling and its thin outflow has spread across the box. The leading [filling box model](../../../turbulent-plume.md#filling-box-model) assumes a negligible source volume, insulated boundaries, fast horizontal spreading, slow evolution compared with the plume transit time, negligible diffusion, and $b\ll R$. Below the interface the ambient still has its original [temperature](../../../thermodynamics.md#temperature), so the local plume flux remains $q(z)=2\alpha w_*z$ from part (c).

The ceiling outflow creates a warm upper region. [Fluid entrainment](../../../fluid-mechanics.md#fluid-entrainment) draws the original lower fluid into the plume, making that upper region deepen. The [filling-box first front](../../../turbulent-plume.md#filling-box-first-front) is the lower material boundary of fluid already modified by plume discharge, separating it from the initially unmodified ambient; it need not bound a uniformly mixed upper layer. With negligible occupied plume area, [volume conservation](../../../physics.md#volume-conservation) at its height $h(t)$ gives

$$
2R\dot h=-q(h)=-2\alpha w_*h.
$$

Therefore

$$
\boxed{h(t)=H e^{-t/t_f},\qquad t_f=\frac{R}{\alpha w_*}=\frac{2R}{(2\alpha)^{2/3}\mathcal B_0^{1/3}}.}
$$

If source switch-on is the time origin instead, replace $t$ by elapsed time after the initial transit and spreading stage; the quasi-steady model does not resolve that stage.

The [buoyancy](../../../fluid-mechanics.md#buoyancy) jump requires distinguishing ambient fluid at the front from the plume crossing it. Just after the first ceiling outflow, the ambient [buoyancy](../../../fluid-mechanics.md#buoyancy) immediately above the nascent front is

$$
G_H=\frac{\mathcal B_0}{q(H)}=\frac{w_*^2}{H}.
$$

Outside the narrow plume, ambient [temperature](../../../thermodynamics.md#temperature) is transported without diffusion. If $G_a$ is its [buoyancy](../../../fluid-mechanics.md#buoyancy) relative to the original fluid, its equation is

$$
\partial_tG_a-\frac{q(z)}{2R}\partial_zG_a=0.
$$

The first front follows precisely these material trajectories, so the [temperature](../../../thermodynamics.md#temperature) of the fluid immediately above it is conserved. The initially unmodified fluid below has $G_a=0$. Thus the ambient jump is

$$
\boxed{[G_a]_{\text{above}-\text{below}}=\frac{w_*^2}{H},\qquad [T_a]=\frac{w_*^2}{g\beta H}.}
$$

By contrast, the contemporaneous plume immediately below the front has $G_p(h,t)=w_*^2/h(t)$, which grows as the front descends. That plume value is not the ambient jump across the material first front. Equating the two would inadvertently impose a uniformly mixed upper layer and discard the [stable density stratification](../../../gravity-wave.md#stable-density-stratification) of the standard [filling box model](../../../turbulent-plume.md#filling-box-model). Diffusion or extensive interfacial mixing can smooth and alter the ideal jump.

<h4 id="5/e">e</h4>

↑ **Parent:** [5](#5)

<h5 id="5/e/solution">Solution</h5>

↑ **Parent:** [E](#5/e)

The [filling box model](../../../turbulent-plume.md#filling-box-model) requires the first outflow to spread across the enclosure and remain above unmodified fluid, while a narrow nearly vertical plume rises below it. Several mechanisms can defeat those assumptions. A tall narrow box makes the plume a substantial fraction of the width, so its compensating return [velocity](../../../classical-mechanics.md#velocity) is no longer small and modifies both [fluid entrainment](../../../fluid-mechanics.md#fluid-entrainment) and [momentum flux](../../../physics.md#momentum-flux). A fast ceiling current can descend the sidewalls and overturn the initially stable upper region. In both cases a horizontally uniform slowly descending [filling-box first front](../../../turbulent-plume.md#filling-box-first-front) is inappropriate. Strong plume displacement from the centre, imposed crossflow, large source volume, vents or substantial wall cooling likewise alter the volume and heat budgets.

A useful diagnostic is whether the ceiling outflow's inertial acceleration, of order $U_c^2/\ell_c$, overwhelms the restoring [buoyancy](../../../fluid-mechanics.md#buoyancy) of the nascent layer. If $U_c^2/(G_H d_c)$ is not small for its depth $d_c$, the outflow can penetrate or overturn the stratification rather than remain trapped above it. This is a diagnostic [Froude number](../../../reduced-gravity.md#froude-number), not a universal threshold without specifying the wall-current geometry and mixing. Low [Reynolds number](../../../fluid-mechanics.md#reynolds-number) invalidates a constant turbulent [entrainment coefficient](../../../turbulent-plume.md#entrainment-coefficient), and thermal diffusion or wall heat loss can erase the sharp first-front jump. Thus **large aspect ratio, strong return circulation, overturning, ventilation or diffusion require a model beyond the standard filling-box approximation**.

### 6

↑ **Parent:** [Section C](#section-c)

<h4 id="6/a">a</h4>

↑ **Parent:** [6](#6)

<h5 id="6/a/solution">Solution</h5>

↑ **Parent:** [A](#6/a)

Use the [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) and a [top-hat plume model](../../../turbulent-plume.md#top-hat-plume-model). Let $v(z)<0$ be the uniform ambient return [velocity](../../../classical-mechanics.md#velocity) outside the plume. Negligible source [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) and an impermeable cylindrical wall require zero net transport through every horizontal section:

$$
\boxed{b^2w+(R^2-b^2)v=0,\qquad v=-\frac{b^2w}{R^2-b^2}.}
$$

The entrainment speed must be specified relative to that moving ambient. Taking it to be $\alpha(w-v)$ gives

$$
\boxed{\frac{d}{dz}(b^2w)=2\alpha b(w-v).}
$$

The surrounding unmodified fluid has zero [buoyancy](../../../fluid-mechanics.md#buoyancy) relative to the initial fluid. Neglecting thermal or compositional loss therefore gives

$$
\boxed{\frac{d}{dz}(b^2wg')=0.}
$$

Let $B_s$ denote the conserved specific source [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux): $B_s=B_o/\pi$ if $B_o$ is the actual integrated source flux, or $B_s=B_o$ if the source strength has already been normalized by $\pi$.

To obtain the usual integral-model singularity one must also state a [pressure](../../../thermodynamics.md#pressure) closure. Here take the whole-section mean [pressure](../../../thermodynamics.md#pressure) to have only its reference ambient [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure), and neglect wall force and extra vertical turbulent-stress fluxes in the integral budget. Internal [momentum](../../../classical-mechanics.md#momentum) transfers between plume and ambient cancel in that whole-section balance. The remaining upward force is the plume [buoyancy](../../../fluid-mechanics.md#buoyancy), giving

$$
\boxed{\frac{d}{dz}\left[b^2w^2+(R^2-b^2)v^2\right]=b^2g'.}
$$

The two [momentum fluxes](../../../physics.md#momentum-flux) add, even though $v$ is negative: vertical [momentum](../../../classical-mechanics.md#momentum) transported downward also contributes $v^2$ to the flux through an upward-oriented horizontal section. These three flux balances, with the algebraic return-velocity constraint, govern $b,w,g'$ in the [confined plume with compensating return flow](../../../turbulent-plume.md#confined-plume-with-compensating-return-flow).

The pressure-neglecting closure is an integral approximation, not a claim that the return fluid has zero acceleration. If a mean [pressure](../../../thermodynamics.md#pressure) departure $p_*(z)$ is retained, the whole-section [momentum](../../../classical-mechanics.md#momentum) balance instead contains $-(R^2/\rho_0)p_*'(z)$, along with any wall-force or stress contribution. The entrainment hypothesis alone does not specify that function. The singularity calculated below belongs to the stated pressure-neglecting model; it is not forced by continuity alone or asserted to be an infinite [velocity](../../../classical-mechanics.md#velocity) in the real fluid.

<h4 id="6/b">b</h4>

↑ **Parent:** [6](#6)

<h5 id="6/b/solution">Solution</h5>

↑ **Parent:** [B](#6/b)

Normalize all fluxes by $\pi$, rather than including that factor in only some of them. The specific plume [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate), [momentum flux](../../../physics.md#momentum-flux) and [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) are

$$
\boxed{Q=b^2w,\qquad M=b^2w^2,\qquad B=b^2wg'=B_s.}
$$

The ambient transport is $-Q$ and its specific [momentum flux](../../../physics.md#momentum-flux) is

$$
M_a=(R^2-b^2)v^2=\frac{Q^2}{R^2-Q^2/M}.
$$

Put $s=b^2/R^2=Q^2/(R^2M)$, with $0<s<1$. The total specific [momentum flux](../../../physics.md#momentum-flux) is

$$
J=M+M_a=\frac{M}{1-s},\qquad b=\frac{Q}{\sqrt M},\qquad w=\frac MQ,\qquad g'=\frac{B_s}{Q}.
$$

The first differential equation follows immediately from relative-speed [fluid entrainment](../../../fluid-mechanics.md#fluid-entrainment):

$$
\boxed{Q'=\frac{2\alpha\sqrt M}{1-s}.}
$$

For the second, differentiate $J=M/(1-s)$ and use $s'=2sQ'/Q-sM'/M$. Since $J'=b^2g'=B_sQ/M$, this yields

$$
\boxed{(1-2s)M'=\frac{B_sQ}{M}(1-s)^2-\frac{2Q}{R^2}Q'.}
$$

This is the requested two-equation system, with $B=B_s$ and zero total [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) as the additional conservation conditions. Near the pure source, $Q,M\to0$ and $s\to0$. Eliminating height in that limit gives

$$
\frac{dM}{dQ}\sim\frac{B_sQ}{2\alpha M^{3/2}},\qquad M^{5/2}\sim\frac{5B_s}{8\alpha}Q^2.
$$

The zero [integration](../../../calculus.md#integral) constant selects a [pure plume](../../../turbulent-plume.md#pure-plume); a nonzero imposed source [momentum](../../../classical-mechanics.md#momentum) would select a different branch and generally a different turning height. The leading radius is $b\sim6\alpha z/5$, which recovers the unconfined pure-plume limit near the source.

<h4 id="6/c">c</h4>

↑ **Parent:** [6](#6)

<h5 id="6/c/solution">Solution</h5>

↑ **Parent:** [C](#6/c)

It is helpful to solve using the nonsingular total flux $J$ and [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) $Q$ before recovering $M$. The relation $J=M/(1-Q^2/(R^2M))$ is quadratic:

$$
M^2-JM+\frac{JQ^2}{R^2}=0,\qquad M=\frac{J+\sqrt{J^2-4JQ^2/R^2}}2.
$$

The plus sign selects the small-area pure-source branch. Its discriminant vanishes when $J=4Q^2/R^2$, giving

$$
\boxed{s_o=\frac12,\qquad b_o=\frac R{\sqrt2},\qquad M_o=\frac{2Q_o^2}{R^2}.}
$$

Therefore

$$
\boxed{w_o=\frac{2Q_o}{R^2},\qquad v_o=-w_o,\qquad (M_a)_o=M_o=\frac{R^2w_o^2}{2}.}
$$

The specific upward plume and ambient momentum-flux contributions are equal, not opposite. The ambient's transported [momentum](../../../classical-mechanics.md#momentum) has the opposite sign from its transported volume, so their product remains positive.

To show that the pure branch actually reaches this fold in finite height and that it is a genuine pole, introduce

$$
U_* =\left(\frac{B_s}{\alpha R}\right)^{1/3},\quad q=\frac Q{R^2U_*},\quad m=\frac M{R^2U_*^2},\quad j=\frac J{R^2U_*^2},\quad \zeta=\frac{\alpha z}{R}.
$$

Then $s=q^2/m$ and

$$
\frac{dq}{d\zeta}=\frac{2\sqrt m}{1-s},\qquad \frac{dj}{dq}=\frac{q(1-s)}{2m^{3/2}},\qquad m=\frac{j+\sqrt{j^2-4jq^2}}2.
$$

The pure-source condition is $j\sim(5/8)^{2/5}q^{4/5}$. Before the fold, $s<1/2$ and $m>2q^2$. Thus for every fixed positive $q_1$, the [derivative](../../../calculus.md#derivative) $dj/dq$ is bounded above by a constant times $q^{-2}$ on $q\geq q_1$. If the branch continued for arbitrarily large $q$, $j$ would remain bounded, contradicting $j\geq4q^2$. Hence it reaches $j=4q^2$ at a finite $q_o>0$. Its height is finite because $d\zeta/dq=(1-s)/(2\sqrt m)$ is finite away from the source and behaves like a constant times $q^{-2/5}$ at the source, an integrable singularity.

For the numerator, write $m=j(1-s)$. Then

$$
\frac{dj}{dq}=\frac{q}{2j^{3/2}\sqrt{1-s}}\geq\frac{q}{2j^{3/2}},\qquad j^{5/2}\geq\frac58q^2.
$$

At the fold $j=4q_o^2$, so $q_o^3\geq5/256$. On the other hand the dimensionless numerator in the $m$ equation at $s=1/2$ is

$$
\frac1{8q_o}-8\sqrt2\,q_o^2.
$$

It is strictly negative because $5/256>1/(64\sqrt2)$. The denominator $1-2s$ approaches zero from above. Consequently **$dM/dz\to-\infty$ at finite $z_o$, although the fluxes and velocities themselves remain finite**. This proves the [confined-plume momentum fold](../../../turbulent-plume.md#confined-plume-momentum-fold) rather than merely noticing a possible zero denominator.

The dimensionless pure-source branch uniquely determines the remaining amplitudes. They can be specified without an elementary antiderivative by integrating the displayed scalar equation for $j(q)$ until $j=4q^2$, and setting

$$
\zeta_o=\int_0^{q_o}\frac{1-q^2/m(q)}{2\sqrt{m(q)}}\,dq.
$$

A direct numerical [integration](../../../calculus.md#integral) gives $q_o\simeq0.281610$, $\zeta_o\simeq0.400049$, so the dimensional results for this specified entrainment convention are

$$
\boxed{z_o\simeq0.400049\frac R\alpha,\quad w_o\simeq0.563220\left(\frac{B_s}{\alpha R}\right)^{1/3},\quad M_o=(M_a)_o\simeq0.158608 R^2\left(\frac{B_s}{\alpha R}\right)^{2/3}.}
$$

A convention using $\alpha w$ instead of $\alpha(w-v)$ would produce different numerical amplitudes; the relative-speed convention was stated in part (a).

Physically $z_o$ is a turnover or breakdown height for a slender steady plume surrounded by uniform counterflow. The opposing streams then occupy equal areas and have equal speeds; the single-valued small-area branch cannot continue smoothly. Above it one expects lateral spreading, stronger recirculation, mixing and unsteady buoyant structures rather than a continuation of the same slender top-hat column. A detailed flow or upper-layer evolution requires restoring [pressure](../../../thermodynamics.md#pressure) and stress dynamics and, eventually, the modified ambient stratification. The model does not predict an infinite physical [velocity](../../../classical-mechanics.md#velocity), nor does it require that all buoyant fluid forever remain below $z_o$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
