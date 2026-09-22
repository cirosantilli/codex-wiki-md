# Paper 345

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_345.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_345.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)

## 1

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $u=psi_z$ and $w=-psi_x$, so [mass conservation](../../../continuum-mechanics.md#mass-conservation) for the two-dimensional [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) is automatic. Write $b$ for buoyancy and introduce the diffusive operators

$$
D_\nu=\partial_t-\nu\nabla^2,
\qquad
D_\kappa=\partial_t-\kappa\nabla^2.
$$

The [Linearized Boussinesq equations](../../../geophysical-fluid-dynamics.md#linearized-boussinesq-equations) are

$$
D_\nu u=-\frac1{\rho_0}p_x,
\qquad
D_\nu w=-\frac1{\rho_0}p_z+b,
\qquad
D_\kappa b=-N^2w.
$$

Taking the curl of the [momentum conservation](../../../classical-mechanics.md#momentum-conservation) equations eliminates the [pressure](../../../thermodynamics.md#pressure) and gives

$$
-D_\nu\nabla^2\psi=b_x.
$$

Apply $D_\kappa$ and use $D_\kappa b=N^2\psi_x$. Since the constant-coefficient [linear partial differential operators](../../../partial-differential-equation.md#linear-partial-differential-operator) commute,

$$
\boxed{\left[D_\nu D_\kappa\nabla^2+N^2\partial_x^2\right]\psi=0.}
$$

This is the viscous-diffusive [internal gravity wave](../../../gravity-wave.md#internal-wave) equation.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let the [group velocity](../../../wave-equation.md#group-velocity) make an angle $\theta$ above the horizontal. A convenient right-handed choice of rotated unit vectors is

$$
\widehat{\boldsymbol\xi}=(\sin\theta,-\cos\theta),
\qquad
\widehat{\boldsymbol\zeta}=(\cos\theta,\sin\theta).
$$

The first vector is parallel to the [wavevector](../../../continuum-mechanics.md#wavevector), the second is parallel to the [group velocity](../../../wave-equation.md#group-velocity), and their perpendicularity is the defining geometry of an [internal-wave phase and group velocity](../../../gravity-wave.md#internal-wave-phase-and-group-velocity). Thus

$$
\partial_x=\sin\theta\,\partial_\xi+\cos\theta\,\partial_\zeta,
\qquad
\nabla^2=\partial_\xi^2+\partial_\zeta^2.
$$

Writing $\Delta_{\xi\zeta}=\partial_\xi^2+\partial_\zeta^2$, the equation becomes

$$
\boxed{\left[(\partial_t-\nu\Delta_{\xi\zeta})(\partial_t-\kappa\Delta_{\xi\zeta})\Delta_{\xi\zeta}
+N^2(\sin\theta\,\partial_\xi+\cos\theta\,\partial_\zeta)^2\right]\psi=0.}
$$

For an inviscid [plane wave](../../../quantum-mechanics.md#plane-wave) proportional to $e^{i(k\xi-\omega t)}$, its [dispersion relation](../../../wave-equation.md#dispersion-relation) is $\omega=N\sin\theta$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $Z=\epsilon\zeta$ and seek the slowly attenuating [wave envelope](../../../wave-equation.md#envelope-waves) $A(Z)$ in

$$
\psi=A(Z)e^{i(k\xi-\omega t)}.
$$

At order $\epsilon^0$, the equation gives the [internal gravity wave](../../../gravity-wave.md#internal-wave) [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\omega^2=N^2\sin^2\theta.
$$

At order $\epsilon^1$, retaining one derivative of the slowly varying amplitude gives

$$
2i\omega k^4A+2iN^2k\sin\theta\cos\theta\,A_Z=0.
$$

Using $\omega=N\sin\theta$ therefore yields

$$
A_Z=-\frac{k^3}{N\cos\theta}A.
$$

Hence the leading [viscous attenuation of an internal-wave beam](../../../gravity-wave.md#viscous-attenuation-of-an-internal-wave-beam) is

$$
\boxed{\widetilde\psi(\zeta)=A_0
\exp\left(-\frac{\epsilon k^3}{N\cos\theta}\zeta\right)
=A_0e^{-k\zeta/\operatorname{Re}},}
\qquad
\boxed{\operatorname{Re}=\frac{N\cos\theta}{\epsilon k^2}.}
$$

The wave [energy density](../../../statistical-physics.md#energy-density), being quadratic in the amplitude, decays twice as rapidly in the exponent.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Set

$$
r=\tan\theta=\frac{\omega}{\sqrt{N^2-\omega^2}},
\qquad
s=\frac{H_0}{L},
$$

where $r$ is the magnitude of the [internal-wave ray](../../../gravity-wave.md#internal-wave-ray-tracing) slope and $s$ is the bottom slope. A rightward ray remains in the triangular basin precisely when its bottom reflection is [subcritical internal-wave reflection](../../../gravity-wave.md#subcritical-internal-wave-reflection), namely $r>s$. Therefore

$$
\boxed{\frac{NH_0}{\sqrt{L^2+H_0^2}}<\omega<N.}
$$

Conservation of frequency and of the component of the [wavevector](../../../continuum-mechanics.md#wavevector) tangent to the slope gives the [focusing power of internal-wave reflection](../../../gravity-wave.md#focusing-power-of-internal-wave-reflection)

$$
\boxed{\gamma=\frac{k_{\rm r}}{k_{\rm i}}
=\frac{\sin(\theta+\alpha)}{\sin(\theta-\alpha)}
=\frac{r+s}{r-s}
=\frac{L\omega+H_0\sqrt{N^2-\omega^2}}
{L\omega-H_0\sqrt{N^2-\omega^2}},}
$$

where $\tan\alpha=s$. In this range $\gamma>1$, so the reflected [wavelength](../../../wave-equation.md#wavelength) is shorter by the factor $\gamma$. The reflected normal [group velocity](../../../wave-equation.md#group-velocity) is smaller by $\gamma^2$; conservation of normal [energy flux](../../../physics.md#energy-flux) therefore increases the wavelength-averaged [energy density](../../../statistical-physics.md#energy-density) by

$$
\boxed{\overline E_{\rm r}=\gamma^2\overline E_{\rm i}.}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The incident [internal-wave ray](../../../gravity-wave.md#internal-wave-ray-tracing) has equation $z=-rx$. Intersecting it with the bottom $z=-H_0+sx$ gives

$$
x_1=\frac{H_0}{r+s}.
$$

Its distance to the slope is consequently

$$
\boxed{\ell=\frac{x_1}{\cos\theta}
=\frac{H_0}{\sin\theta+s\cos\theta}.}
$$

The subcritically reflected ray rises through the same vertical distance at angle $\theta$, so its next free-surface reflection is at

$$
\boxed{x_2=2x_1=\frac{2H_0}{r+s}.}
$$

On the first leg, [viscous attenuation of an internal-wave beam](../../../gravity-wave.md#viscous-attenuation-of-an-internal-wave-beam) multiplies the [energy density](../../../statistical-physics.md#energy-density) by $e^{-2k\ell/\operatorname{Re}}$. The bottom reflection multiplies it by $\gamma^2$ and changes the [wavenumber](../../../wave-equation.md#wavenumber) to $\gamma k$. Since the corresponding [Reynolds number](../../../fluid-mechanics.md#reynolds-number) is $\operatorname{Re}/\gamma^2$, attenuation on the second leg contributes $e^{-2\gamma^3k\ell/\operatorname{Re}}$. Ignoring boundary-layer enhancement as requested,

$$
\boxed{\overline E_2=\gamma^2\overline E_0
\exp\left[-\frac{2k\ell}{\operatorname{Re}}(1+\gamma^3)\right].}
$$

## 2

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [shallow-water approximation](../../../physics.md#shallow-water-approximation) requires $h/L\ll1$, a nearly [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure), negligible vertical acceleration, and approximately depth-independent horizontal velocity, concentration, and density. The large [Reynolds number](../../../fluid-mechanics.md#reynolds-number) allows viscous stress to be neglected away from thin boundary layers, while the deep ambient is taken to remain stationary.

For unit channel width, [volume conservation](../../../physics.md#volume-conservation), chemical conservation, and [mass conservation](../../../continuum-mechanics.md#mass-conservation) are respectively

$$
h_t+(uh)_x=w_e-w_d,
$$



$$
(\phi h)_t+(\phi uh)_x=-\phi w_d,
$$

and

$$
(\rho h)_t+(\rho uh)_x=\rho_0w_e-\rho w_d.
$$

Entrained ambient fluid contains no chemical and enters with density $\rho_0$; detrained fluid carries the local concentration and density. The ambient has no horizontal momentum, whereas detrained fluid carries horizontal momentum $\rho u$ per unit volume. The depth-integrated [momentum conservation](../../../classical-mechanics.md#momentum-conservation) law is therefore

$$
\frac{\partial(\rho uh)}{\partial t}
+\frac{\partial}{\partial x}\left(\rho u^2h+\frac12(\rho-\rho_0)gh^2\right)
=\boxed{-\rho u w_d},
$$

so $M=-\rho u w_d$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Define the concentration-dependent [reduced gravity](../../../reduced-gravity.md)

$$
g'(\phi)=\frac g{\rho_0}(R_1\phi+R_2\phi^2),
\qquad
g'_\phi=\frac g{\rho_0}(R_1+2R_2\phi).
$$

Under the [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation), the three [shallow water equations](../../../physics.md#shallow-water-equations) can be written in advective form as

$$
\phi_t+u\phi_x=-\frac{\phi w_e}{h},
$$



$$
h_t+uh_x+hu_x=w_e-w_d,
$$



$$
u_t+uu_x+g'h_x+\frac h2g'_\phi\phi_x=-\frac{uw_e}{h}.
$$

The coefficient matrix of this [quasilinear system](../../../partial-differential-equation.md#quasilinear-system) has [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed)

$$
\boxed{\lambda_0=u,\qquad \lambda_\pm=u\pm\sqrt{g'h}.}
$$

Thus this is a [hyperbolic system](../../../partial-differential-equation.md#hyperbolic-system) when $g'h>0$. Along the intermediate [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) $dx/dt=u$, the concentration obeys

$$
\boxed{\frac{D\phi}{Dt}=\phi_t+u\phi_x=-\frac{\phi w_e}{h}.}
$$

It decreases because ambient entrainment dilutes the chemical; detrainment does not change the concentration of a well-mixed parcel.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use a well-mixed [gravity-current box model](../../../reduced-gravity.md#gravity-current-box-model) of length $L(t)$ and depth $h(t)=V_0/L(t)$. Its fixed volume requires $w_e=w_d$. The integrated chemical balance and the standard [gravity-current front condition](../../../reduced-gravity.md#gravity-current-front-condition) are

$$
V_0\dot\phi=-w_dL\phi,
\qquad
\dot L=\operatorname{Fr}\sqrt{g'(\phi)h}
=\operatorname{Fr}\sqrt{\frac{gV_0}{\rho_0L}(R_1\phi+R_2\phi^2)}.
$$

These two [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation) are the required integral model.

First suppose $R_1>0$ and put

$$
a=\frac{R_2}{R_1},
\qquad
C=\frac{\operatorname{Fr}V_0}{w_d}
\sqrt{\frac{gV_0R_1}{\rho_0}}.
$$

Eliminating time gives

$$
L^{3/2}\frac{dL}{d\phi}
=-C\sqrt{\frac{1+a\phi}{\phi}}.
$$

With

$$
I(f)=\sqrt{f(1+af)}+\frac1{\sqrt a}\operatorname{arsinh}\sqrt{af},
$$

integration from $(L,\phi)=(L_0,1)$ yields

$$
\boxed{L^{5/2}=L_0^{5/2}+\frac52C\,[I(1)-I(\phi)].}
$$

As $t\to\infty$, the [concentration](../../../physics.md#concentration) tends to zero and the [runout length of a gravity current](../../../reduced-gravity.md#runout-length-of-a-gravity-current) is

$$
\boxed{L_\infty=
\left\{L_0^{5/2}+\frac52C\left[
\sqrt{1+a}+\frac1{\sqrt a}\operatorname{arsinh}\sqrt a
\right]\right\}^{2/5}.}
$$

The formula has a regular $a\to0$ limit. If $R_1=0<R_2$, direct integration instead gives

$$
L^{5/2}=L_0^{5/2}+\frac52\frac{\operatorname{Fr}V_0}{w_d}
\sqrt{\frac{gV_0R_2}{\rho_0}}(1-\phi),
$$

whose value at $\phi=0$ gives $L_\infty$.

## 3

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write $\widehat\rho(z)$ for the ambient density far from the wall and $\rho(z)$ for the density at the wall. Across the plume, let $y=x/b$ and use the prescribed triangular profiles

$$
w=W(1-y),
\qquad
\rho_p=\widehat\rho-(\widehat\rho-\rho)(1-y),
\qquad 0\leq y\leq1.
$$

Direct integration gives the [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate), [mass flux](../../../physics.md#mass-flux), [momentum flux](../../../physics.md#momentum-flux), and density-weighted [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux), all per unit radiator length:

$$
\boxed{V=\int_0^b w\,dx=\frac{bW}{2},}
$$



$$
\boxed{Q=\int_0^b\rho_pw\,dx
=\frac{bW}{6}(\widehat\rho+2\rho),}
$$



$$
\boxed{M=\int_0^b\rho_pw^2\,dx
=\frac{bW^2}{12}(\widehat\rho+3\rho),}
$$



$$
\boxed{F=\int_0^b g(\widehat\rho-\rho_p)w\,dx
=\frac{gbW}{3}(\widehat\rho-\rho).}
$$

These coefficients distinguish the [triangular-profile wall line plume](../../../turbulent-plume.md#triangular-profile-wall-line-plume) from a [top-hat plume model](../../../turbulent-plume.md#top-hat-plume-model).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Batchelor entrainment hypothesis](../../../turbulent-plume.md#batchelor-entrainment-hypothesis) takes the inflow speed through the plume's exposed outer edge to be $\alpha W$, where $\alpha$ is the [entrainment coefficient](../../../turbulent-plume.md#entrainment-coefficient). A wall plume has only one such edge, so $dV/dz=\alpha W$.

The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) replaces density by a constant reference value $\rho_0$ in inertia and mass flux while retaining the small density deficit in [buoyancy](../../../fluid-mechanics.md#buoyancy). It requires $|\widehat\rho-\rho|/\rho_0\ll1$. A sufficiently hot radiator can violate this near the source, where thermal expansion is large and the developed-plume description may also fail.

Put $B_0=F_0/\rho_0$ for the kinematic [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) per unit length. Dimensional analysis for a [line plume](../../../turbulent-plume.md#line-plume) gives

$$
W\sim B_0^{1/3},
\qquad
b\sim z,
\qquad
V\sim B_0^{1/3}z.
$$

The plume rise time is therefore $t_{\rm rise}\sim H/B_0^{1/3}$. Changing the room stratification requires a plume volume comparable with $XH$, so $t_{\rm room}\sim XH/V(H)\sim X/B_0^{1/3}$. Hence

$$
\frac{t_{\rm rise}}{t_{\rm room}}\sim\frac HX\ll1.
$$

The plume consequently follows the slowly changing ambient through a [quasi-steady approximation](../../../mathematics.md#quasi-steady-approximation) when $X\gg H$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Choose $\rho_0$ as a representative room density, for example the fresh-air density, and neglect relative density variations everywhere except in [buoyancy](../../../fluid-mechanics.md#buoyancy). With

$$
g'=\frac{\widehat\rho-\rho}{\rho_0}g,
$$

the triangular profiles give

$$
Q=\frac12\rho_0bW,
\qquad
M=\frac13\rho_0bW^2,
\qquad
F=\frac13\rho_0bWg'.
$$

Solving these algebraic relations,

$$
\boxed{W=\frac{3M}{2Q},
\qquad b=\frac{4Q^2}{3\rho_0M},
\qquad g'=\frac{3F}{2Q}.}
$$

The [Batchelor entrainment hypothesis](../../../turbulent-plume.md#batchelor-entrainment-hypothesis), vertical [momentum conservation](../../../classical-mechanics.md#momentum-conservation), and [mass conservation](../../../continuum-mechanics.md#mass-conservation) give

$$
\boxed{\frac{dV}{dz}=\alpha W,}
\qquad
\boxed{\frac{dQ}{dz}=\rho_0\alpha W=\frac{3\rho_0\alpha M}{2Q},}
\qquad
\boxed{\frac{dM}{dz}=\frac12\rho_0bg'=\frac{QF}{M}.}
$$

An ascending parcel entrains ambient fluid from progressively lower ambient density. With the [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency)

$$
N^2=-\frac g{\rho_0}\frac{d\widehat\rho}{dz},
$$

the change of ambient reference density subtracts $QN^2$ from its density-weighted [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux), so

$$
\boxed{\frac{dF}{dz}=-QN^2.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The source supplies the kinematic [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) $B_0=F_0/\rho_0$. The unstratified [line plume](../../../turbulent-plume.md#line-plume) velocity scale is $B_0^{1/3}$. Comparing this with the stratification time scale $N_0^{-1}$ gives the [stratified line-plume height scale](../../../turbulent-plume.md#stratified-line-plume-height-scale)

$$
\boxed{z_s\sim\frac{B_0^{1/3}}{N_0}
=\left(\frac{F_0}{\rho_0N_0^3}\right)^{1/3}.}
$$

If $z_s\gg H$, the initial plume is only weakly affected by the [stable density stratification](../../../gravity-wave.md#stable-density-stratification) and reaches the ceiling much like an unstratified wall plume. If $z_s\sim H$, its [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) falls substantially during the rise; it approaches neutral buoyancy near the upper room, overshoots because of its [momentum flux](../../../physics.md#momentum-flux), and spreads as a horizontal [buoyant intrusion](../../../turbulent-plume.md#buoyant-intrusion). If $z_s\ll H$, the plume reaches neutral buoyancy low in the room and forms a low intrusion after a modest overshoot. In each sketch the plume widens by [entrainment](../../../fluid-mechanics.md#fluid-entrainment), while increasing $N_0$ lowers the neutral-buoyancy and overshoot heights.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The final state is [displacement ventilation](../../../fluid-mechanics.md#displacement-ventilation): fresh air of density $\rho_0$ forms a cool lower layer, radiator-heated air forms a well-mixed upper layer, and the wall plume crosses their interface at height $h$. Steady [volume conservation](../../../physics.md#volume-conservation) requires the plume volume flux there to equal the imposed ventilation flux,

$$
V(h)=A.
$$

Below the interface the ambient is uniform, so $B_0=F_0/\rho_0$ is constant. Put $J=M/\rho_0$. The triangular-profile [wall line plume](../../../turbulent-plume.md#wall-line-plume) equations reduce to

$$
\frac{dV}{dz}=\alpha W=\frac{3\alpha J}{2V},
\qquad
\frac{dJ}{dz}=\frac{B_0V}{J}.
$$

The [pure plume](../../../turbulent-plume.md#pure-plume) conditions $V,J\to0$ at the radiator select the [similarity solution](../../../partial-differential-equation.md#similarity-solution)

$$
V(z)=C_LB_0^{1/3}z,
\qquad
C_L=\left(\frac{3\alpha}{2}\right)^{2/3}.
$$

Consequently the [displacement-ventilation interface height](../../../fluid-mechanics.md#displacement-ventilation-interface-height) is

$$
\boxed{h=\frac{A}{C_L(F_0/\rho_0)^{1/3}}
=\left(\frac{2}{3\alpha}\right)^{2/3}
\frac{A}{(F_0/\rho_0)^{1/3}}.}
$$

The upper-layer [reduced gravity](../../../reduced-gravity.md) follows from its steady buoyancy balance as $g'_u=B_0/A=F_0/(\rho_0A)$. The two-layer solution applies when the calculated interface satisfies $0<h<H$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
