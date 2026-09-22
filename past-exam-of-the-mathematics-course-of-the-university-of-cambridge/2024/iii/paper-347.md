# Paper 347

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_347.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_347.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 347](paper-347.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let the mean particle mass be $\mu m_p$. For a monatomic [ideal gas](../../../thermodynamics.md#ideal-gas) with $\gamma=5/3$,

$$
P=\frac{\rho_0k_BT}{\mu m_p},
\qquad
c_s^2=\frac{\gamma k_BT}{\mu m_p}.
$$

A uniform sphere of mass $M=(4\pi/3)\rho_0r^3$ has Newtonian gravitational energy

$$
W=-\frac{3GM^2}{5r}.
$$

At the virial threshold, the pressure term $3\int P\,dV=3Mk_BT/(\mu m_p)$ balances $|W|$. Therefore

$$
M=\frac{5k_BT}{G\mu m_p}r.
$$

Eliminating $r$ gives the [Jeans mass](../../../stellar-astrophysics.md#jeans-mass)

$$
\boxed{
M_J=\left(\frac{5k_BT}{G\mu m_p}\right)^{3/2}
\left(\frac{3}{4\pi\rho_0}\right)^{1/2}
}.
$$

The numerical coefficient depends on the convention used to identify a finite cloud with a Jeans mode. For example, assigning the mass inside a sphere of radius half the standard [Jeans instability](../../../linear-cosmological-density-perturbation.md#jeans-instability) wavelength gives

$$
M_J=\frac{\pi^{5/2}}6
\frac{c_s^3}{G^{3/2}\rho_0^{1/2}}.
$$

Both conventions have the physically invariant scaling

$$
M_J\propto T^{3/2}\rho_0^{-1/2}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For [adiabatic](../../../thermodynamics.md#adiabatic-process) collapse, $T\rho^{1-\gamma}$ is constant. With $\gamma=5/3$,

$$
T\propto\rho^{2/3},
\qquad
M_J\propto T^{3/2}\rho^{-1/2}\propto\rho^{1/2}.
$$

The rising [Jeans mass](../../../stellar-astrophysics.md#jeans-mass) produces [adiabatic suppression of fragmentation](../../../stellar-astrophysics.md#adiabatic-suppression-of-fragmentation): smaller subregions become more pressure-supported as density increases.

For [isothermal fragmentation](../../../stellar-astrophysics.md#isothermal-fragmentation), $T$ stays approximately constant, and

$$
M_J\propto\rho^{-1/2}.
$$

The instability scale then falls during collapse, allowing hierarchical fragmentation until cooling fails, opacity rises, or another source of support intervenes.

Primordial metal-free gas cools inefficiently, principally through molecular hydrogen, and remains relatively hot. It therefore has a larger [Jeans mass](../../../stellar-astrophysics.md#jeans-mass) and tends toward a top-heavy [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) of massive [Population III stars](../../../stellar-astrophysics.md#population-iii-star). Metal lines and dust let enriched gas remain cool to higher density, so [Population II stars](../../../stellar-astrophysics.md#population-ii-star) extend to much lower birth masses.

These alternatives map directly onto [black-hole seed](../../../astrophysics.md#black-hole-seed) channels. Massive Population III remnants produce light [Population III remnant black-hole seeds](../../../astrophysics.md#population-iii-remnant-black-hole-seed). If cooling and fragmentation are strongly suppressed while a primordial halo supplies rapid inflow, near-monolithic collapse can produce a heavy [direct-collapse black-hole seed](../../../astrophysics.md#direct-collapse-black-hole-seed). Intermediate cooling and fragmentation in a dense cluster can instead permit a [runaway stellar-collision black-hole seed](../../../astrophysics.md#runaway-stellar-collision-black-hole-seed). The Jeans argument selects plausible mass scales; angular momentum, feedback, chemistry, and accretion determine which channel actually operates.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The axisymmetric razor-thin [astrophysical disk](../../../astrophysics.md#astrophysical-disk) equations are

$$
\partial_t\Sigma+\frac1R\partial_R(R\Sigma u_R)=0,
$$



$$
\partial_tu_R+u_R\partial_Ru_R-\frac{u_\phi^2}{R}
=-\frac1\Sigma\partial_Rp-\partial_R\Phi,
$$



$$
\partial_tu_\phi+u_R\partial_Ru_\phi+\frac{u_Ru_\phi}{R}=0,
\qquad
\nabla^2\Phi=4\pi G\Sigma(R,t)\delta(z).
$$

For the stationary background, mass and azimuthal momentum conservation are automatic, while radial force balance and the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) give

$$
R\Omega^2=\frac1{\Sigma_0}\frac{dp_0}{dR}+\frac{d\Phi_0}{dR},
\qquad
\nabla^2\Phi_0=4\pi G\Sigma_0\delta(z).
$$

Here $dp_0/dR=0$ under the stated constant-pressure assumption.

Retaining first-order perturbations and using $c_s^2=dp/d\Sigma$ gives

$$
\partial_t\Sigma'+\frac{\Sigma_0}{R}\partial_R(Ru_R')=0,
$$



$$
\partial_tu_R'-2\Omega u_\phi'
=-\frac{c_s^2}{\Sigma_0}\partial_R\Sigma'-\partial_R\Phi',
$$



$$
\partial_tu_\phi'+\frac{\kappa^2}{2\Omega}u_R'=0,
\qquad
\nabla^2\Phi'=4\pi G\Sigma'\delta(z),
$$

where

$$
\kappa^2=4\Omega^2+2R\Omega\frac{d\Omega}{dR}
$$

is the squared [radial epicyclic frequency](../../../astrophysics.md#radial-epicyclic-frequency). In the local $|k|R\gg1$ limit, a [Fourier mode](../../../fourier-analysis.md#fourier-mode) $e^{i(kR-\omega t)}$ obeys

$$
-i\omega\Sigma'+ik\Sigma_0u_R'=0,
$$



$$
-i\omega u_R'-2\Omega u_\phi'
=-ik\left(c_s^2\frac{\Sigma'}{\Sigma_0}+\Phi'\right),
$$



$$
-i\omega u_\phi'+\frac{\kappa^2}{2\Omega}u_R'=0,
\qquad
\Phi'=-\frac{2\pi G\Sigma'}{|k|}.
$$

Eliminating $\Sigma'$, $u_\phi'$, and $\Phi'$ yields the local [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{
\omega^2=\kappa^2-2\pi G\Sigma_0|k|+c_s^2k^2
}.
$$

For a [Keplerian orbit](../../../classical-mechanics.md#kepler-orbit), $\Omega\propto R^{-3/2}$, so

$$
\kappa^2=4\Omega^2-3\Omega^2=\Omega^2.
$$

Instability requires $\omega^2<0$, equivalently a mode with positive imaginary frequency. Treating the right-hand side as a quadratic in $x=|k|$, its two roots are

$$
x_\pm=\frac{\pi G\Sigma_0}{c_s^2}
\left(1\pm\sqrt{1-Q^2}\right),
\qquad
Q=\frac{c_s\Omega}{\pi G\Sigma_0}.
$$

Real distinct roots, and hence an unstable interval $x_-<|k|<x_+$, exist exactly when the [Toomre stability criterion](../../../gravitational-instability-of-an-astrophysical-disk.md#toomre-s-stability-criterion) has $Q<1$.

With $h=c_s/\Omega$,

$$
\frac{\omega^2}{\Omega^2}
=1-\frac{2h|k|}{Q}+h^2k^2.
$$

The constant positive term is epicyclic restoration by rotation and stabilizes long wavelengths. The negative term is the razor-thin disk's self-gravity and drives collapse. The positive $k^2$ term is gas-pressure restoration and stabilizes short wavelengths. Gravitational instability can therefore survive only on an intermediate band of scales.

## 2

↑ **Parent:** [Paper 347](paper-347.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Steady [mass conservation](../../../continuum-mechanics.md#mass-conservation) with inward-positive [accretion rate](../../../astrophysics.md#accretion-rate) gives

$$
\dot m=-2\pi R\Sigma u_R=\text{constant}.
$$

Write the specific angular momentum as $l=R^2\Omega$. Multiplying the azimuthal equation by $2\pi R$ and using the mass equation shows that the sum of advected and viscous angular-momentum flux is constant:

$$
\dot m,l+2\pi\nu\Sigma R^3\frac{d\Omega}{dR}
=\dot m,l_{\rm in}.
$$

The right-hand side implements the [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition). For a [Keplerian accretion disk](../../../astrophysics.md#keplerian-accretion-disk), $l\propto R^{1/2}$ and $R^3d\Omega/dR=-(3/2)l$. Therefore

$$
\boxed{
\nu\Sigma
=\frac{\dot m}{3\pi}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]
},
$$

and

$$
\boxed{
u_R
=-\frac{3\nu}{2R}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]^{-1}
}.
$$

Far outside the inner edge, $\Sigma\simeq\dot m/(3\pi\nu)$ and $u_R\simeq-3\nu/(2R)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Shakura--Sunyaev thin disk](../../../astrophysics.md#shakura-sunyaev-thin-disk) model replaces poorly resolved turbulent angular-momentum transport by a stress proportional to pressure,

$$
|T_{R\phi}|=\alpha p,
\qquad 0<\alpha\lesssim1.
$$

Equivalently, an eddy viscosity has $\nu\sim v_{\rm eddy}\ell_{\rm eddy}$. Turbulent motions much faster than the [sound speed](../../../compressible-flow.md#speed-of-sound) $c_s$ would shock, while eddies much larger than the [disk scale height](../../../astrophysics.md#disk-scale-height) $H$ would not fit within the disk. Writing $v_{\rm eddy}\ell_{\rm eddy}=\alpha c_sH$ therefore gives the [alpha disk](../../../astrophysics.md#alpha-disk) prescription

$$
\boxed{
\nu=\alpha c_sH
\simeq\alpha\frac{c_s^2}{\Omega_K}
},
$$

where vertical hydrostatic balance gives $H\simeq c_s/\Omega_K$. The parameter $\alpha$ summarizes the correlation and efficiency of turbulent or magnetic stresses; it is not a molecular viscosity.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $\varepsilon=H/R\ll1$. Vertical hydrostatic balance gives $c_s\sim H\Omega_K$, whereas leading radial force balance gives $u_\phi\sim R\Omega_K$. Hence

$$
\frac{u_\phi}{c_s}\sim\frac RH=\varepsilon^{-1}\gg1.
$$

Using part (a) and $\nu=\alpha c_sH$ far from the inner edge,

$$
\frac{|u_R|}{c_s}
\simeq\frac32\frac{\nu}{Rc_s}
=\frac32\alpha\frac HR
=O(\alpha\varepsilon)\ll1.
$$

Thus [subsonic radial drift in a thin disk](../../../astrophysics.md#subsonic-radial-drift-in-a-thin-disk) coexists with highly supersonic orbital motion. Gas follows nearly circular, pressure-coherent orbits and loses angular momentum only slowly, completing of order $(\alpha\varepsilon^2)^{-1}$ revolutions during its viscous inflow.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

At fixed radiative efficiency, the [Eddington ratio](../../../astrophysics.md#eddington-ratio) implies $\dot m\propto f_{\rm Edd}M$. Far outside the [innermost stable circular orbit](../../../astrophysics.md#innermost-stable-circular-orbit), part (a) gives $\Sigma\propto\dot m/\nu$. The supplied viscosity law therefore gives, in physical radius,

$$
\Sigma
\propto
f_{\rm Edd}^{7/10}
\left(\frac\alpha{0.1}\right)^{-4/5}
M^{19/20}R^{-3/4}.
$$

The disk mass follows by radial integration:

$$
M_d(R)=2\pi\int^{R}\Sigma(R')R'\,dR'
\propto
f_{\rm Edd}^{7/10}
\left(\frac\alpha{0.1}\right)^{-4/5}
M^{19/20}R^{5/4}.
$$

Since the [Schwarzschild radius](../../../general-relativity.md#schwarzschild-radius) satisfies $R_S\propto M$, replacing $R$ by $(R/R_S)R_S$ contributes another factor $M^{5/4}$. Thus

$$
\boxed{
M_d(R)=C_1
f_{\rm Edd}^{7/10}
\left(\frac\alpha{0.1}\right)^{-4/5}
\left(\frac{M}{10^6M_\odot}\right)^{11/5}
\left(\frac R{R_S}\right)^{5/4}
},
$$

so

$$
(k_1,k_2,k_3,k_4)=
\left(\frac7{10},-\frac45,\frac{11}5,\frac54\right).
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [alpha disk](../../../astrophysics.md#alpha-disk) relation and Keplerian angular frequency give

$$
c_s\sim\left(\frac{\nu\Omega}{\alpha}\right)^{1/2}
\propto
R^{-3/8}f_{\rm Edd}^{3/20}
\left(\frac\alpha{0.1}\right)^{-1/10}M^{11/40}.
$$

Combining this with $\Omega\propto M^{1/2}R^{-3/2}$ and the surface-density scaling from part (d), the [Toomre stability criterion](../../../gravitational-instability-of-an-astrophysical-disk.md#toomre-s-stability-criterion) becomes

$$
Q(R)\propto
R^{-9/8}f_{\rm Edd}^{-11/20}
\left(\frac\alpha{0.1}\right)^{7/10}M^{-7/40}.
$$

It decreases strictly with radius, so it crosses unity at a unique [self-gravitating radius of an accretion disk](../../../gravitational-instability-of-an-astrophysical-disk.md#self-gravitating-radius-of-an-accretion-disk). Expressing radius in units of $R_S\propto M$ gives

$$
Q\propto
\left(\frac R{R_S}\right)^{-9/8}
f_{\rm Edd}^{-11/20}
\left(\frac\alpha{0.1}\right)^{7/10}M^{-13/10}.
$$

Solving $Q(R_{\rm sg})=1$ therefore yields

$$
\boxed{
\frac{R_{\rm sg}}{R_S}
=C_2f_{\rm Edd}^{-22/45}
\left(\frac\alpha{0.1}\right)^{28/45}
\left(\frac{M}{10^6M_\odot}\right)^{-52/45}
},
$$

and

$$
(k_5,k_6,k_7)=
\left(-\frac{22}{45},\frac{28}{45},-\frac{52}{45}\right).
$$

Let $x_{\rm ISCO}=R_{\rm ISCO}/R_S$. Requiring a non-self-gravitating annulus outside the [innermost stable circular orbit](../../../astrophysics.md#innermost-stable-circular-orbit) gives $R_{\rm sg}>R_{\rm ISCO}$, and equality defines

$$
M_{\rm crit}
=10^6M_\odot
\left(\frac{C_2}{x_{\rm ISCO}}\right)^{45/52}
f_{\rm Edd}^{-11/26}
\left(\frac\alpha{0.1}\right)^{7/13}.
$$

For a nonspinning hole, $x_{\rm ISCO}=3$, and with $C_2\simeq10^5$, $\alpha\simeq0.1$, and $f_{\rm Edd}\simeq1$, this is approximately $8\times10^9M_\odot$, conventionally quoted as order $10^{10}M_\odot$. Above this mass the disk would become self-gravitating essentially as soon as stable circular orbits begin, so the assumed smooth [Shakura--Sunyaev thin disk](../../../astrophysics.md#shakura-sunyaev-thin-disk) cannot provide a broad luminous accretion region.

The corresponding [Eddington luminosity](../../../stellar-structure.md#eddington-luminosity) is of order $10^{48}\,\mathrm{erg\,s^{-1}}$, comparable to the upper envelope of quasar luminosities. This supports self-gravity as one contributor to the observed luminous-mass ceiling. It is not an absolute upper bound on black-hole mass: mergers, radiatively inefficient growth, nonstandard gas supply, spin-dependent inner radii, and fragmented or episodic accretion can all build a more massive hole without maintaining this particular steady thin disk.

## 3

↑ **Parent:** [Paper 347](paper-347.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [radiatively inefficient accretion flow](../../../astrophysics.md#radiatively-inefficient-accretion-flow) radiates only a small fraction of the energy released before the gas crosses the inner boundary. At low [Eddington ratio](../../../astrophysics.md#eddington-ratio), an optically thin flow has such low density that radiative cooling, commonly proportional to density squared, is slower than inflow; the gas remains hot and forms an [advection-dominated accretion flow](../../../astrophysics.md#advection-dominated-accretion-flow). At high Eddington ratio, an optically thick [slim accretion disk](../../../astrophysics.md#slim-accretion-disk) can instead undergo [photon trapping in an accretion flow](../../../astrophysics.md#photon-trapping-in-an-accretion-flow): diffusion is slower than inward motion, so radiation is advected into the hole.

The local [accretion-flow advection balance](../../../astrophysics.md#accretion-flow-advection-balance)

$$
q_{\rm adv}=q^+-q^-
$$

has three sign classes. If $q_{\rm adv}=0$, local heating equals local radiative cooling and the flow is a radiatively efficient thin disk. If $q_{\rm adv}>0$, heating exceeds cooling and inward advection removes the excess; low-rate ADAFs and high-rate slim disks are the two principal realizations. If $q_{\rm adv}<0$, radiation exceeds local dissipation and compressive advection supplies heat, producing a [luminous hot accretion flow](../../../astrophysics.md#luminous-hot-accretion-flow) branch.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Denote the four terms by

$$
I=(\mathbf v_p\mathbin\cdot\nabla)\mathbf v_p,
\qquad
P=-\frac1\rho\nabla p,
\qquad
G=-\nabla\Phi,
\qquad
C=\Omega^2\mathbf R,
$$

so the radial or poloidal momentum equation is $I=P+G+C$.

i) In a thin [Keplerian accretion disk](../../../astrophysics.md#keplerian-accretion-disk), radial inertia and pressure are higher-order in $H/R$, leaving $G+C\simeq0$.

ii) In a nearly static stellar atmosphere, $I=C=0$ and [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) balance gives $P+G=0$.

iii) In pressureless gravitational collapse, rotation and pressure are negligible, so $I=G$; this is free fall.

iv) A [slim accretion disk](../../../astrophysics.md#slim-accretion-disk) retains radial inertia and radial pressure together with gravity and centrifugal support, so all four terms generally survive: $I=P+G+C$.

v) A stationary geometrically thick disk or torus has negligible poloidal inertia but order-one pressure support, giving $P+G+C=0$.

vi) Nonrotating [Bondi accretion](../../../astrophysics.md#bondi-accretion) has $C=0$ and $I=P+G$. In a highly supersonic Bondi--Hoyle limit the pressure term is also negligible, reducing this to ballistic $I=G$.

vii) A sub-Keplerian [advection-dominated accretion flow](../../../astrophysics.md#advection-dominated-accretion-flow) has significant pressure support and radial inflow as well as rotation, so again $I=P+G+C$, with $C$ smaller than the Keplerian value and the remaining inward gravity balanced by $P$ and $I$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The stated [standard thin-disk dissipation flux](../../../astrophysics.md#standard-thin-disk-dissipation-flux) is summed over the two faces, so the total luminosity is

$$
\begin{aligned}
L_{\rm thin}
&=\int_{R_{\rm ISCO}}^\infty 2\pi R F_{\rm diss}(R)\,dR\\
&=\frac{3GM\dot m}{2}
\int_{R_{\rm ISCO}}^\infty
\left(R^{-2}-R_{\rm ISCO}^{1/2}R^{-5/2}\right)dR\\
&=\boxed{\frac{GM\dot m}{2R_{\rm ISCO}}}.
\end{aligned}
$$

This equals the Newtonian [standard thin-disk luminosity](../../../astrophysics.md#standard-thin-disk-luminosity) and the orbital binding energy delivered per unit time at the inner edge. It is half the magnitude $GM\dot m/R_{\rm ISCO}$ of the potential-energy decrease because the other half appears as orbital kinetic energy. In the zero-torque model that remaining mechanical energy passes through the inner edge rather than being dissipated at larger radii. The associated Newtonian [radiative efficiency of black-hole accretion](../../../astrophysics.md#radiative-efficiency-of-black-hole-accretion) is $GM/(2R_{\rm ISCO}c^2)$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Steady [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $\dot m=-2\pi R\Sigma u_R$. With specific angular momentum $l=R^2\Omega$, multiply the angular-momentum equation by $2\pi$ and define the signed [viscous torque in an accretion disk](../../../astrophysics.md#viscous-torque-in-an-accretion-disk)

$$
\mathcal G(R)=2\pi\nu\Sigma R^3\frac{d\Omega}{dR}.
$$

Then

$$
\frac{d\mathcal G}{dR}
=-\dot m\frac{dl}{dR}.
$$

Integration from $R_1$ to $R_2$ gives

$$
\boxed{
\mathcal G_2-\mathcal G_1=-\dot m(l_2-l_1)
}.
$$

The viscous power generated in an annulus is $2\pi R F_{\rm diss}\,dR=\mathcal G\,d\Omega$. Taking the inner torque to vanish and writing $l_{\rm in}=l(R_{\rm in})$ gives $\mathcal G=-\dot m(l-l_{\rm in})$, hence

$$
L_{\rm gen}
=-\dot m\int_{R_{\rm in}}^{R_{\rm out}}
(l-l_{\rm in})\frac{d\Omega}{dR}\,dR.
$$

[Integration by parts](../../../calculus.md#integration-by-parts) yields

$$
L_{\rm gen}
=\dot m\left[
\int_{l_{\rm in}}^{l_{\rm out}}\Omega\,dl
-\Omega_{\rm out}(l_{\rm out}-l_{\rm in})
\right].
$$

For steady circular force balance, $de=\Omega\,dl$; equivalently, the stated equality of gravitational- and rotational-potential differences makes the integral $e_{\rm out}-e_{\rm in}$. Therefore

$$
\boxed{
L_{\rm gen}(R_{\rm in},R_{\rm out})
\simeq\dot m
\left[e_{\rm out}-e_{\rm in}
-\Omega_{\rm out}(l_{\rm out}-l_{\rm in})\right]
}.
$$

When $R_{\rm out}\gg R_{\rm in}$, the outer energy and boundary term vanish. For an approximately Keplerian inner orbit, $e_{\rm in}=-R_{\rm in}^2\Omega_{\rm in}^2/2$, so

$$
L_{\rm gen}\simeq
\frac12\dot mR_{\rm in}^2\Omega_{\rm in}^2.
$$

Comparison with part (c) gives

$$
\boxed{
\frac{L_{\rm gen}}{L_{\rm thin}}
\simeq
\left(\frac{\Omega_{\rm in}}{\Omega_{K,\rm in}}\right)^2
}.
$$

A Keplerian inner flow generates the standard thin-disk power. A pressure-supported sub-Keplerian slim disk generates less through shear, and its emergent luminosity can be smaller still because [photon trapping in an accretion flow](../../../astrophysics.md#photon-trapping-in-an-accretion-flow) carries part of that generated energy through the inner edge.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
