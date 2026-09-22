# Paper 345

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_345.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_345.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
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

## 1

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $W_f$ be the vertical velocity of the carrier fluid. Each species has its isolated [Stokes settling velocity](../../../fluid-mechanics.md#stokes-settling-velocity) relative to that fluid, so $W_i=W_f+\widehat W_i$. The mixture has no imposed vertical [volumetric flow rate](../../../fluid-mechanics.md#volumetric-flow-rate). Using the [particle volume fractions](../../../fluid-mechanics.md#particle-volume-fraction), its zero-volume-flux condition is

$$
(1-\phi_1-\phi_2)W_f+\phi_1W_1+\phi_2W_2=0.
$$

Substitution of $W_i=W_f+\widehat W_i$ gives the common carrier-fluid backflow

$$
W_f=-\phi_1\widehat W_1-\phi_2\widehat W_2.
$$

Consequently the [hindered settling](../../../fluid-mechanics.md#hindered-settling) velocities are

$$
W_1=(1-\phi_1)\widehat W_1-\phi_2\widehat W_2,
\qquad
W_2=(1-\phi_2)\widehat W_2-\phi_1\widehat W_1.
$$

The same $W_f$ appears for both populations precisely because every particle is assumed to feel the same volume-averaged backflow.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Local [mass conservation](../../../continuum-mechanics.md#mass-conservation) of each particle species gives the [system of conservation laws](../../../partial-differential-equation.md#system-of-conservation-laws)

$$
\partial_t\phi_i+\partial_z(\phi_iW_i)=0,
\qquad i=1,2.
$$

For $\boldsymbol\phi=(\phi_1,\phi_2)^T$ and flux $F_i=\phi_iW_i$, the [flux Jacobian](../../../partial-differential-equation.md#flux-jacobian) is

$$
A(\boldsymbol\phi)=
\begin{pmatrix}
(1-2\phi_1)\widehat W_1-\phi_2\widehat W_2&-\phi_1\widehat W_2\\
-\phi_2\widehat W_1&(1-2\phi_2)\widehat W_2-\phi_1\widehat W_1
\end{pmatrix}.
$$

Writing its entries as $A_{ij}$, the two [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed) are its [eigenvalues](../../../linear-operator-theory.md#eigenvalue)

$$
\lambda_\pm
=\frac{A_{11}+A_{22}}2
\pm\frac12\sqrt{(A_{11}-A_{22})^2+4A_{12}A_{21}}.
$$

The discriminant is nonnegative because $A_{12}A_{21}=\phi_1\phi_2\widehat W_1\widehat W_2\geq0$, so positive concentrations of two settling species give real characteristics.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Set

$$
s=\phi_1+\phi_2,
\qquad
c=\frac{\phi_1}{s},
$$

where $s>0$. Applying [first-order perturbation of a simple eigenvalue](../../../linear-operator-theory.md#first-order-perturbation-of-a-simple-eigenvalue) to the [flux Jacobian](../../../partial-differential-equation.md#flux-jacobian), or expanding its quadratic formula directly, separates the characteristic that changes total concentration from the characteristic that changes composition:

$$
\lambda_s
=\widehat W(1-2s)\bigl[1-\epsilon(2c-1)\bigr]+O(\epsilon^2),
$$



$$
\lambda_c
=\widehat W\bigl[1-s+\epsilon(2c-1)(1+s)\bigr]+O(\epsilon^2).
$$

At $\epsilon=0$, both species move with the common hindered velocity $\widehat W(1-s)$. Summing their conservation laws gives

$$
s_t+\widehat W\,\partial_z\bigl[s(1-s)\bigr]=0,
$$

so the total concentration is a nonlinear [kinematic wave](../../../partial-differential-equation.md#kinematic-wave):

$$
\frac{dz}{dt}=\widehat W(1-2s),
\qquad
\frac{ds}{dt}=0.
$$

Taking the ratio $c=\phi_1/s$ instead gives the [composition wave in a bidisperse suspension](../../../fluid-mechanics.md#composition-wave-in-a-bidisperse-suspension)

$$
c_t+\widehat W(1-s)c_z=0,
$$

and hence

$$
\frac{dz}{dt}=\widehat W(1-s),
\qquad
\frac{dc}{dt}=0.
$$

These are the requested leading-order [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation) along the two characteristic families.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Let the fixed current volume per unit channel width be

$$
V_0=Lh=L_0h_0.
$$

A suitable high-[Reynolds number](../../../fluid-mechanics.md#reynolds-number) deep-ambient [gravity-current front condition](../../../reduced-gravity.md#gravity-current-front-condition) is

$$
\dot L=\operatorname{Fr}\sqrt{g'h},
$$

where the order-one [Froude number](../../../reduced-gravity.md#froude-number) $\operatorname{Fr}$ records the selected front closure. In the dilute limit the mixture's [reduced gravity](../../../reduced-gravity.md) is

$$
g'=\frac g{\rho_a}
\sum_{i=1}^2(\rho_i-\rho_a)\phi_i,
$$

with ambient and carrier-fluid density $\rho_a$.

The well-mixed particle volume of species $i$ is $V_0\phi_i$. Its deposition rate through the base of length $L$ is $L\widehat W_i\phi_i$, where $\widehat W_i<0$. The resulting [gravity-current box model](../../../reduced-gravity.md#gravity-current-box-model) is therefore

$$
h=\frac{V_0}{L},
\qquad
\dot L=\operatorname{Fr}\sqrt{\frac{V_0g'}L},
\qquad
\dot\phi_i=\frac{L\widehat W_i}{V_0}\phi_i.
$$

It conserves fluid volume while suspended particle volume, and therefore the driving buoyancy, decreases by deposition.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

When $\widehat W_1=\widehat W_2=\widehat W$, both concentrations acquire the same decay factor. The total reduced gravity consequently obeys

$$
\dot g'=\frac{\widehat W L}{V_0}g'.
$$

Eliminating time with the front equation gives

$$
\frac{d\sqrt{g'}}{dL}
=\frac{\widehat W L^{3/2}}{2\operatorname{Fr}V_0^{3/2}}.
$$

Integration from the initial state yields

$$
\sqrt{g'(L)}
=\sqrt{\widetilde g'}
+\frac{\widehat W}{5\operatorname{Fr}V_0^{3/2}}
\left(L^{5/2}-L_0^{5/2}\right),
$$

where

$$
\widetilde g'
=\frac g{\rho_a}
\left[(\rho_1-\rho_a)\widetilde\phi_1
+(\rho_2-\rho_a)\widetilde\phi_2\right].
$$

The [particle-laden gravity current](../../../reduced-gravity.md#particle-laden-gravity-current) reaches its [runout length of a gravity current](../../../reduced-gravity.md#runout-length-of-a-gravity-current) when $g'$ vanishes. Since $\widehat W<0$,

$$
L_\infty
=\left[
L_0^{5/2}
+5\operatorname{Fr}
\frac{(L_0h_0)^{3/2}\sqrt{\widetilde g'}}{|\widehat W|}
\right]^{2/5}.
$$

**Thus $C=5\operatorname{Fr}$ for the stated front condition; the common normalization $\operatorname{Fr}=1$ gives $C=5$.**

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

Because $\widehat W<0$, species 1 now settles more slowly and species 2 more rapidly than in the equal-speed case. The supplied inequality says that species 2 provides the larger initial particle-density contribution to the [reduced gravity](../../../reduced-gravity.md); with exact Boussinesq density contrasts, the corresponding condition is $\widetilde\phi_1(\rho_1-\rho_a)<\widetilde\phi_2(\rho_2-\rho_a)$. The dominant buoyancy contribution is therefore removed earlier, so $g'(t)$ and the [gravity-current front condition](../../../reduced-gravity.md#gravity-current-front-condition) fall below their equal-settling values at first order in $\epsilon$. The runout length decreases. The slower loss of the weaker species-1 contribution only partly compensates for this effect.

## 2

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write the density as a hydrostatic reference profile $\widehat\rho(z)$ plus a small perturbation $\rho'$, and define buoyancy and [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency) by

$$
b=-\frac g{\rho_0}\rho',
\qquad
N^2=-\frac g{\rho_0}\frac{d\widehat\rho}{dz}>0.
$$

The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) to the [Navier-Stokes equation](../../../viscous-fluid-flow.md#navier-stokes-equation), together with [mass conservation](../../../continuum-mechanics.md#mass-conservation), is

$$
\nabla\mathbin\cdot\mathbf u=0,
$$



$$
\frac{D\mathbf u}{Dt}
=-\nabla\pi+b\mathbf e_z+\nu\nabla^2\mathbf u,
\qquad
\frac{Db}{Dt}+N^2w=\kappa\nabla^2b,
$$

where $D/Dt$ is the [material derivative](../../../continuum-mechanics.md#material-derivative), $\nu$ is [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity), and $\kappa$ is [mass diffusivity](../../../fluid-mechanics.md#mass-diffusivity). Linearizing about rest and eliminating pressure and buoyancy gives

$$
\left[(\partial_t-\kappa\nabla^2)(\partial_t-\nu\nabla^2)\nabla^2
+N^2\partial_x^2\right]w=0.
$$

For a [plane wave](../../../quantum-mechanics.md#plane-wave) proportional to $e^{i(kx+mz-\omega t)}$, with $K^2=k^2+m^2$, the viscous-diffusive [dispersion relation](../../../wave-equation.md#dispersion-relation) is

$$
(-i\omega+\nu K^2)(-i\omega+\kappa K^2)K^2+N^2k^2=0.
$$

In the inviscid limit this becomes

$$
\omega_0^2=\frac{N^2k^2}{k^2+m^2}.
$$

For weak diffusion the two oscillatory roots are

$$
\omega=\pm\omega_0-\frac i2(\nu+\kappa)K^2
+O\bigl((\nu-\kappa)^2K^4/\omega_0\bigr),
$$

so a freely evolving Fourier mode decays.

A single plane wave is also an exact solution of the nonlinear equations. Every field depends only on its phase $\Theta=\mathbf k\mathbin\cdot\mathbf x-\omega t$, while [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) gives $\mathbf u\mathbin\cdot\mathbf k=0$. Therefore $\mathbf u\mathbin\cdot\nabla$ annihilates both $\mathbf u(\Theta)$ and $b(\Theta)$, and all nonlinear advection terms vanish.

For a boundary-forced wave with real $\omega$, nonzero $\nu$ or $\kappa$ instead makes the bulk vertical wavenumber complex, attenuating the propagating beam. Because diffusion raises the spatial order of the equations, additional short vertical-wavenumber roots form viscous and scalar [boundary layers](../../../continuum-mechanics.md#boundary-layer); they allow a no-slip velocity condition and a scalar no-flux condition to accompany impermeability. These layers and bulk attenuation become essential near [critical internal-wave reflection](../../../gravity-wave.md#critical-internal-wave-reflection), where the inviscid reflected wavelength collapses.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $\theta$ be the angle made by the [group velocity](../../../wave-equation.md#group-velocity) ray with the horizontal. The [internal gravity wave](../../../gravity-wave.md#internal-wave) dispersion relation gives

$$
\sin\theta=\frac{|\omega|}{N},
\qquad
\tan\theta=\frac{|k|}{|m|}
=\frac{|\omega|}{\sqrt{N^2-\omega^2}}.
$$

Each sawtooth face changes height by $2h_0$ over horizontal distance $\lambda_T/2$, so its slope magnitude is

$$
s_T=\frac{4h_0}{\lambda_T}.
$$

The [internal-wave slope criticality](../../../gravity-wave.md#internal-wave-slope-criticality) criterion is $s_T<\tan\theta$. Hence reflection is subcritical for

$$
\boxed{
\frac{Ns_T}{\sqrt{1+s_T^2}}<|\omega|<N
}.
$$

In the corresponding [internal-wave ray tracing](../../../gravity-wave.md#internal-wave-ray-tracing) sketch, every incident ray meets one planar face and leaves it into the fluid at the same angle $\theta$ to the horizontal. The reflected ray is steeper than either face, so it clears the sawtooth rather than running into an adjacent corner.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For a face of signed slope $s$, conservation of frequency and tangential [wavenumber](../../../wave-equation.md#wavenumber) gives, on the branch relevant to an incident downward-right ray,

$$
k_r=k\frac{1+s\mu}{1-s\mu},
\qquad
\mu=\frac{|m|}{|k|}=\cot\theta.
$$

At $s\mu=1$, the reflected wavenumber diverges and the reflected [group velocity](../../../wave-equation.md#group-velocity) becomes tangent to the face. On a supercritical face the denominator changes sign: horizontal propagation reverses and rays from the two faces are directed towards a sawtooth corner. Successive reflections therefore focus energy and shorten the wavelength.

The inviscid ray pattern cannot persist indefinitely. Near-critical focusing amplifies gradients until [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity), [mass diffusivity](../../../fluid-mechanics.md#mass-diffusivity), nonlinear wave steepening, and wave breaking matter; a real corner is also rounded on some finite scale. These effects replace the singular ray construction by dissipative boundary layers, mixing, and a finite-width reflected beam.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The maximum boundary slope is $s_{\max}=h_0k_T$, so [subcritical internal-wave reflection](../../../gravity-wave.md#subcritical-internal-wave-reflection) requires

$$
h_0k_T<\frac{|\omega|}{\sqrt{N^2-\omega^2}},
$$

or equivalently

$$
\boxed{
\frac{Nh_0k_T}{\sqrt{1+h_0^2k_T^2}}<|\omega|<N
}.
$$

Take $k,m>0$ without loss of generality, put

$$
\mu=\frac mk=\sqrt{\frac{N^2}{\omega^2}-1},
\qquad
p_j=k+jk_T,
$$

and write the incident field as the imaginary part of $\widetilde w_i e^{i(kx+mz-\omega t)}$. The [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) on $z=h(x)$ is

$$
[w-u h_x]_{z=h(x)}=0.
$$

For a flat boundary the reflected wave is $-\widetilde w_i\sin(kx-mz-\omega t)$. Expanding the boundary condition in a [Taylor expansion](../../../calculus.md#taylor-expansion) about $z=0$ creates the [topographic sidebands of an internal gravity wave](../../../gravity-wave.md#topographic-sideband-of-an-internal-gravity-wave). With upward-radiating vertical wavenumber $-\mu|p_j|$, their complex amplitudes through second order are

$$
B_0=-\widetilde w_i
+\frac{\mu^2h_0^2k}{2}
\left(p_1+|p_{-1}|\right)\widetilde w_i,
$$



$$
B_1=-\mu h_0p_1\widetilde w_i,
\qquad
B_{-1}=\mu h_0p_{-1}\widetilde w_i,
$$



$$
B_2=-\frac12\mu^2h_0^2p_1p_2\widetilde w_i,
\qquad
B_{-2}=-\frac12\mu^2h_0^2|p_{-1}|p_{-2}\widetilde w_i.
$$

Thus the general compact result is

$$
w_r(x,z,t)
=\operatorname{Im}\left\{
e^{-i\omega t}
\sum_{j=-2}^{2}B_j
e^{ip_jx-i\mu|p_j|z}
\right\}+O(h_0^3).
$$

For the convenient nondegenerate case $k>2k_T$, all displayed sideband wavenumbers are positive. Defining $\Theta_j=p_jx-\mu p_jz-\omega t$, the same answer is the explicitly real formula

$$
\begin{aligned}
\frac{w_r}{\widetilde w_i}
={}&\left(-1+\mu^2h_0^2k^2\right)\sin\Theta_0\\
&+\mu h_0\left(p_{-1}\sin\Theta_{-1}-p_1\sin\Theta_1\right)\\
&-\frac{\mu^2h_0^2}{2}
\left(p_{-1}p_{-2}\sin\Theta_{-2}+p_1p_2\sin\Theta_2\right)
+O(h_0^3).
\end{aligned}
$$

Validity requires a linear incident wave, an inviscid uniformly stratified bulk, an outgoing-radiation condition, strict separation from critical slopes, and small boundary excursions for every retained mode, in particular $h_0k_T\ll1$ and $\mu h_0\max_{|j|\leq2}|p_j|\ll1$. A vanishing $p_j$ is a degenerate zero-horizontal-wavenumber case and must be treated by taking the corresponding zero-amplitude limit rather than dividing by $p_j$.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

If $h_0k_T>\tan\theta$, each period contains two critical points satisfying $|h_x|=\tan\theta$, with supercritical intervals around the steepest parts. [Internal-wave ray tracing](../../../gravity-wave.md#internal-wave-ray-tracing) sends neighbouring reflected rays towards caustics attached to those critical points; rays can reverse horizontal direction in the supercritical intervals and intersect rays reflected elsewhere on the sinusoid. At equality the inviscid reflected wavelength collapses locally. The physical pattern is therefore a set of intense finite-width beams and mixing regions once viscosity, scalar diffusion, and wave breaking regularize the ray caustics.

## 3

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) replaces density by a common reference value $\rho_0$ in inertia, [mass conservation](../../../continuum-mechanics.md#mass-conservation), and pressure acceleration, while retaining small density differences in the gravitational buoyancy term. It gives [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) and is appropriate here when

$$
\frac{|\rho_1-\rho_H|}{\rho_0}\ll1,
$$

even though those small differences drive the room-scale motion. It would fail for order-one thermal density contrasts or strongly compressible ventilation.

The [Batchelor entrainment hypothesis](../../../turbulent-plume.md#batchelor-entrainment-hypothesis) sets the mean inflow speed across a turbulent plume edge to $\alpha$ times a representative axial plume speed, where $\alpha$ is the [entrainment coefficient](../../../turbulent-plume.md#entrainment-coefficient). It closes integral plume balances by relating plume growth to its speed. Applied here, it produces an entraining axisymmetric warm plume above the floor source and a one-sided cold [wall line plume](../../../turbulent-plume.md#wall-line-plume) below the vent. Treating both as turbulent [top-hat plume models](../../../turbulent-plume.md#top-hat-plume-model) neglects source regions, detailed profiles, wall friction, interaction between the two plumes, and the finite thickness of the density interface; these are the principal modelling assumptions.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Define the indoor-to-outdoor [reduced gravity](../../../reduced-gravity.md)

$$
g'_V=\frac{g(\rho_1-\rho_H)}{\rho_0}>0.
$$

Because the whole opening lies above the interface, its indoor side contains upper-layer fluid of density $\rho_H$. Under [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure), the pressure difference varies linearly about a [neutral pressure level](../../../fluid-mechanics.md#neutral-pressure-level). Equal opening geometry and equal [discharge coefficients](../../../fluid-mechanics.md#discharge-coefficient) for inflow and outflow put that level at the vent midpoint. At vertical distance $y$ from it, the ideal [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) gives speed $\sqrt{2g'_V|y|}$.

Writing $Q_V$ for either one-way [volumetric flow rate](../../../fluid-mechanics.md#volumetric-flow-rate), integration over one half of the opening gives

$$
Q_V
=C_dL\int_0^{H'/2}\sqrt{2g'_Vy}\,dy
=\frac{C_d}{3}LH'^{3/2}\sqrt{g'_V}.
$$

The total unsigned exchange is $2Q_V$. The ideal sharp-edged inviscid model has $C_d=1$; an empirical $C_d<1$ represents contraction and losses.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For plume radius $r$, top-hat speed $U$, and plume reduced gravity $g'_B$, define the [volumetric flow rate](../../../fluid-mechanics.md#volumetric-flow-rate), momentum flux, and [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux)

$$
Q_B=\pi r^2U,
\qquad
M_B=\pi r^2U^2,
\qquad
B=\pi r^2Ug'_B.
$$

The integral balances for a steady [axisymmetric pure plume](../../../turbulent-plume.md#axisymmetric-pure-plume) in a uniform lower layer are

$$
\frac{dQ_B}{dz}=2\pi\alpha rU,
\qquad
\frac{dM_B}{dz}=\pi r^2g'_B=\frac BU,
\qquad
\frac{dB}{dz}=0.
$$

The source is at the plume's virtual origin $z=0$. Solving these equations gives

$$
r(z)=\frac{6\alpha}{5}z,
$$



$$
U(z)=
\left(\frac{25B}{48\pi\alpha^2}\right)^{1/3}z^{-1/3}.
$$

It is useful to define

$$
C_P=\frac{6\alpha}{5}
\left(\frac{9\alpha}{10}\right)^{1/3}\pi^{2/3}.
$$

Then the remaining similarity laws take the compact form

$$
Q_B(z)=C_PB^{1/3}z^{5/3},
\qquad
g'_B(z)=C_P^{-1}B^{2/3}z^{-5/3}.
$$

The second relation also follows immediately from conservation of [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux), $B=Q_Bg'_B$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Measure downward distance from the [plume virtual origin](../../../turbulent-plume.md#plume-virtual-origin) by

$$
s=z_o-z>0,
$$

and let $\mathcal B$ be the magnitude of the cold plume's [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux) per unit span. A one-sided [wall line plume](../../../turbulent-plume.md#wall-line-plume) with width $b$, downward speed $W>0$, and reduced-gravity magnitude $g'$ satisfies

$$
\frac d{ds}(bW)=\alpha W,
\qquad
\frac d{ds}(bW^2)=bg'=\frac{\mathcal B}{W},
\qquad
bWg'=\mathcal B.
$$

The [pure plume](../../../turbulent-plume.md#pure-plume) solution is

$$
b(z)=\alpha(z_o-z),
\qquad
W(z)=\left(\frac{\mathcal B}{\alpha}\right)^{1/3},
\qquad
g'(z)=
\left(\frac{\mathcal B}{\alpha}\right)^{2/3}
\frac1{z_o-z}.
$$

Imposing $b(z_V)=H'/2$ fixes

$$
\boxed{z_o=z_V+\frac{H'}{2\alpha}}.
$$

The constant speed is a special feature of a pure top-hat line plume; its width and [volumetric flow rate](../../../fluid-mechanics.md#volumetric-flow-rate) grow linearly with downward distance while entrainment dilutes its density anomaly like $(z_o-z)^{-1}$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let

$$
g'_H=\frac{g(\rho_1-\rho_H)}{\rho_0},
\qquad
g'_L=\frac{g(\rho_1-\rho_L)}{\rho_0}.
$$

The global steady heat, or [buoyancy flux](../../../turbulent-plume.md#buoyancy-flux), balance equates the floor-source input to the buoyancy carried out by the one-way upper-layer exhaust:

$$
B=Q_Vg'_H.
$$

The corresponding upper-to-lower density jump is fixed by the warm plume crossing the interface,

$$
B=Q_B(h)(g'_H-g'_L).
$$

The first balance also shows that the descending cold plume has buoyancy-flux magnitude per unit wall length

$$
\mathcal B=\frac{Q_Vg'_H}{L}=\frac BL.
$$

At a steady interface, the upward axisymmetric-plume volume flux equals the total downward wall-plume volume flux. Using parts (c) and (d),

$$
C_PB^{1/3}h^{5/3}
=L\alpha(z_o-h)
\left(\frac{B}{\alpha L}\right)^{1/3}.
$$

After cancellation of $B^{1/3}$, the required implicit geometric relation is

$$
\boxed{
C_Ph^{5/3}
=\alpha^{2/3}L^{2/3}(z_o-h),
\qquad
z_o=z_V+\frac{H'}{2\alpha}
}.
$$

Thus the ideal steady interface fraction is independent of the source strength: increasing $B$ multiplies both opposing plume volume fluxes by $B^{1/3}$. The floor area $A$ and room height $H$ affect the transient filling time and admissibility of the assumed ordering, but not this steady integral balance, provided $0<h<z_V$ and the plumes remain separated.

Set

$$
K_V=\frac{C_d}{3}LH'^{3/2}.
$$

Combining the [single-opening exchange flow](../../../fluid-mechanics.md#single-opening-exchange-flow) relation $Q_V=K_V\sqrt{g'_H}$ with $B=Q_Vg'_H$ gives

$$
\boxed{
Q_V=(K_V^2B)^{1/3}
=\left(\frac{C_d^2L^2H'^3B}{9}\right)^{1/3}
}.
$$

It also gives $g'_H=(B/K_V)^{2/3}$, after which the second density balance determines $g'_L$.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Assume the two identical openings and their wall plumes behave symmetrically and do not interact before reaching the interface. If $Q_V^{(1)}$ is the one-way rate through either vent, the global buoyancy balance is

$$
B=2Q_V^{(1)}g'_H.
$$

Each wall plume therefore has buoyancy flux per unit span $\mathcal B=B/(2L)$. The steady volume balance now includes two descending plumes:

$$
C_PB^{1/3}h^{5/3}
=2L\alpha(z_o-h)
\left(\frac{B}{2\alpha L}\right)^{1/3}.
$$

Hence the interface height is determined implicitly by

$$
\boxed{
C_Ph^{5/3}
=2^{2/3}\alpha^{2/3}L^{2/3}(z_o-h),
\qquad
z_o=z_V+\frac{H'}{2\alpha}
}.
$$

For completeness, if each opening retains the same [single-opening exchange flow](../../../fluid-mechanics.md#single-opening-exchange-flow) coefficient $K_V$, then

$$
Q_V^{(1)}=\left(\frac{K_V^2B}{2}\right)^{1/3},
\qquad
Q_{V,\mathrm{total}}=2Q_V^{(1)}
=2^{2/3}(K_V^2B)^{1/3}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
