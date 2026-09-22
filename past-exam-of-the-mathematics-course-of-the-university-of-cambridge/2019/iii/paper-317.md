# Paper 317

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_317.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_317.pdf)

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
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [a](#3/ii/a)
      - [Solution](#3/ii/a/solution)
    - [b](#3/ii/b)
      - [Solution](#3/ii/b/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 317](paper-317.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Assume [stellar homology](../../../stellar-structure.md#stellar-homology): fixed dimensionless profiles, uniform fixed composition, negligible [radiation pressure](../../../thermodynamics.md#radiation-pressure), [ideal gas](../../../thermodynamics.md#ideal-gas) support, and radiative transport throughout the model. [Mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $\rho_c\propto M/R^3$. The [hydrostatic pressure support equation](../../../stellar-structure.md#hydrostatic-pressure-support-equation) gives $P_c\propto GM^2/R^4$; combining with $P\propto\rho T$ gives $T_c\propto M/R$.

Integrating specific [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) energy generation over mass gives

$$
L_{\rm nuc}\propto M\rho_cT_c^4\propto M^6R^{-7}.
$$

For [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star), $T_c/R\propto\kappa_c\rho_cL/(R^2T_c^3)$, hence $L_{\rm rad}\propto RT_c^4/(\kappa_c\rho_c)$. With the [Kramers' opacity law](../../../stellar-structure.md#kramers-opacity-law) $\kappa_c\propto\rho_cT_c^{-7/2}$,

$$
L_{\rm rad}\propto\frac{RT_c^{15/2}}{\rho_c^2}\propto M^{11/2}R^{-1/2}.
$$

Equating generated and transported luminosity gives $M^{1/2}\propto R^{13/2}$, so the [radiative homology with proton-proton burning and Kramers opacity](../../../stellar-structure.md#radiative-homology-with-proton-proton-burning-and-kramers-opacity) relation is

$$
\boxed{M\propto R^{13}.}
$$

The proportionality constants are fixed only within the adopted homologous family, not for arbitrary evolving stars.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Using $R\propto M^{1/13}$ in the [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star) scaling from part (i),

$$
L\propto M^{11/2}R^{-1/2}\propto M^{11/2-1/26}.
$$

Therefore the [mass-luminosity relation](../../../stellar-structure.md#mass-luminosity-relation) is

$$
\boxed{L\propto M^{71/13}.}
$$

The nuclear scaling independently gives $L\propto M^6R^{-7}\propto M^{6-7/13}=M^{71/13}$, consistent with [radiative homology with proton-proton burning and Kramers opacity](../../../stellar-structure.md#radiative-homology-with-proton-proton-burning-and-kramers-opacity).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law) defines the [effective temperature](../../../stellar-structure.md#effective-temperature) through $L=4\pi R^2\sigma_{\rm SB}T_{\rm eff}^4$. The [stellar homology](../../../stellar-structure.md#stellar-homology) relations give $R\propto M^{1/13}\propto L^{1/71}$, so

$$
T_{\rm eff}^4\propto L/R^2\propto L^{69/71}.
$$

Thus

$$
\boxed{T_{\rm eff}\propto L^q,\qquad q=\frac{69}{284}.}
$$

In a logarithmic [Hertzsprung-Russell diagram](../../../stellar-astrophysics.md#hertzsprung-russell-diagram), with $\log L$ plotted vertically against $\log T_{\rm eff}$,

$$
\boxed{\frac{d\log L}{d\log T_{\rm eff}}=\frac{284}{69}\simeq4.12.}
$$

The usual horizontal axis increases in [effective temperature](../../../stellar-structure.md#effective-temperature) toward the left, so the hotter, more luminous end lies toward the upper left. The quoted algebraic slope uses increasing $\log T_{\rm eff}$ as the coordinate.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Retain the same [stellar homology](../../../stellar-structure.md#stellar-homology) and gas-pressure assumptions, but use the specified [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) law $\epsilon\propto\rho T^{16}$ and constant [electron-scattering opacity](../../../stellar-structure.md#electron-scattering-opacity). The nuclear luminosity now scales as

$$
L_{\rm nuc}\propto M\rho_cT_c^{16}\propto M^{18}R^{-19}.
$$

The [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star) scaling becomes

$$
L_{\rm rad}\propto RT_c^4/\rho_c\propto M^3.
$$

Equating the two yields $R^{19}\propto M^{15}$. Therefore [radiative homology with CNO burning and electron scattering](../../../stellar-structure.md#radiative-homology-with-cno-burning-and-electron-scattering) gives

$$
\boxed{M\propto R^{19/15},\qquad L\propto M^3.}
$$

Since $R\propto L^{5/19}$, the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law) gives

$$
\boxed{T_{\rm eff}\propto L^{9/76},\qquad
\frac{d\log L}{d\log T_{\rm eff}}=\frac{76}{9}\simeq8.44.}
$$

This is a model comparison using the exponent 16 prescribed here. Actual massive stars may have appreciable [radiation pressure](../../../thermodynamics.md#radiation-pressure) and convective cores, which violate the assumptions of this purely radiative gas-pressure family.

## 2

↑ **Parent:** [Paper 317](paper-317.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Consider an element displaced upward by $\xi$ in [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium). Assume it quickly reaches the ambient [pressure](../../../thermodynamics.md#pressure), but moves adiabatically and retains its composition. Put $\nabla=d\log T/d\log P$, $\nabla_\mu=d\log\mu/d\log P$, and let $\nabla_{\rm ad}$ be the [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient). The [equation of state](../../../thermodynamics.md#equation-of-state) has differential

$$
d\log\rho=\alpha_P\,d\log P-\delta\,d\log T+\phi\,d\log\mu,
$$

where $\delta=-(\partial\log\rho/\partial\log T)_{P,\mu}$ and $\phi=(\partial\log\rho/\partial\log\mu)_{P,T}$.

At the new [pressure](../../../thermodynamics.md#pressure), the parcel-to-environment density difference is

$$
\frac{\rho_{\rm parcel}-\rho_{\rm env}}\rho
=[\delta(\nabla-\nabla_{\rm ad})-\phi\nabla_\mu]\,\Delta\log P.
$$

With positive pressure scale height $H_P=-(d\log P/dr)^{-1}$, $\Delta\log P=-\xi/H_P$. The [buoyancy](../../../fluid-mechanics.md#buoyancy) acceleration is therefore $\ddot\xi=-N^2\xi$, with [stellar buoyancy frequency](../../../gravity-wave.md#stellar-buoyancy-frequency)

$$
N^2=\frac g{H_P}[\delta(\nabla_{\rm ad}-\nabla)+\phi\nabla_\mu].
$$

A negative $N^2$ amplifies the displacement. For a radiative background, $\nabla=\nabla_{\rm rad}$, so the [Ledoux criterion](../../../stellar-structure.md#ledoux-criterion) for instability is

$$
\boxed{\nabla_{\rm rad}>\nabla_{\rm ad}+\frac\phi\delta\nabla_\mu.}
$$

For uniform composition, $\nabla_\mu=0$, giving the [Schwarzschild criterion](../../../stellar-structure.md#schwarzschild-criterion)

$$
\boxed{\nabla_{\rm rad}>\nabla_{\rm ad}.}
$$

Equality is marginal stability. A [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight) increasing inward has $\nabla_\mu>0$ and supplies a stabilizing composition term when $\phi,\delta>0$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [Eddington closure approximation](../../../astrophysics.md#eddington-closure-approximation) with the standard surface boundary condition gives the [grey atmosphere](../../../astrophysics.md#grey-atmosphere) profile

$$
T^4=\frac34T_{\rm eff}^4\left(\tau+\frac23\right).
$$

Together with the specified pressure law, logarithmic differentiation gives

$$
\frac{d\log T}{d\tau}=\frac1{4(\tau+2/3)},\qquad
\frac{d\log P}{d\tau}=\frac{3}{4(1+3\tau/2)\log(1+3\tau/2)}.
$$

Consequently the [radiative temperature gradient](../../../exoplanet.md#radiative-temperature-gradient) is

$$
\nabla_{\rm rad}=\frac{d\log T}{d\log P}=\frac12\log(1+3\tau/2).
$$

For a monatomic [perfect gas](../../../thermodynamics.md#ideal-gas), $\gamma=5/3$ and the [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient) is $(\gamma-1)/\gamma=2/5$. Uniform composition makes the [Schwarzschild criterion](../../../stellar-structure.md#schwarzschild-criterion) applicable. The first marginal layer therefore satisfies $\log(1+3\tau_c/2)=4/5$, giving the [convection onset in a logarithmic-pressure grey atmosphere](../../../stellar-structure.md#convection-onset-in-a-logarithmic-pressure-grey-atmosphere)

$$
\boxed{\tau_c=\frac23(e^{4/5}-1)\simeq0.817.}
$$

The assumed profile becomes convectively unstable for $\tau>\tau_c$; further inward, a self-consistent model must account for convective transport.

## 3

↑ **Parent:** [Paper 317](paper-317.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Assume zero temperature, complete ionization, constant composition, noninteracting electrons, negligible ion thermal pressure, and Newtonian stellar gravity. Ions supply almost all the mass, while [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) supplies support. By the [Pauli exclusion principle](../../../quantum-mechanics.md#pauli-exclusion-principle), the two electron spin states fill a momentum sphere up to [Fermi momentum](../../../statistical-physics.md#fermi-momentum) $p_F$. Counting states gives

$$
n_e=\frac{2}{(2\pi\hbar)^3}\frac{4\pi p_F^3}{3}
=\frac{p_F^3}{3\pi^2\hbar^3},\qquad
\rho=\mu_em_un_e,
$$

where $\mu_e$ is [mean molecular weight per electron](../../../thermodynamics.md#mean-molecular-weight-per-electron). The momentum flux of this isotropic [Fermi gas](../../../statistical-physics.md#fermi-gas) is

$$
P=\frac{2}{3(2\pi\hbar)^3}\int_{p\le p_F}p\,v(p)\,d^3p
=\frac1{3\pi^2\hbar^3}\int_0^{p_F}\frac{p^4c^2}{\sqrt{m_e^2c^4+p^2c^2}}\,dp.
$$

Writing $x=p_F/(m_ec)$ and performing the integral gives the [equation of state of a cold electron gas](../../../statistical-physics.md#equation-of-state-of-a-cold-electron-gas)

$$
\boxed{P=\frac{m_e^4c^5}{24\pi^2\hbar^3}
\left[x(2x^2-3)\sqrt{1+x^2}+3\operatorname{arsinh}x\right],\qquad
x=\frac{\hbar}{m_ec}\left(\frac{3\pi^2\rho}{\mu_em_u}\right)^{1/3}.}
$$

In the nonrelativistic limit $p_F\ll m_ec$, $v(p)\simeq p/m_e$, so

$$
\boxed{P=K_{\rm NR}\rho^{5/3},\qquad
K_{\rm NR}=\frac{\hbar^2(3\pi^2)^{2/3}}{5m_e(\mu_em_u)^{5/3}}.}
$$

In the ultrarelativistic limit $p_F\gg m_ec$, $v(p)\simeq c$, so

$$
\boxed{P=K_{\rm R}\rho^{4/3},\qquad
K_{\rm R}=\frac{\hbar c(3\pi^2)^{1/3}}{4(\mu_em_u)^{4/3}}.}
$$

These are [polytropic equations of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state) with indices $3/2$ and $3$, respectively. The relativistic softening underlies the [Chandrasekhar mass](../../../stellar-astrophysics.md#chandrasekhar-limit) limit; Coulomb corrections, thermal effects, rotation, and general relativity are excluded from this idealized derivation.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/a">a</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/ii/a)

For the [nonrelativistic white dwarf](../../../stellar-astrophysics.md#nonrelativistic-white-dwarf), combine the [hydrostatic pressure support equation](../../../stellar-structure.md#hydrostatic-pressure-support-equation) and [enclosed mass](../../../stellar-structure.md#enclosed-mass) equation:

$$
\frac{dP}{dr}=-\frac{Gm\rho}{r^2},\qquad
\frac{dm}{dr}=4\pi r^2\rho.
$$

Eliminating $m$ yields

$$
\boxed{\frac1{r^2}\frac d{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G\rho,\qquad P=K_{\rm NR}\rho^{5/3}.}
$$

Introduce the [Lane-Emden variables for a stellar polytrope](../../../stellar-structure.md#lane-emden-variables-for-a-stellar-polytrope),

$$
\rho=\rho_c\theta^{3/2},\qquad r=a\xi,\qquad
 a^2=\frac{5K_{\rm NR}}{8\pi G}\rho_c^{-1/3}.
$$

The resulting [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation) is

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}(\xi^2\theta')=-\theta^{3/2},\qquad
\theta(0)=1,\quad\theta'(0)=0.}
$$

The [white dwarf](../../../stellar-astrophysics.md#white-dwarf) surface is at the first zero $\xi_1$ of $\theta$, with $R=a\xi_1$.

<h4 id="3/ii/b">b</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/ii/b)

Let $\omega=-\xi_1^2\theta'(\xi_1)$ be the [Lane-Emden surface mass constant](../../../stellar-structure.md#lane-emden-surface-mass-constant). The [Lane-Emden mass formula](../../../stellar-structure.md#lane-emden-mass-formula) gives

$$
R=a\xi_1,\qquad M=4\pi a^3\rho_c\omega,
\qquad a^2=\frac{5K_{\rm NR}}{8\pi G}\rho_c^{-1/3}.
$$

Thus $R\propto\rho_c^{-1/6}$ while $M\propto\rho_c^{1/2}$ at fixed composition. Eliminating central [mass density](../../../fluid-mechanics.md#density) gives the [polytropic mass-radius relation](../../../stellar-structure.md#polytropic-mass-radius-relation)

$$
\boxed{M\propto R^{-3},\qquad s=-3.}
$$

More explicitly,

$$
R=\xi_1(4\pi\omega)^{1/3}\frac{5K_{\rm NR}}{8\pi G}M^{-1/3}.
$$

Increasing the mass of a [nonrelativistic white dwarf](../../../stellar-astrophysics.md#nonrelativistic-white-dwarf) decreases its radius. This scaling ceases to apply when relativistic [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) becomes important.

## 4

↑ **Parent:** [Paper 317](paper-317.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For $P=K\rho^2$, [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives $2K\nabla\rho=-\nabla\Phi$. The [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) therefore gives the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation)

$$
\nabla^2\rho+k^2\rho=0,\qquad k^2=\frac{2\pi G}{K}.
$$

For spherical symmetry, the regular [polytrope of index one](../../../stellar-structure.md#polytrope-of-index-one) solution is

$$
\boxed{\rho(r)=\rho_c\frac{\sin(kr)}{kr}.}
$$

The singular $\cos(kr)/r$ solution is excluded by finite central [mass density](../../../fluid-mechanics.md#density). Taking the first zero as the stellar surface yields

$$
\boxed{R=\frac\pi k=\sqrt{\frac{\pi K}{2G}}.}
$$

The mass integral is

$$
M=4\pi\int_0^R\rho r^2\,dr
=\frac{4\pi\rho_c}{k^3}\int_0^\pi u\sin u\,du
=\frac{4\pi^2\rho_c}{k^3}.
$$

Dividing by the volume $4\pi R^3/3$ gives

$$
\boxed{\frac{\bar\rho}{\rho_c}=\frac3{\pi^2}.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The same [polytrope of index one](../../../stellar-structure.md#polytrope-of-index-one) interior equation is $\nabla^2\rho+(2\pi G/K)\rho=0$. A positive separated solution with zero density on all six cube faces is the [cubic polytropic interior](../../../stellar-structure.md#cubic-polytropic-interior)

$$
\boxed{\rho(x,y,z)=\rho_c\sin\frac{\pi x}{L}\sin\frac{\pi y}{L}\sin\frac{\pi z}{L}.}
$$

Its [Laplacian](../../../calculus.md#laplacian) is $-3\pi^2\rho/L^2$, so the required side length is

$$
\boxed{L=\sqrt{\frac{3\pi K}{2G}}.}
$$

With $\Phi=C-2K\rho$ and $P=K\rho^2$, it satisfies the interior [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) and [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity). Integrating each sine factor yields

$$
M=\rho_c\left(\frac{2L}{\pi}\right)^3,
\qquad
\boxed{\frac{\bar\rho}{\rho_c}=\frac8{\pi^3}.}
$$

This formal interior solution is not an isolated physical cubic star. The [cubic polytrope fails isolated gravitational matching](../../../stellar-structure.md#cubic-polytrope-fails-isolated-gravitational-matching): at a vertex, the product of sines has $\nabla\rho=0$, so the interior potential predicts zero gravitational acceleration. At the vertex $(0,0,0)$, however, the field generated by its own positive mass is

$$
\mathbf g(0)=G\int_{[0,L]^3}\rho(\mathbf r')\frac{\mathbf r'}{|\mathbf r'|^3}\,d^3r',
$$

and each component is strictly positive. There can be no continuous matching to the isolated external field without additional forces or mass sources. Thus solving the interior density equation and imposing zero face values is insufficient. Fluid stars also have no rigid structure to maintain sharp cubic faces, and observed stellar shapes are approximately spherical or rotationally flattened rather than cubic.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
