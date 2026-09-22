# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20310.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
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
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [i](#4/e/i)
      - [Solution](#4/e/i/solution)
    - [ii](#4/e/ii)
      - [Solution](#4/e/ii/solution)

## 1

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

In natural units, the equilibrium [phase-space distribution function](../../../statistical-physics.md#phase-space-distribution-function) is

$$
f(\mathbf p)=\frac{1}{\exp[(E(\mathbf p)-\mu)/T]\mp1},
\qquad E(\mathbf p)=\sqrt{\mathbf p^2+m^2},
$$

where the minus sign gives the [Bose-Einstein distribution](../../../statistical-physics.md#bose-einstein-distribution) for [bosons](../../../quantum-mechanics.md#boson) and the plus sign gives the [Fermi-Dirac distribution](../../../statistical-physics.md#fermi-dirac-distribution) for [fermions](../../../quantum-mechanics.md#fermion).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Summing over the $g$ internal states, the [number density](../../../statistical-physics.md#number-density), [energy density](../../../statistical-physics.md#energy-density), and isotropic [pressure](../../../thermodynamics.md#pressure) are

$$
n=g\int\frac{d^3p}{(2\pi)^3}f(\mathbf p),
\qquad
\rho=g\int\frac{d^3p}{(2\pi)^3}E(\mathbf p)f(\mathbf p),
$$

and

$$
P=g\int\frac{d^3p}{(2\pi)^3}
\frac{\mathbf p^2}{3E(\mathbf p)}f(\mathbf p).
$$

The factor $\mathbf p^2/(3E)$ in the [kinetic pressure of an isotropic gas](../../../statistical-physics.md#kinetic-pressure-of-an-isotropic-gas) is the angular average of one diagonal component of the momentum flux.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

For an [ultrarelativistic particle](../../../special-relativity.md#ultrarelativistic-particle), $E\simeq|\mathbf p|$. Setting $\mu=0$ and writing the three-dimensional momentum integral radially gives

$$
n=\frac{gT^3}{2\pi^2}\int_0^\infty\frac{x^2\,dx}{e^x\mp1},
\qquad
\rho=\frac{gT^4}{2\pi^2}\int_0^\infty\frac{x^3\,dx}{e^x\mp1},
\qquad
P=\frac{\rho}{3}.
$$

The standard Bose integrals yield

$$
n_b=\frac{g\zeta(3)}{\pi^2}T^3,
\qquad
\rho_b=\frac{g\pi^2}{30}T^4,
\qquad
P_b=\frac{\rho_b}{3}.
$$

For [fermions](../../../quantum-mechanics.md#fermion), the corresponding integrals differ by the familiar factors

$$
n_f=\frac34\frac{g\zeta(3)}{\pi^2}T^3,
\qquad
\rho_f=\frac78\frac{g\pi^2}{30}T^4,
\qquad
P_f=\frac{\rho_f}{3}.
$$

**Thus the [number density](../../../statistical-physics.md#number-density) scales as $T^3$, while the [energy density](../../../statistical-physics.md#energy-density) and [pressure](../../../thermodynamics.md#pressure) scale as $T^4$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [entropy density](../../../thermodynamics.md#entropy-density) is

$$
s=\frac{\rho+P-\mu n}{T}.
$$

For the homogeneous cosmological plasma, adiabaticity gives the [cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) equation

$$
\nabla_\mu(su^\mu)=0,
\qquad
\dot s+3Hs=0,
$$

or equivalently $sa^3=\text{constant}$ in a comoving volume.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

After [thermal decoupling in cosmology](../../../cosmology.md#thermal-decoupling-in-cosmology), the collisionless relativistic species has $T_Xa=\text{constant}$. The still-coupled plasma separately conserves entropy, so $g_{*s}T_\gamma^3a^3$ remains constant. At decoupling $T_X=T_\gamma$, while at late times the coupled plasma contains only the two photon polarizations. Therefore the [temperature of a decoupled relativistic relic](../../../cosmology.md#temperature-of-a-decoupled-relativistic-relic) is

$$
\boxed{\frac{T_X}{T_\gamma}=\left(\frac{2}{g_*}\right)^{1/3}}.
$$

Here $g_*$ is understood as the effective entropy degrees of freedom in the plasma that remains coupled after $X$ decouples.

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For the [hilltop inflation](../../../cosmic-inflation.md#hilltop-inflation) potential,

$$
V'=-m^2\phi,
\qquad
V''=-m^2.
$$

The two [potential slow-roll parameters](../../../cosmic-inflation.md#potential-slow-roll-parameter) are consequently

$$
\epsilon_V
=\frac{M_{\rm Pl}^2m^4\phi^2}
{2(\Lambda^4-\tfrac12m^2\phi^2)^2}
\simeq\frac{M_{\rm Pl}^2m^4\phi^2}{2\Lambda^8}
$$

and

$$
\eta_V
=-\frac{M_{\rm Pl}^2m^2}{\Lambda^4-\tfrac12m^2\phi^2}
\simeq-\frac{M_{\rm Pl}^2m^2}{\Lambda^4}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Estimating the end of [slow-roll inflation](../../../cosmic-inflation.md#slow-roll-approximation) by $\epsilon_V(\phi_e)\simeq1$ and using the leading hilltop expression gives

$$
\boxed{\phi_e\simeq
\frac{\sqrt2\,\Lambda^4}{M_{\rm Pl}m^2}}.
$$

This is a formal leading-order estimate. Its self-consistency requires $m^2\phi_e^2\ll\Lambda^4$; if that condition fails, the full potential or the mechanism that ends inflation must be retained.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The homogeneous [inflaton](../../../cosmic-inflation.md#inflaton) obeys

$$
\ddot\phi+3H\dot\phi+V'(\phi)=0.
$$

Under the [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation), the acceleration and kinetic-energy corrections may be neglected, so the field equation and [Friedmann equation](../../../cosmology.md#friedmann-equations) become

$$
3H\dot\phi\simeq-V'=m^2\phi,
\qquad
H^2\simeq\frac{V}{3M_{\rm Pl}^2}
\simeq\frac{\Lambda^4}{3M_{\rm Pl}^2}.
$$

**Thus a positive field rolls away from the hilltop while $H$ is approximately constant.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [slow-roll e-fold count](../../../cosmic-inflation.md#slow-roll-e-fold-count) before the end of inflation is

$$
N(\phi)=\int_t^{t_e}H\,dt
=\frac1{M_{\rm Pl}^2}\int_{\phi_e}^{\phi}\frac{V}{V'}\,d\phi.
$$

At leading order near the hilltop, $V/V'\simeq-\Lambda^4/(m^2\phi)$, and hence

$$
N(\phi)\simeq
\frac{\Lambda^4}{M_{\rm Pl}^2m^2}
\log\frac{\phi_e}{\phi}.
$$

This has $N(\phi_e)=0$ and gives

$$
\boxed{\phi_{60}=\phi_e
\exp\!\left(-\frac{60M_{\rm Pl}^2m^2}{\Lambda^4}\right)}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Comparing the stated curvature [power spectrum](../../../probability-and-statistics.md#power-spectrum) with $P_{\mathcal R}=2\pi^2A_s/k^3$ at the pivot scale gives the [primordial scalar amplitude](../../../cosmic-inflation.md#primordial-scalar-amplitude)

$$
A_s=\frac{H^2}{8\pi^2\epsilon_VM_{\rm Pl}^2}
\simeq
\boxed{\frac{\Lambda^{12}}
{12\pi^2M_{\rm Pl}^6m^4\phi^2}}.
$$

The [scalar spectral index](../../../cosmic-inflation.md#scalar-spectral-index) is

$$
n_s-1\simeq-6\epsilon_V+2\eta_V
\simeq
\boxed{-\frac{3M_{\rm Pl}^2m^4\phi^2}{\Lambda^8}
-\frac{2M_{\rm Pl}^2m^2}{\Lambda^4}}.
$$

Sufficiently close to the hilltop, $\epsilon_V$ is suppressed by $\phi^2$ and the $\eta_V$ term controls the [spectral tilt](../../../cosmic-inflation.md#scalar-spectral-index).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Neglecting the $\epsilon_V$ contribution to the tilt, the observed value gives

$$
-\frac1{30}\simeq-\frac{2M_{\rm Pl}^2m^2}{\Lambda^4},
\qquad
\frac{M_{\rm Pl}^2m^2}{\Lambda^4}\simeq\frac1{60}.
$$

Part (d) then gives $\phi_{60}=e^{-1}\phi_e$. Using the formal end estimate from part (b), $\epsilon_V(\phi_{60})\simeq e^{-2}$. The amplitude relation therefore yields

$$
\frac{H}{M_{\rm Pl}}
=\sqrt{8\pi^2A_s\epsilon_V(\phi_{60})}
\simeq\frac{\sqrt{8\pi^2(2\times10^{-9})}}{e}
\simeq1.5\times10^{-4}.
$$

Thus the requested order-of-magnitude estimate is

$$
\boxed{H/M_{\rm Pl}\sim10^{-4}}.
$$

The simultaneous approximations make $\epsilon_V(\phi_{60})$ only moderately small, so this numerical result should be read as the order-of-magnitude estimate requested rather than a precision fit.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Local energy-momentum conservation is the vanishing [covariant divergence](../../../general-relativity.md#covariant-divergence) of the [energy-momentum tensor](../../../general-relativity.md#stress-energy-tensor):

$$
\boxed{\nabla_\mu T^\mu{}_{\nu}=0}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a mixed tensor,

$$
\nabla_\mu T^\mu{}_{\nu}
=\partial_\mu T^\mu{}_{\nu}
+\Gamma^\mu{}_{\mu\lambda}T^\lambda{}_{\nu}
-\Gamma^\lambda{}_{\mu\nu}T^\mu{}_{\lambda}.
$$

Write $T=\bar T+\delta T$ and $\Gamma=\bar\Gamma+\delta\Gamma$. The homogeneous background already satisfies $\bar\nabla_\mu\bar T^\mu{}_{\nu}=0$, and discarding products of two perturbations leaves

$$
\boxed{
\delta(\nabla_\mu T^\mu{}_{\nu})
=\partial_\mu\delta T^\mu{}_{\nu}
+\bar\Gamma^\mu{}_{\mu\lambda}\delta T^\lambda{}_{\nu}
-\bar\Gamma^\lambda{}_{\mu\nu}\delta T^\mu{}_{\lambda}
+\delta\Gamma^\mu{}_{\mu\lambda}\bar T^\lambda{}_{\nu}
-\delta\Gamma^\lambda{}_{\mu\nu}\bar T^\mu{}_{\lambda}}.
$$

This is simply the first variation of the tensor's [covariant derivative](../../../general-relativity.md#covariant-derivative).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For a spatial index $j$, the background [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) give

$$
\bar\Gamma^\mu{}_{\mu0}=3H,
\qquad
-\bar\Gamma^i{}_{0j}\delta T^0{}_i=-H\delta T^0{}_j,
\qquad
-\bar\Gamma^0{}_{ij}\delta T^i{}_0=-a^2H\delta T^j{}_0.
$$

Together with the $3H\delta T^0{}_j$ trace term, the first two contributions combine to $2H\delta T^0{}_j$. Varying the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) and contracting it with $\bar T^\mu{}_{\nu}=\operatorname{diag}(-\bar\rho,\bar P,\bar P,\bar P)$ gives

$$
\delta\Gamma^\mu{}_{\mu j}=\frac12\partial_j(h^\mu{}_{\mu}),
$$

and the surviving combination reduces to

$$
-(\bar\rho+\bar P)
\left(\frac12\partial_jh_{00}-Hh_{j0}\right).
$$

Consequently the spatial momentum equation is

$$
\boxed{
\partial_0\delta T^0{}_j+\partial_i\delta T^i{}_j
+2H\delta T^0{}_j-a^2H\delta T^j{}_0
-(\bar\rho+\bar P)
\left(\frac12\partial_jh_{00}-Hh_{j0}\right)=0}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

In [synchronous gauge in cosmology](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology), $h_{0\mu}=0$, so the explicit metric terms vanish. Symmetry of the covariant [energy-momentum tensor](../../../general-relativity.md#stress-energy-tensor) and the background metric imply

$$
\delta T^j{}_0=-a^{-2}\delta^{ji}\delta T^0{}_i.
$$

Hence the two expansion terms in part (c) combine to $3H\delta T^0{}_j$. Substituting the [scalar velocity potential](../../../linear-cosmological-perturbation-theory.md#scalar-velocity-potential) and [scalar anisotropic stress](../../../linear-cosmological-perturbation-theory.md#scalar-anisotropic-stress) definitions gives

$$
\boxed{\partial_0[(\bar\rho+\bar P)\partial_j\delta u]
+3H(\bar\rho+\bar P)\partial_j\delta u
+\partial_j\delta P
+\partial_j\nabla^2\pi^S=0.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Every term in part (d) is a spatial [gradient](../../../calculus.md#gradient). Extracting the longitudinal scalar coefficient, up to a spatially homogeneous function that can be absorbed into the zero mode, yields the [Cosmological Euler equation in synchronous gauge](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation-in-synchronous-gauge):

$$
\boxed{
\delta P+\nabla^2\pi^S
+\partial_0[(\bar\rho+\bar P)\delta u]
+3H(\bar\rho+\bar P)\delta u=0}.
$$

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

**Yes.** [Synchronous gauge in cosmology](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) uses freely falling time lines and sets the lapse and shift perturbations to zero, so no gravitational-potential force appears explicitly in this component of momentum conservation. Metric perturbations still affect the other field equations, the evolution of matter variables, and the relation between coordinate-dependent variables and gauge-invariant observables; synchronous gauge also retains residual gauge modes.

In [Newtonian gauge in cosmology](../../../linear-cosmological-perturbation-theory.md#newtonian-gauge), the time-time metric perturbation is a Newtonian gravitational potential. Its spatial [gradient](../../../calculus.md#gradient) therefore appears explicitly as a force term in the [Euler equation](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid). The difference is a coordinate representation of the same covariant conservation law.

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Taking the [divergence](../../../calculus.md#divergence) of the linear Euler equation and defining the [peculiar-velocity divergence](../../../cosmology.md#peculiar-velocity-divergence) $\theta=\nabla\mathbin\cdot\mathbf v$ gives

$$
\boxed{
\dot\theta+H\theta
=-\frac1{a\bar\rho}\nabla^2\delta P
-\frac1a\nabla^2\Phi}.
$$

The assumption of negligible [vorticity](../../../fluid-mechanics.md#vorticity) ensures that this longitudinal variable captures the velocity perturbation relevant to scalar density growth.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Differentiate the [linearized cosmological continuity equation](../../../linear-cosmological-density-perturbation.md#linearized-cosmological-continuity-equation), $\dot\delta=-\theta/a$, and use $\dot a/a=H$:

$$
\ddot\delta=-\frac{\dot\theta}{a}+\frac{H\theta}{a}.
$$

Substitution of part (a), followed by the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) $\nabla^2\Phi=4\pi Ga^2\bar\rho\,\delta$, yields

$$
\boxed{
\ddot\delta+2H\dot\delta
-\frac1{a^2\bar\rho}\nabla^2\delta P
-4\pi G\bar\rho\,\delta=0}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For a [barotropic equation of state](../../../cosmology.md#barotropic-equation-of-state), $\delta P=c_s^2\delta\rho=c_s^2\bar\rho\,\delta$. A spatial [Fourier mode](../../../fourier-analysis.md#fourier-mode) of comoving wavenumber $k$ therefore satisfies

$$
\ddot\delta_k+2H\dot\delta_k
+\left(\frac{c_s^2k^2}{a^2}-4\pi G\bar\rho\right)\delta_k=0.
$$

The [Jeans wavenumber](../../../linear-cosmological-density-perturbation.md#jeans-wavenumber) is defined by equality of the pressure and self-gravity terms:

$$
\boxed{k_J=\frac{a\sqrt{4\pi G\bar\rho}}{c_s}}.
$$

For $k\gg k_J$, pressure dominates and produces acoustic oscillations whose amplitude is affected by [Hubble friction](../../../cosmology.md#hubble-friction). For $k\ll k_J$, self-gravity dominates and a growing mode develops: this is [Jeans instability](../../../linear-cosmological-density-perturbation.md#jeans-instability).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Cold dark matter has $c_s=0$. During matter domination,

$$
a(t)\propto t^{2/3},
\qquad
H=\frac{2}{3t},
\qquad
\bar\rho=\frac{1}{6\pi Gt^2}.
$$

The density equation becomes

$$
\ddot\delta+\frac{4}{3t}\dot\delta
-\frac{2}{3t^2}\delta=0.
$$

Trying the [power law](../../../analysis.md#power-law) $\delta=t^p$ gives

$$
p(p-1)+\frac43p-\frac23=0,
$$

whose roots are $p=2/3$ and $p=-1$. Thus the [cosmic-time matter density modes](../../../linear-cosmological-density-perturbation.md#cosmic-time-matter-density-modes) are

$$
\boxed{\delta(t)=A t^{2/3}+B t^{-1}},
$$

and the leading growing mode is $\delta\propto t^{2/3}\propto a(t)$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/i">i</h4>

↑ **Parent:** [E](#4/e)

<h5 id="4/e/i/solution">Solution</h5>

↑ **Parent:** [I](#4/e/i)

The [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) gives

$$
\bar\rho_D\propto a^{-3(1+w)}=a^{-1}.
$$

For a spatially flat universe dominated by this component, the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $H^2\propto a^{-1}$. Integrating $\dot a/a\propto a^{-1/2}$ yields

$$
\boxed{a(t)\propto(t-t_*)^2,
\qquad H(t)=\frac{2}{t-t_*}}.
$$

This is accelerated expansion because $w=-2/3<-1/3$.

<h4 id="4/e/ii">ii</h4>

↑ **Parent:** [E](#4/e)

<h5 id="4/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/e/ii)

The dominant component is smooth, so only the subdominant matter density clusters. The cold-matter perturbation equation is therefore

$$
\ddot\delta+2H\dot\delta-4\pi G\bar\rho_m\delta=0,
\qquad
\bar\rho_m\propto a^{-3}.
$$

At late times, $a\gg1$, the source term is negligible compared with the expansion terms. Setting $\tau=t-t_*$ and using $H=2/\tau$ gives

$$
\ddot\delta+\frac4\tau\dot\delta\simeq0.
$$

It integrates to

$$
\boxed{\delta=C_1+C_2\tau^{-3}
=C_1+C_2a^{-3/2}}.
$$

The constant mode shows the [suppression of matter growth by smooth accelerated expansion](../../../linear-cosmological-density-perturbation.md#suppression-of-matter-growth-by-smooth-accelerated-expansion); the second mode decays.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
