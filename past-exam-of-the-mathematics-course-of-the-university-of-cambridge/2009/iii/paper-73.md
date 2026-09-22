# Paper 73

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper73.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper73.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [1](#1/iii/1)
      - [Solution](#1/iii/1/solution)
    - [2](#1/iii/2)
      - [Solution](#1/iii/2/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
  - [vi](#3/vi)
    - [Solution](#3/vi/solution)
  - [vii](#3/vii)
    - [Solution](#3/vii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)
  - [vi](#4/vi)
    - [Solution](#4/vi/solution)
  - [vii](#4/vii)
    - [Solution](#4/vii/solution)

## 1

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Choose $x$ upslope and $z$ normally downwards from the impermeable roof, so the buoyant layer occupies $0<z<h(x,t)$. Use the [hydrostatic approximation](../../../fluid-mechanics.md#hydrostatic-approximation) and neglect the ambient return-flow [pressure](../../../thermodynamics.md#pressure) correction of relative order $h/H$. [Pressure](../../../thermodynamics.md#pressure) continuity at the interface gives the [pressure](../../../thermodynamics.md#pressure) inside the buoyant layer as

$$
p=p_0-\rho gx\sin\theta+\Delta\rho\,gh\cos\theta+(\rho-\Delta\rho)gz\cos\theta.
$$

The along-slope [Darcy velocity](../../../porous-media-flow.md#darcy-velocity) is therefore

$$
v_D=-\frac{k}{\mu}\left[p_x+(\rho-\Delta\rho)g\sin\theta\right]=\frac{kg\Delta\rho}{\mu}(\sin\theta-\cos\theta\,h_x).
$$

Define $u=kg\Delta\rho\sin\theta/\mu$. Integrating over depth gives the [volume flux per unit width](../../../fluid-mechanics.md#volume-flux-per-unit-width) $F=uh-u\cot\theta\,hh_x$. Local fluid-volume conservation, including [porosity](../../../porous-media-flow.md#porosity), is $\phi h_t+F_x=0$. Hence the [inclined porous gravity current](../../../porous-media-flow.md#inclined-porous-gravity-current) satisfies

$$
\boxed{\phi h_t=-\frac{kg\Delta\rho}{\mu}\sin\theta\left[h_x-\cot\theta\,(hh_x)_x\right].}
$$

The first term is upslope [advection](../../../fluid-mechanics.md#advection) driven by the [mass density](../../../fluid-mechanics.md#density) difference; the second is nonlinear hydrostatic spreading. The [Darcy velocity](../../../porous-media-flow.md#darcy-velocity) $u$ and the corresponding [pore velocity](../../../porous-media-flow.md#pore-velocity) $u/\phi$ must be distinguished.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

When the hydrostatic spreading term is small, the depth equation reduces to $h_t+c h_x=0$, where $c=u/\phi$. Its [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) have $x=c(t-t_0)$, and the depth is constant along each characteristic. At the inlet the imposed flux gives $uh(0,t_0)=Qe^{-t_0/\tau}$. Therefore $h_0=h(0,0)=Q/u$ in this advective approximation and

$$
\boxed{u=\frac{kg\Delta\rho}{\mu}\sin\theta,\qquad h(x,t)=h_0\exp\left[-\frac{t-\phi x/u}{\tau}\right].}
$$

This is the [advection limit of an inclined porous current](../../../porous-media-flow.md#advection-limit-of-an-inclined-porous-current), behind its leading nose and after the relevant characteristic has left the inlet. For injection starting into an empty aquifer, the advective support is $0<x<ut/\phi$.

The qualification “sufficiently large time” must refer to an advection-dominated outer region, not an exact solution of the full nonlinear equation. Substituting this exponential into the full equation leaves a nonzero spreading term. The next part quantifies when it can be neglected and explains the nonuniform leading-edge limit.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/1">1</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/1/solution">Solution</h5>

↑ **Parent:** [1](#1/iii/1)

For the proposed exponential profile, put $\ell=u\tau/\phi$. Then $h_x=h/\ell$ and $(hh_x)_x=2h^2/\ell^2$. Thus the exact ratio of the discarded spreading term to the retained advective term is

$$
\boxed{\mathcal E(x,t)=\frac{|u\cot\theta\,(hh_x)_x|}{|uh_x|}=\frac{2\phi h_0\cot\theta}{u\tau}\exp\left[-\frac{t-\phi x/u}{\tau}\right]\ll1.}
$$

This is a quantitative validity condition for the [advection limit of an inclined porous current](../../../porous-media-flow.md#advection-limit-of-an-inclined-porous-current). For a specified small tolerance $\eta>0$, at a fixed $x$ it is enough that the inlet characteristic has arrived and

$$
t-\frac{\phi x}{u}>\tau\log\left(\frac{2\phi h_0\cot\theta}{\eta u\tau}\right).
$$

If the logarithm is negative, arrival itself already gives this tolerance. A large-distance estimate comparing the overall current length $ct$ with a height-induced [pressure](../../../thermodynamics.md#pressure) length $h\cot\theta$ is $t\gg\phi h\cot\theta/u$, but the local gradient criterion above is the sharper test for this particular injection history.

At the advective nose, $x=ut/\phi$, the exponential factor is one. Therefore **large time alone is insufficient for uniform validity**: the outer profile also needs $2\phi h_0\cot\theta/(u\tau)\ll1$, and its abrupt nose needs an inner spreading layer. This limitation follows by direct substitution, not from a missing constant in the solution.

Indeed, with $\xi=x-ut/\phi$, the full equation becomes $h_t=D(hh_\xi)_\xi$, $D=u\cot\theta/\phi$. Once a finite-volume injection pulse is effectively over, nonlinear diffusion continues to broaden it. Dimensional balances give width $\ell_d\sim(DMt)^{1/3}$ and height $M/\ell_d$, where $M=\int h\,d\xi$ is the conserved area. A fixed exponential translating profile cannot be the uniform infinite-time limit of that equation. The printed formula is consequently an outer [advection](../../../fluid-mechanics.md#advection) approximation with the displayed smallness condition.

<h4 id="1/iii/2">2</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/2/solution">Solution</h5>

↑ **Parent:** [2](#1/iii/2)

Let $X(t)$ be the advancing nose into previously unoccupied pores. In the advective limit the interior flux is $uh$, while the exterior current thickness and flux are zero. Applying the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions) to the storage $\phi h$ gives

$$
\boxed{\phi\dot X=u,\qquad X(0)=0,\qquad X(t)=\frac{ut}{\phi}.}
$$

This is the leading-edge kinematic boundary condition. The outer depth immediately behind this nose is $h(X(t)^-,t)=h_0$, whereas ahead it is zero. A first-order [advection](../../../fluid-mechanics.md#advection) model allows this jump; imposing zero depth on its interior trace would contradict its characteristic solution.

For the full [inclined porous gravity current](../../../porous-media-flow.md#inclined-porous-gravity-current), the nose is instead resolved by a continuous spreading layer with $h(X,t)=0$. Taking the flux divided by depth at that interface gives $\dot X=(u/\phi)(1-\cot\theta\,h_x|_{X^-})$, when this one-sided derivative exists. Its leading outer value is $u/\phi$ only when the nose correction is negligible on the scale of the approximation. The zero-depth condition belongs to that resolved layer, not to the discontinuous outer profile itself.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

At a fixed location behind the advancing nose, the depth decreases after passage. A fall $-dh>0$ leaves the immobile fluid volume $s\phi(-dh)$ per unit length, so total local fluid storage changes by $\phi\,dh+s\phi(-dh)=\phi(1-s)\,dh$. The thinning-region equation is therefore

$$
\phi(1-s)h_t+uh_x=0.
$$

The inlet flux remains $uh(0,t)=Qe^{-t/\tau}$. Applying the [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics) with thinning-wave speed $u/[\phi(1-s)]$ gives the [residual-trapping attenuation of a porous current](../../../porous-media-flow.md#residual-trapping-attenuation-of-a-porous-current):

$$
\boxed{h(x,t)=h_0\exp\left[-\frac{t}{\tau}+\frac{\phi(1-s)x}{u\tau}\right],\qquad h_0=Q/u.}
$$

The nose advances into new pore space, which has no residual fluid yet, so its storage factor is still $\phi$ and its speed is still $u/\phi$. Consequently $X(t)=ut/\phi$ and the interior nose trace becomes $h_0e^{-st/\tau}$. Using the faster thinning-wave speed for the leading nose would incorrectly erase the attenuation caused by [capillary residual trapping](../../../porous-media-flow.md#capillary-residual-trapping). The broken printed reference “(??)” points to the preceding outer profile.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

The mobile fluid volume per unit well length includes the [porosity](../../../porous-media-flow.md#porosity):

$$
V(t)=\phi\int_0^{ut/\phi}h(x,t)\,dx.
$$

Integrating the [residual-trapping attenuation of a porous current](../../../porous-media-flow.md#residual-trapping-attenuation-of-a-porous-current) gives, for $0\leq s<1$,

$$
\boxed{V(t)=\frac{Q\tau}{1-s}\left(e^{-st/\tau}-e^{-t/\tau}\right).}
$$

This is mobile volume in the current; retained fluid outside its mobile thickness is not counted. Since $h_t=-h/\tau$ in the thinning region, the rate of accumulation of immobile retained volume is $\dot V_r=sV/\tau$. Direct differentiation verifies $\dot V+\dot V_r=Qe^{-t/\tau}$, so the mobile-volume expression obeys the overall injection balance.

Without [capillary residual trapping](../../../porous-media-flow.md#capillary-residual-trapping), $s=0$ gives $V=Q\tau(1-e^{-t/\tau})$. The limiting expression as $s\to1$ is $V=Qt e^{-t/\tau}$, though the local thinning equation degenerates at exactly $s=1$. Both limits provide useful consistency checks.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

For $0<s<1$, differentiation gives

$$
V'(t)=\frac{Q}{1-s}\left(e^{-t/\tau}-s e^{-st/\tau}\right).
$$

Its unique zero solves $e^{-(1-s)t/\tau}=s$. Therefore the [mobile-volume peak of an exponentially forced porous current](../../../porous-media-flow.md#mobile-volume-peak-of-an-exponentially-forced-porous-current) occurs at

$$
\boxed{t_{\max}=\frac{\tau\log(1/s)}{1-s}.}
$$

The derivative is initially positive and is negative after this time. More explicitly, at the stationary point $V''=-Qs e^{-st/\tau}/\tau<0$. Thus it is the global positive maximum, with

$$
\boxed{V_{\max}=Q\tau s^{s/(1-s)}.}
$$

The claim of a finite maximum requires nonzero [capillary residual trapping](../../../porous-media-flow.md#capillary-residual-trapping). At $s=0$ the mobile volume rises monotonically towards $Q\tau$ and the peak time tends to infinity. As $s\to1$, the limiting peak time is $\tau$ and the limiting maximum is $Q\tau/e$.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $X(t)$ denote the polymer–oil material interface, measured from the injection well, and let $U(t)$ be the [Darcy velocity](../../../porous-media-flow.md#darcy-velocity). [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) and uniform cross-sectional area make $U$ independent of $x$ in this planar model. Integrating [Darcy's law](../../../porous-media-flow.md#darcy-law) through the injected layer and the oil layer gives

$$
\Delta P=\frac{U}{k}\left[\mu X+\mu_h(L-X)\right].
$$

The material interface moves at the [pore velocity](../../../porous-media-flow.md#pore-velocity), so $X'=U/\phi$. Put $a=\mu-\mu_h$ and $A=\mu_hL$. Then $(A+aX)X'=k\Delta P/\phi$, which integrates from $X(0)=0$ to

$$
AX+\frac a2X^2=\frac{k\Delta P}{\phi}t.
$$

Thus the [fixed-pressure planar Darcy displacement](../../../porous-media-flow.md#fixed-pressure-planar-darcy-displacement) has

$$
\boxed{\dot X(t)=\frac{k\Delta P}{\phi\sqrt{(\mu_hL)^2+2(\mu-\mu_h)k\Delta P\,t/\phi}},\qquad U(t)=\phi\dot X(t).}
$$

For $a\ne0$, $X=[\sqrt{A^2+2ak\Delta P\,t/\phi}-A]/a$; its continuous $a=0$ limit is $X=k\Delta P\,t/(\phi\mu_hL)$. Positive layer [dynamic viscosities](../../../fluid-mechanics.md#dynamic-viscosity) ensure the resistance stays positive until breakthrough, which occurs at $t_b=\phi L^2(\mu+\mu_h)/(2k\Delta P)$. The formulas stop there, since the two-layer geometry then changes.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $Y(t)$ be the [porous thermal front](../../../porous-media-flow.md#thermal-front-in-a-porous-medium) and $X(t)$ the polymer front. With the literal stated convention for [Darcy velocity](../../../porous-media-flow.md#darcy-velocity),

$$
Y'=\Gamma U,\qquad X'=U/\phi,\qquad Y(0)=X(0)=0.
$$

Therefore $Y=\beta X$ with $\beta=\Gamma\phi$. This is [thermal-front retardation in Darcy flow](../../../porous-media-flow.md#thermal-front-retardation-in-darcy-flow). The region $0<x<Y$ is cold injected fluid of [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $\mu$; $Y<x<X$ is heated injected fluid of [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $b\mu$; $X<x<L$ is oil of [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $\mu_h$. The [pressure](../../../thermodynamics.md#pressure) drop is consequently

$$
\Delta P=\frac{U}{k}\left[\mu Y+b\mu(X-Y)+\mu_h(L-X)\right]=\frac{U}{k}\left[\mu_hL+(\mu_{\rm eff}-\mu_h)X\right],
$$

where $\mu_{\rm eff}=\mu[\beta+b(1-\beta)]$. Apply the preceding [fixed-pressure planar Darcy displacement](../../../porous-media-flow.md#fixed-pressure-planar-darcy-displacement) calculation with $\mu$ replaced by this effective [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity). The **polymer-front speed** is

$$
\boxed{\dot X=\frac{k\Delta P}{\phi\sqrt{(\mu_hL)^2+2(\mu_{\rm eff}-\mu_h)k\Delta P\,t/\phi}},\qquad\mu_{\rm eff}=\mu[b-(b-1)\Gamma\phi].}
$$

Its position solves $\mu_hLX+(\mu_{\rm eff}-\mu_h)X^2/2=k\Delta P\,t/\phi$, and $Y=\Gamma\phi X$. These expressions hold while both interfaces remain in the field, the [porous thermal front](../../../porous-media-flow.md#thermal-front-in-a-porous-medium) is sharp and stable, and $0\leq\Gamma\phi\leq1$. For $b=1$ the original constant-viscosity answer is recovered.

Sometimes a thermal retardation factor is defined relative to the [pore velocity](../../../porous-media-flow.md#pore-velocity) instead. Under that alternative definition one substitutes $\beta=\Gamma$ throughout. The factor of $\phi$ in the boxed answer follows specifically from the PDF's phrase “fraction of the Darcy speed.”

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

At the [porous thermal front](../../../porous-media-flow.md#thermal-front-in-a-porous-medium), the cold polymer solution behind has [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $\mu$, while the hot solution ahead has [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $b\mu>\mu$. Thus a more mobile region pushes a less mobile one. A forward protrusion locally reduces the length of high-resistance hot fluid and concentrates [Darcy flux](../../../porous-media-flow.md#darcy-velocity) into itself; it advances faster, amplifying the protrusion. This is the mechanism of the [Saffman–Taylor instability](../../../porous-media-flow.md#saffman-taylor-instability).

The leading polymer–oil interface can nevertheless be stable when the hot polymer [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) is at least the oil [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity). Stability of that leading interface does not guarantee stability of the trailing [porous thermal front](../../../porous-media-flow.md#thermal-front-in-a-porous-medium). Slow [thermal conduction](../../../thermodynamics.md#thermal-conduction) makes the latter sharp and offers weak short-wave smoothing; in practice it is the adverse [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) contrast across this front that can invalidate the assumed planar stable-flow calculation.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Take constant [Darcy velocity](../../../porous-media-flow.md#darcy-velocity) $U$ and work locally near a planar [porous thermal front](../../../porous-media-flow.md#thermal-front-in-a-porous-medium) moving at $V_T=\Gamma U$. Let $\xi=x-V_Tt$ and perturb its position by $\eta=\eta_0e^{\sigma t+ia y}$, with wavelength $\lambda=2\pi/|a|$. Neglect [thermal conduction](../../../thermodynamics.md#thermal-conduction) and regard the adjoining layers as semi-infinite on this disturbance scale. In each region, [Darcy's law](../../../porous-media-flow.md#darcy-law) and [incompressibility](../../../fluid-mechanics.md#incompressible-flow) imply that the [pressure](../../../thermodynamics.md#pressure) perturbation is harmonic, so the bounded [normal modes](../../../wave-equation.md#normal-mode) are

$$
p'_- =A_-e^{|a|\xi}e^{\sigma t+iay},\qquad p'_+=A_+e^{-|a|\xi}e^{\sigma t+iay}.
$$

Here the minus side is cold with [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $\mu$, and the plus side is hot with [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $b\mu$. The base [pressure gradients](../../../fluid-mechanics.md#pressure-gradient) are $p^0_{-,x}=-\mu U/k$ and $p^0_{+,x}=-b\mu U/k$. Linearizing [pressure continuity](../../../fluid-mechanics.md#pressure-continuity) at the displaced front yields

$$
A_--A_+=-\eta_0\frac{(b-1)\mu U}{k}.
$$

Continuity of the perturbed normal [Darcy velocity](../../../porous-media-flow.md#darcy-velocity) gives

$$
\delta U=-\frac{k|a|}{\mu}A_- =\frac{k|a|}{b\mu}A_+,
$$

so $A_+=-bA_-$. Therefore $\delta U=U|a|(b-1)\eta_0/(b+1)$. The thermal-front kinematic law is $\sigma\eta_0=\Gamma\delta U$, proving the [thermal-front viscous-fingering dispersion relation](../../../porous-media-flow.md#thermal-front-viscous-fingering-dispersion-relation)

$$
\boxed{\sigma(\lambda)=\frac{2\pi\Gamma U}{\lambda}\frac{b-1}{b+1}=\frac{2\pi V_T}{\lambda}\frac{b-1}{b+1}.}
$$

It is positive for $b>1$, zero for $b=1$, and negative for $b<1$. Without [thermal conduction](../../../thermodynamics.md#thermal-conduction) the model has no finite fastest wavelength: the positive growth rate increases without bound as $\lambda\to0$. A resolved thermal transition and diffusion regularize that short-wave limit.

For a material interface the kinematic coefficient would be $1/\phi$ rather than $\Gamma$. Thus, if the interface of interest were instead the hot polymer–oil interface, the same calculation would give $\sigma=2\pi(U/\phi)(\mu_h-b\mu)/[\lambda(\mu_h+b\mu)]$, the usual [planar viscous-fingering dispersion relation](../../../porous-media-flow.md#planar-viscous-fingering-dispersion-relation). This distinguishes the two interfaces and their speeds. The boxed thermal result uses the local planar approximation; distant wells or the other front modify the [pressure](../../../thermodynamics.md#pressure) eigenfunctions for wavelengths comparable to those separations.

## 3

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Here $k$ is [turbulent kinetic energy](../../../turbulence.md#turbulent-kinetic-energy) per unit mass, $k=\tfrac12\overline{u'^2+v'^2+w'^2}$, rather than the [permeability of a porous medium](../../../porous-media-flow.md#permeability-of-a-porous-medium) used in the porous-flow questions. The [K-epsilon turbulence model](../../../turbulence.md#k-epsilon-turbulence-model) represents the high-Reynolds-number transport of this energy and its [turbulent kinetic energy dissipation rate](../../../stokes-flow.md#turbulent-kinetic-energy-dissipation-rate) $\epsilon$.

In the $k$ equation, $d[(\nu_T/\sigma_k)k_y]/dy$ is the divergence of modeled [turbulent diffusion](../../../turbulence.md#eddy-diffusion), $\mathcal P$ is [mean-shear production](../../../turbulence.md#mean-shear-production-of-turbulent-kinetic-energy), and $-\epsilon$ is molecular conversion of fluctuation energy into heat. Statistical stationarity and fully developed flow have removed storage and streamwise [advection](../../../fluid-mechanics.md#advection) from this reduction.

In the $\epsilon$ equation, $d[(\nu_T/\sigma_\epsilon)\epsilon_y]/dy$ transports dissipation intensity; $C_{\epsilon1}\mathcal P\epsilon/k$ models its generation associated with energy production; and $-C_{\epsilon2}\epsilon^2/k$ models its destruction. The time scale $k/\epsilon$ supplies the source-rate dimension. The $\epsilon$ equation is a closure, not another energy-conservation equation. Finally, $\nu_T=C_\mu k^2/\epsilon$ has [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) dimensions and parametrizes [Reynolds stress](../../../turbulence.md#reynolds-stress) transport; $\sigma_k,\sigma_\epsilon$ set the relative diffusion strengths, and the remaining constants calibrate the closure.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let the mean streamwise [velocity](../../../classical-mechanics.md#velocity) be $U(y)$ and set $S=dU/dy>0$. The relevant covariance is $\overline{u'v'}<0$ on this half of the channel. The work of the [Reynolds stress](../../../turbulence.md#reynolds-stress) against the mean [shear rate](../../../viscous-fluid-flow.md#shear-rate) gives

$$
\boxed{\mathcal P=-\overline{u'v'}\frac{dU}{dy}.}
$$

The [eddy viscosity](../../../turbulence.md#eddy-viscosity) relation is $-\overline{u'v'}=\nu_T S$, so

$$
\boxed{\nu_T=\frac{-\overline{u'v'}}{dU/dy},\qquad\mathcal P=\nu_T\left(\frac{dU}{dy}\right)^2.}
$$

These are the kinematic-stress conventions, with the covariance measured per unit mass; inserting a stress measured in force per area would require division by [mass density](../../../fluid-mechanics.md#density).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [law of the wall](../../../continuum-mechanics.md#law-of-the-wall) in the logarithmic overlap region is $U/u_*=\kappa^{-1}\log(y/y_0)+B$, with the wall-scale reference absorbed in $y_0$ and $B$. Differentiating gives the **mean [shear rate](../../../viscous-fluid-flow.md#shear-rate)**

$$
\boxed{\frac{dU}{dy}=\frac{u_*}{\kappa y}.}
$$

Here $\kappa$ is the [Von Kármán constant](../../../continuum-mechanics.md#von-karman-constant). This form applies outside the viscous sublayer but well below the outer channel scale; it is not valid at the wall itself or at the channel centre.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Define the [friction velocity](../../../viscous-fluid-flow.md#shear-velocity) by $u_*=(|\tau_w|/\rho)^{1/2}$, where $\tau_w$ is the total tangential wall stress. It is a stress-derived [velocity](../../../classical-mechanics.md#velocity) scale, not the local mean [velocity](../../../classical-mechanics.md#velocity). In the overlap region, $y$ is small relative to the channel half-width, so the total stress is approximately its wall value. Molecular stress is small there, giving $-\overline{u'v'}\simeq u_*^2$.

Combining this [Reynolds stress](../../../turbulence.md#reynolds-stress) with the logarithmic shear gives $\mathcal P\simeq u_*^3/(\kappa y)$. For locally equilibrated wall [turbulence](../../../turbulence.md), energy transfer to small scales occurs over the local eddy turnover time and is balanced by molecular dissipation; energy storage and the net energy-transport divergence are small in the leading overlap-layer balance. Thus

$$
\boxed{\mathcal P\simeq\epsilon=\frac{u_*^3}{\kappa y}.}
$$

This is the [local turbulent kinetic energy balance](../../../turbulence.md#local-turbulent-kinetic-energy-balance). It is a modeling approximation rather than a general identity for all wall positions. The constant-energy solution derived next is consistent with it: its modeled $k$ diffusion term is exactly zero, while the $\epsilon$ diffusion term remains essential.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

The constant [Reynolds stress](../../../turbulence.md#reynolds-stress) and the logarithmic shear imply the [eddy viscosity](../../../turbulence.md#eddy-viscosity) $\nu_T=u_*\kappa y$. On the other hand the [K-epsilon model](../../../turbulence.md#k-epsilon-turbulence-model) gives $\nu_T=C_\mu k^2/\epsilon$. Insert $\epsilon=u_*^3/(\kappa y)$:

$$
u_*\kappa y=\frac{C_\mu k^2\kappa y}{u_*^3}.
$$

Canceling the positive factors yields $C_\mu k^2=u_*^4$. Since energy is nonnegative, the [log-layer solution of the k-epsilon model](../../../turbulence.md#log-layer-solution-of-the-k-epsilon-model) has

$$
\boxed{k=\frac{u_*^2}{\sqrt{C_\mu}},}
$$

independent of $y$ to this leading overlap-layer accuracy. In particular $k_y=0$, and the $k$ diffusion term vanishes, confirming the local production–dissipation balance in the energy equation.

<h3 id="3/vi">vi</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#3/vi)

Equating the two expressions for [eddy viscosity](../../../turbulence.md#eddy-viscosity) gives directly

$$
\epsilon=\frac{C_\mu k^2}{u_*\kappa y}.
$$

From the preceding part, $u_*^2=\sqrt{C_\mu}\,k$. Replace one factor of $k$ using that identity, and then replace $u_*$ itself by $C_\mu^{1/4}k^{1/2}$. This proves all three equivalent dissipation expressions:

$$
\boxed{\epsilon=\frac{C_\mu k^2}{u_*\kappa y}=\frac{C_\mu^{1/2}k u_*}{\kappa y}=\frac{C_\mu^{3/4}k^{3/2}}{\kappa y}.}
$$

Each is the same [turbulent kinetic energy dissipation rate](../../../stokes-flow.md#turbulent-kinetic-energy-dissipation-rate), with dimensions of [velocity](../../../classical-mechanics.md#velocity) cubed divided by length. Its equivalent friction-velocity form is $u_*^3/(\kappa y)$.

<h3 id="3/vii">vii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#3/vii)

Use $\nu_T=u_*\kappa y$, $\epsilon=u_*^3/(\kappa y)$, $k=u_*^2/\sqrt{C_\mu}$, and $\mathcal P=\epsilon$ in the dissipation equation. Its diffusion term is

$$
\frac{d}{dy}\left(\frac{\nu_T}{\sigma_\epsilon}\frac{d\epsilon}{dy}\right)=\frac{d}{dy}\left(-\frac{u_*^4}{\sigma_\epsilon y}\right)=\frac{u_*^4}{\sigma_\epsilon y^2}.
$$

The net modeled source is $(C_{\epsilon1}-C_{\epsilon2})\epsilon^2/k=-(C_{\epsilon2}-C_{\epsilon1})\sqrt{C_\mu}\,u_*^4/(\kappa^2y^2)$. Dividing the equation by $u_*^4/y^2$ and solving gives

$$
\boxed{\kappa^2=\sigma_\epsilon\sqrt{C_\mu}(C_{\epsilon2}-C_{\epsilon1}),\qquad\kappa=C_\mu^{1/4}\sqrt{\sigma_\epsilon(C_{\epsilon2}-C_{\epsilon1})}.}
$$

The physical [Von Kármán constant](../../../continuum-mechanics.md#von-karman-constant) is the positive root, requiring $C_{\epsilon2}>C_{\epsilon1}$ with positive $C_\mu,\sigma_\epsilon$. Neglecting dissipation diffusion would incorrectly require the two dissipation-equation constants to be equal. The parameter $\sigma_k$ does not enter because the constant $k$ profile has no energy-diffusion contribution.

## 4

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Set $S=\partial_z\overline u>0$ and $N^2=-(g/\rho_0)\partial_z\overline\rho>0$, using the constant reference [mass density](../../../fluid-mechanics.md#density) $\rho_0$ of the [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation). The [mean-shear production](../../../turbulence.md#mean-shear-production-of-turbulent-kinetic-energy) is $\mathcal P=-\overline{u'w'}S>0$. The stable [buoyancy](../../../fluid-mechanics.md#buoyancy) destruction is $B=(g/\rho_0)\overline{\rho'w'}>0$. Therefore

$$
\boxed{\mathrm{Ri}_f=\frac{B}{\mathcal P}=\frac{(g/\rho_0)\overline{\rho'w'}}{-\overline{u'w'}\,\partial_z\overline u},\qquad \mathrm{Ri}(z)=\frac{N^2}{S^2}=-\frac{g\,\partial_z\overline\rho}{\rho_0(\partial_z\overline u)^2}.}
$$

The [Flux Richardson number](../../../gravity-wave.md#flux-richardson-number) compares stable [buoyancy](../../../fluid-mechanics.md#buoyancy) destruction with shear production; the [gradient Richardson number](../../../gravity-wave.md#gradient-richardson-number) compares restoring stratification with mean [shear rate](../../../viscous-fluid-flow.md#shear-rate). They are generally different. The stationary energy budget gives $\epsilon=\mathcal P(1-\mathrm{Ri}_f)$, so positive dissipation in this balance requires $\mathrm{Ri}_f<1$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The fluctuation speed $q$ and the [integral scale of turbulence](../../../turbulence.md#integral-scale-of-turbulence) $L_u$ give a turnover time $L_u/q$. Dividing the velocity-variance scale $q^2$ by that time gives a [turbulent kinetic energy dissipation rate](../../../stokes-flow.md#turbulent-kinetic-energy-dissipation-rate) proportional to $q^3/L_u$. Likewise [mass density](../../../fluid-mechanics.md#density) variance $\overline{\rho'^2}$ removed over scalar mixing time $L_\rho/q$ gives the [density-variance dissipation rate](../../../turbulence.md#density-variance-dissipation-rate) proportional to $\overline{\rho'^2}q/L_\rho$. Absorbing dimensionless proportionality coefficients into the specified length scales gives

$$
\boxed{\epsilon=\frac{q^3}{L_u},\qquad\chi=\frac{\overline{\rho'^2}q}{L_\rho}.}
$$

These are integral-scale closure estimates, not exact consequences of dimensional analysis alone. In particular $q^2=2k$ for the turbulent-energy convention in Question 3. The normalization of $\chi$ is the one fixed by the printed scalar balance; if the budget is written for the full variance rather than one half of it, both production and dissipation terms acquire a factor two.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Write $F=\overline{\rho'w'}$. The density-variance balance gives $F\overline\rho_z=-\overline{\rho'^2}q/L_\rho$. From the definition of $C_\rho^2$, $\overline{\rho'^2}=F^2/(C_\rho^2q^2)$. For a nontrivial stratified turbulent state, substitute and divide by $F$:

$$
\boxed{F=-C_\rho^2L_\rho q\,\overline\rho_z.}
$$

This is positive for the stipulated stable negative [mass density](../../../fluid-mechanics.md#density) gradient. The [mean-shear production](../../../turbulence.md#mean-shear-production-of-turbulent-kinetic-energy) is $\mathcal P=C_uq^2S$. Substitute the scalar flux and $\epsilon=q^3/L_u$ into $\mathcal P=B+\epsilon$ to obtain

$$
\boxed{C_uq^2\frac{\partial\overline u}{\partial z}=-\frac{g}{\rho_0}C_\rho^2L_\rho q\frac{\partial\overline\rho}{\partial z}+\frac{q^3}{L_u}.}
$$

Equivalently $C_uSq^2=C_\rho^2L_\rho N^2q+q^3/L_u$. This is the [fixed-correlation equilibrium model for stratified turbulence](../../../turbulence.md#fixed-correlation-equilibrium-model-for-stratified-turbulence). The unstratified limit has $F=0$ and is obtained by continuity without performing the division by $F$ at zero. The [mass density](../../../fluid-mechanics.md#density) symbols in the actual PDF are $\rho$; the converted TeX's pressure-like $p$ symbols in this equation are transcription errors.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

For $q>0$, divide the two sink terms by $\mathcal P=C_uSq^2$. Put

$$
a=\frac{C_\rho^2L_\rho N^2}{C_uS},\qquad b=\frac1{L_uC_uS}.
$$

The requested ratio is

$$
\boxed{R(q)=\frac{B+\epsilon}{\mathcal P}=\frac{a}{q}+bq.}
$$

Here $b>0$ and $a\geq0$. With stable stratification $a>0$, $R$ diverges at both $q\downarrow0$ and $q\to\infty$, and has a single minimum at $q_m=\sqrt{a/b}$, with $R_{\min}=2\sqrt{ab}$. Increasing the stable density-gradient magnitude increases $a$, lifting the minimum and moving it rightward. When the [mass density](../../../fluid-mechanics.md#density) gradient vanishes, $a=0$ and the curve reduces to the straight line $R=bq$, with zero only as a limiting value at $q=0$ where the original ratio is undefined.

<a id="4/iv/image-sink-to-production-ratio-for-zero-subcritical-critical-and-supercritical-density-gradients"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73-equilibrium.png)

**[Figure 1](#4/iv/image-sink-to-production-ratio-for-zero-subcritical-critical-and-supercritical-density-gradients). Sink-to-production ratio for zero, subcritical, critical and supercritical density gradients**.

The plot uses $\widetilde q=bq=q/(L_uC_uS)$ and $\mathcal A=ab=[L_\rho C_\rho^2/(L_uC_u^2)]\mathrm{Ri}$, so $R=\widetilde q+\mathcal A/\widetilde q$. The horizontal line $R=1$ selects equilibria: two positive intersections for $0<\mathcal A<1/4$, one double intersection at $\mathcal A=1/4$, and none above it. The zero-gradient line has one positive equilibrium; its formal zero root before division by $q$ is the non-turbulent state.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

Differentiating $R=a/q+bq$ gives $R'=-a/q^2+b$, so for positive stratification its minimum has $q_m^2=a/b$. At that point

$$
\frac{B}{\mathcal P}=\frac{a}{q_m}=\sqrt{ab},\qquad\frac{\epsilon}{\mathcal P}=bq_m=\sqrt{ab}.
$$

Thus the two sinks are equal. The [buoyancy fraction of total turbulent sinks](../../../gravity-wave.md#buoyancy-fraction-of-total-turbulent-sinks) is always $B/(B+\epsilon)=1/2$ there. But the [Flux Richardson number](../../../gravity-wave.md#flux-richardson-number) defined in part (i) is instead

$$
\boxed{\mathrm{Ri}_f(q_m)=\sqrt{ab}=\frac{R_{\min}}2.}
$$

It equals $1/2$ **only when the minimum is also an equilibrium**, $R_{\min}=1$, namely at the critical gradient. This is the qualification needed for the printed assertion; an arbitrary minimum on a curve plotted away from equilibrium need not have $\mathrm{Ri}_f=1/2$.

For example choose closure parameters $C_u=C_\rho=1/4$, units with $L_u=L_\rho=S=1$, and $N^2=1/16$. Then $a=1/64$, $b=4$, $q_m=1/16$ and $R_{\min}=1/2$. The actual flux Richardson number at this minimum is $1/4$, while the [buoyancy](../../../fluid-mechanics.md#buoyancy) fraction of the total sinks is $1/2$. This is a concrete counterexample to the unqualified wording. With zero [mass density](../../../fluid-mechanics.md#density) gradient there is no positive interior minimum at all, and $\mathrm{Ri}_f=0$.

<h3 id="4/vi">vi</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#4/vi)

Divide the equilibrium equation by $q>0$ to get $bq^2-q+a=0$. Hence both positive branches, when $0<4ab<1$, are

$$
q_\pm=\frac{1\pm\sqrt{1-4ab}}{2b}=\frac{C_uSL_u}{2}\left[1\pm\sqrt{1-4\frac{L_\rho C_\rho^2}{L_uC_u^2}\mathrm{Ri}}\right].
$$

At equilibrium, $\mathrm{Ri}_f=a/q=1-bq$. Therefore the larger-speed branch $q_+$ gives the **printed flux Richardson number**

$$
\boxed{\mathrm{Ri}_f=\frac12\left[1-\sqrt{1-4\frac{L_\rho C_\rho^2}{L_uC_u^2}\mathrm{Ri}}\right],}
$$

while the smaller-speed branch gives the same formula with a plus sign before the square root. Solving the quadratic alone does not discard that second branch.

The larger-speed branch is selected by local kinetic-energy stability. If the same closures are used in the local energy evolution, $\tfrac12d(q^2)/dt=\mathcal P-B-\epsilon$. For $q>0$, divide by $q$ to obtain

$$
\dot q=C_uSq-C_\rho^2L_\rho N^2-q^2/L_u.
$$

Its linearization at $q_\pm$ has derivative $C_uS-2q_\pm/L_u=\mp C_uS\sqrt{1-4ab}$. The upper branch is therefore stable and the lower unstable in this local closure model.

The discriminant gives the **critical gradient Richardson number**

$$
\boxed{\mathrm{Ri}_c=\frac{L_uC_u^2}{4L_\rho C_\rho^2}.}
$$

At criticality the branches meet and $\mathrm{Ri}_f=1/2$. At zero stratification the stable positive solution is $q=C_uSL_u$ with $\mathrm{Ri}_f=0$; the lower algebraic root is $q=0$. This closure-dependent critical value is not automatically the inviscid $1/4$ criterion of the [Miles–Howard theorem](../../../gravity-wave.md#miles-howard-theorem).

<h3 id="4/vii">vii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#4/vii)

For $\mathrm{Ri}>\mathrm{Ri}_c$, the [fixed-correlation equilibrium model for stratified turbulence](../../../turbulence.md#fixed-correlation-equilibrium-model-for-stratified-turbulence) has $R_{\min}>1$. Thus [buoyancy](../../../fluid-mechanics.md#buoyancy) destruction plus dissipation exceeds shear production for every $q>0$, and the local kinetic-energy budget predicts decay rather than any positive statistically steady turbulent equilibrium. The stable and unstable turbulent branches have disappeared together at the critical point.

The implied outcome within this closure is suppression or decay of sustained [turbulence](../../../turbulence.md). It is not a proof that every physical stratified shear flow above this value must be permanently laminar: energy transport, external forcing, intermittent mixing or variable correlations and length-scale ratios can violate the model assumptions. As [turbulence](../../../turbulence.md) decays, the original fully turbulent high-Reynolds-number approximation itself ceases to apply. The critical Richardson number is consequently a prediction of the stated local closure, not a universal nonlinear stability bound.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
