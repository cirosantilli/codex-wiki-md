# Paper 71

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper71.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper71.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use $\mathcal R$ for the [stellar gas constant](../../../thermodynamics.md#stellar-gas-constant), reserving $R$ for the stellar [radius](../../../topology.md#radius). The [specific internal energy](../../../thermodynamics.md#specific-internal-energy) of a [monatomic gas](../../../thermodynamics.md#monatomic-gas) obeying the [ideal gas](../../../thermodynamics.md#ideal-gas) law is $e=P/[(\gamma-1)\rho]=3P/(2\rho)$. At fixed enclosed [mass](../../../classical-mechanics.md#mass), the [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics) gives the heat available to the outgoing [luminosity](../../../astrophysics.md#luminosity) as $\epsilon=-\partial_te-P\partial_t(1/\rho)$ when there is no [stellar nuclear fusion](../../../stellar-astrophysics.md#stellar-nuclear-fusion) heating. Therefore

$$
\boxed{\epsilon=-\frac3{2\rho}\left(\frac{\partial P}{\partial t}\right)_m
+\frac{5P}{2\rho^2}\left(\frac{\partial\rho}{\partial t}\right)_m.}
$$

The second coefficient includes both the [mass density](../../../fluid-mechanics.md#density) dependence of $e$ and [pressure](../../../thermodynamics.md#pressure) work. This is [gravitational energy generation in a homologously contracting ideal-gas star](../../../stellar-astrophysics.md#gravitational-energy-generation-in-a-homologously-contracting-ideal-gas-star).

Write the characteristic scales as

$$
\rho_0=\frac M{4\pi R^3},\qquad P_0=\frac{GM^2}{4\pi R^4},\qquad T_0=\frac{\mu GM}{\mathcal R R}.
$$

Then $\rho=\rho_0b$, $P=P_0p$, $T=T_0p/b$, $m=Mq$ and $L_r=Ll$. Since $d/dr=R^{-1}d/dx$, direct substitution in the [stellar hydrostatic equation](../../../stellar-structure.md#hydrostatic-pressure-support-equation) and [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives

$$
\boxed{\frac{dp}{dx}=-\frac{bq}{x^2},\qquad\frac{dq}{dx}=x^2b.}
$$

For [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star), dividing the [temperature](../../../thermodynamics.md#temperature) equation by $T_0/R$ gives

$$
\frac d{dx}\left(\frac pb\right)
=-\frac{3\kappa_0\rho_0L}{16\pi acRT_0^4}\frac{bl}{x^2(p/b)^3}
=-D\frac{b^4l}{x^2p^3},\qquad
\boxed{D=\frac{3\kappa_0\mathcal R^4L}{64\pi^2ac\mu^4G^4M^3}.}
$$

In particular the fourth power here is of $\mathcal R$, not of the [radius](../../../topology.md#radius).

Because $q(x)$ is fixed and $M$ is constant, a fixed [mass](../../../classical-mechanics.md#mass) label has fixed $x$. Thus [stellar homology](../../../stellar-structure.md#stellar-homology) gives $\partial_t\rho=-3\rho\dot R/R$ and $\partial_tP=-4P\dot R/R$. The heating rate reduces to $\epsilon=-3P\dot R/(2\rho R)$, positive during [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism). Substitution in $dL_r/dr=4\pi r^2\rho\epsilon$ now yields

$$
\frac{dl}{dx}=-\frac{6\pi R^2\dot R}{L}x^2P
=Ex^2p,\qquad
\boxed{E=-\frac{3GM^2\dot R}{2R^2L}>0.}
$$

The [dimensionless](../../../physics.md#dimensionless-quantity) profiles fix $D$ and $E$. In a common [stellar homology](../../../stellar-structure.md#stellar-homology) family with fixed [stellar composition](../../../stellar-astrophysics.md#stellar-chemical-abundance) and [opacity](../../../stellar-structure.md#opacity) normalization, the expression for $D$ implies

$$
\boxed{L=\frac{64\pi^2ac\mu^4G^4D}{3\kappa_0\mathcal R^4}M^3\propto M^3.}
$$

It is independent of [radius](../../../topology.md#radius) and constant in time for a particular fixed-mass star. The formula for $E$ gives $\dot R=-2ELR^2/(3GM^2)$, which integrates to

$$
\frac1{R(t)}=\frac1{R_0}+\frac{2ELt}{3GM^2}.
$$

When the initial-radius term is negligible,

$$
\boxed{\frac{RLt}{GM^2}=\frac3{2E}.}
$$

This is the [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism) time law in the prescribed [stellar homology](../../../stellar-structure.md#stellar-homology) model. Infinite initial [radius](../../../topology.md#radius) is a limiting idealization; a finite initial [radius](../../../topology.md#radius) retains the first term.

At [main sequence](../../../stellar-astrophysics.md#main-sequence) arrival, [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) heating with fixed [stellar composition](../../../stellar-astrophysics.md#stellar-chemical-abundance) has [luminosity](../../../astrophysics.md#luminosity)

$$
L_{\rm nuc}=\epsilon_0M\rho_0T_0^{16}\int_0^1b(q)\left(\frac{p(q)}{b(q)}\right)^{16}dq
\propto\frac{M^{18}}{R^{19}}.
$$

The [integral](../../../calculus.md#integral) is [dimensionless](../../../physics.md#dimensionless-quantity) and fixed within the [stellar homology](../../../stellar-structure.md#stellar-homology) family. The constant-[opacity](../../../stellar-structure.md#opacity) radiative scaling still gives $L\propto M^3$. Equating the [stellar nuclear fusion](../../../stellar-astrophysics.md#stellar-nuclear-fusion) and transported [luminosities](../../../astrophysics.md#luminosity) gives

$$
\boxed{R_{\rm MS}\propto M^{15/19}.}
$$

Finally the [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism) law evaluated at $R_{\rm MS}$ gives $t_{\rm MS}\propto M^2/(LR_{\rm MS})\propto M^{-34/19}$. In a coeval [star cluster](../../../galaxy.md#star-cluster), the [mass](../../../classical-mechanics.md#mass) just arriving at the [main sequence](../../../stellar-astrophysics.md#main-sequence) consequently satisfies

$$
\boxed{M_{\rm arrival}\propto t^{-19/34}.}
$$

These results comprise [constant-opacity homologous contraction to CNO ignition](../../../stellar-structure.md#constant-opacity-homologous-contraction-to-cno-ignition); their [mass](../../../classical-mechanics.md#mass) exponents compare fixed-composition models with common [dimensionless](../../../physics.md#dimensionless-quantity) profiles.

## 2

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Consider a small outward displacement $\delta r$ of a fluid element. It adjusts to the ambient [pressure](../../../thermodynamics.md#pressure) while retaining its [specific entropy](../../../thermodynamics.md#specific-entropy) and [stellar composition](../../../stellar-astrophysics.md#stellar-chemical-abundance), so an [adiabatic process](../../../thermodynamics.md#adiabatic-process) gives $d\log\rho_{\rm parcel}=d\log P/\gamma$. Its excess [mass density](../../../fluid-mechanics.md#density) over the new surroundings is, to first order,

$$
\rho_{\rm parcel}-\rho_{\rm ambient}
=\left[\frac\rho{\gamma P}\frac{dP}{dr}-\frac{d\rho}{dr}\right]\delta r.
$$

Restoring [buoyancy](../../../fluid-mechanics.md#buoyancy) requires this bracket to be positive. With $\gamma=5/3$, the [Schwarzschild criterion](../../../stellar-structure.md#schwarzschild-criterion) is therefore

$$
\boxed{\frac{dP}{dr}>\frac{5P}{3\rho}\frac{d\rho}{dr}.}
$$

Equality is neutral stability. For uniform [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight), the [ideal gas](../../../thermodynamics.md#ideal-gas) law gives $d\log\rho=d\log P-d\log T$. Since [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) [pressure](../../../thermodynamics.md#pressure) decreases outward, the inequality is equivalent to $\nabla=d\log T/d\log P<\nabla_{\rm ad}=2/5$. Dividing the [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star) and [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) [stellar structure equations](../../../stellar-structure.md#stellar-structure-equations) gives

$$
\nabla_{\rm rad}=\frac{3\kappa L_rP}{16\pi acGmT^4},\qquad
\boxed{\frac{3\kappa L_rP}{16\pi acGmT^4}<\frac25.}
$$

This is the [stellar radiative temperature gradient](../../../stellar-structure.md#stellar-radiative-temperature-gradient) test for [stellar convective stability](../../../stellar-structure.md#stellar-convective-stability).

In the thin upper [stellar atmosphere](../../../stellar-astrophysics.md#stellar-atmosphere) take $m\simeq M$, $L_r\simeq L$ and use [gas pressure](../../../thermodynamics.md#gas-pressure) dominance. The prescribed [opacity](../../../stellar-structure.md#opacity) becomes $\kappa=\kappa_0\mu PT^{12}/\mathcal R$. Dividing the two structure equations then yields

$$
P\frac{dP}{dT}=\frac{16\pi acGM\mathcal R}{3\kappa_0L\mu}T^{-9}.
$$

At zero [optical depth](../../../astrophysics.md#optical-depth), the atmospheric boundary has $T_s^4=T_e^4/2$ and negligible [gas pressure](../../../thermodynamics.md#gas-pressure). Integrating from that boundary, with $T_s^{-8}=4T_e^{-8}$, gives

$$
\boxed{P^2=\frac{4\pi acGM\mathcal R}{3\kappa_0L\mu T_e^8}
\left(4-\frac{T_e^8}{T^8}\right).}
$$

To locate the onset, put $y=T_e^8/T^8$. [Logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) gives $d\log P/d\log T=4y/(4-y)$, hence

$$
\nabla_{\rm rad}=\frac{4-y}{4y}=\frac{T^8}{T_e^8}-\frac14.
$$

This starts at zero at the outer boundary and increases inward. It first reaches $2/5$ at

$$
\boxed{T_b=(13/20)^{1/8}T_e.}
$$

The corresponding [optical depth](../../../astrophysics.md#optical-depth) is $\tau_b=\tfrac43(\sqrt{13/20}-\tfrac12)>0$, so the onset lies inside the [stellar atmosphere](../../../stellar-astrophysics.md#stellar-atmosphere). This is [grey-atmosphere convection onset with thirteenth-power opacity](../../../stellar-structure.md#grey-atmosphere-convection-onset-with-thirteenth-power-opacity).

Let the interior of the [fully convective star](../../../stellar-structure.md#fully-convective-star) have $P=K_TT^{5/2}$, with $K_T$ spatially constant. At its boundary $T_b/T_e$ is fixed, so the atmospheric [pressure](../../../thermodynamics.md#pressure) formula gives

$$
K_T^2=\frac{P_b^2}{T_b^5}\propto\frac M{LT_e^{13}}.
$$

The [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law), $L=4\pi R^2\sigma T_e^4$ with $\sigma=ac/4$, consequently implies

$$
K_T^2\propto MR^{13/2}L^{-17/4}.
$$

The [ideal gas](../../../thermodynamics.md#ideal-gas) equation transforms the interior relation into

$$
P=K_\rho\rho^{5/3},\qquad K_\rho=(\mathcal R/\mu)^{5/3}K_T^{-2/3}.
$$

For completeness, the mass-radius scaling follows by taking $\rho=\rho_c\theta^{3/2}$ and $r=\alpha\xi$ with $\alpha^2=5K_\rho\rho_c^{-1/3}/(8\pi G)$. [Hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) and [mass conservation](../../../continuum-mechanics.md#mass-conservation) reduce to the [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation) $(\xi^2\theta')'=-\xi^2\theta^{3/2}$, with $\theta(0)=1$, $\theta'(0)=0$. Its fixed [dimensionless](../../../physics.md#dimensionless-quantity) profile gives $R\propto\alpha$ and $M\propto\alpha^3\rho_c$. Eliminating $\rho_c$ gives $R\propto K_\rho G^{-1}M^{-1/3}$, or $K_\rho\propto GM^{1/3}R$. Thus $K_T^2\propto M^{-1}R^{-3}$ at fixed [stellar composition](../../../stellar-astrophysics.md#stellar-chemical-abundance). Equating this with the atmospheric expression gives $L^{17/4}\propto M^2R^{19/2}$, and hence

$$
\boxed{L\propto M^{8/17}R^{38/17}.}
$$

This [Hayashi relation with thirteenth-power opacity](../../../stellar-astrophysics.md#hayashi-relation-with-thirteenth-power-opacity) concerns the interior of a [fully convective star](../../../stellar-structure.md#fully-convective-star) beneath a thin [stellar atmosphere](../../../stellar-astrophysics.md#stellar-atmosphere). The coefficient $K_T$ may vary between stars; spatially constant [specific entropy](../../../thermodynamics.md#specific-entropy) does not mean equal [specific entropy](../../../thermodynamics.md#specific-entropy) across the whole sequence.

## 3

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A fully ionized [helium](../../../chemistry.md#helium) nucleus supplies two [Electrons](../../../physics.md#electron) for approximately $4m_p$ of [mass](../../../classical-mechanics.md#mass), so $n_e=\rho/(2m_p)$. Filling all [Electron](../../../physics.md#electron) [momentum](../../../classical-mechanics.md#momentum) states up to the [Fermi momentum](../../../statistical-physics.md#fermi-momentum) gives

$$
n_e=\int_0^{p_0}\frac{8\pi p^2}{h^3}dp=\frac{8\pi p_0^3}{3h^3},\qquad
p_0=\left(\frac{3h^3\rho}{16\pi m_p}\right)^{1/3}.
$$

For a nonrelativistic [Electron](../../../physics.md#electron), the speed is $p/m_e$. The three mean squared Cartesian components of [momentum](../../../classical-mechanics.md#momentum) are equal by rotational symmetry and sum to $p^2$, so each is $p^2/3$. This is the [isotropic tensor integral](../../../geometry-and-topology.md#isotropic-tensor-integral). Thus the [momentum flux](../../../physics.md#momentum-flux), or [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure), is

$$
P_e=\frac13\int_0^{p_0}\frac{p^2}{m_e}\frac{8\pi p^2}{h^3}dp
=\frac{8\pi p_0^5}{15m_eh^3}.
$$

Substituting the expression for $p_0$ and simplifying the powers of two gives

$$
\boxed{P_e=K\rho^{5/3},\qquad
K=\left(\frac3{2\pi}\right)^{2/3}\frac{h^2}{40m_em_p^{5/3}}.}
$$

Here $h$ is the [Planck constant](../../../quantum-mechanics.md#planck-constant). This is the pure-helium specialization of [nonrelativistic electron-degeneracy pressure in a hydrogen-helium mixture](../../../statistical-physics.md#nonrelativistic-electron-degeneracy-pressure-in-a-hydrogen-helium-mixture).

For a cold [helium white dwarf](../../../stellar-astrophysics.md#helium-white-dwarf), neglect ion thermal [pressure](../../../thermodynamics.md#pressure) and use this [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) as the support against [Newtonian gravity](../../../classical-mechanics.md#gravitational-acceleration). Combining [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) with [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives

$$
\frac1{r^2}\frac d{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G\rho.
$$

Set $\rho=\rho_c\theta^{3/2}$ and $r=\alpha\xi$, where $\alpha^2=5K\rho_c^{-1/3}/(8\pi G)$. Direct substitution gives the [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation)

$$
\frac1{\xi^2}\frac d{d\xi}(\xi^2\theta')=-\theta^{3/2},\qquad\theta(0)=1,\quad\theta'(0)=0.
$$

Its [dimensionless](../../../physics.md#dimensionless-quantity) solution is independent of $\rho_c$. Let $\xi_1$ be its first zero and $\omega_1=-\xi_1^2\theta'(\xi_1)=\int_0^{\xi_1}\xi^2\theta^{3/2}d\xi$. Integrating [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives

$$
R=\alpha\xi_1,\qquad M=4\pi\alpha^3\rho_c\omega_1.
$$

Eliminating $\rho_c$ yields the [polytropic mass-radius relation](../../../stellar-structure.md#polytropic-mass-radius-relation)

$$
\boxed{R=AM^{-1/3},\qquad
A=\frac{5K}{8\pi G}\,\xi_1(4\pi\omega_1)^{1/3}.}
$$

Thus a more massive [nonrelativistic white dwarf](../../../stellar-astrophysics.md#nonrelativistic-white-dwarf) is smaller at fixed [stellar composition](../../../stellar-astrophysics.md#stellar-chemical-abundance). The assumptions require $p_0\ll m_ec$ and $k_BT\ll p_0^2/(2m_e)$ in the region providing most support; the law is not extended into the relativistic or thermally supported regimes.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Outside the emitting layer, take $m\simeq M_c$, $L_r\simeq L$ and $P=\mathcal R\rho T/\mu$. The [Kramers' opacity law](../../../stellar-structure.md#kramers-opacity-law) then reads $\kappa=(\kappa_0\mu/\mathcal R)PT^{-9/2}$. Division of the [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star) equation by the [stellar hydrostatic equation](../../../stellar-structure.md#hydrostatic-pressure-support-equation) gives

$$
\frac{dP}{dT}=\frac{16\pi acGM_c}{3\kappa L}T^3,
\qquad
P\frac{dP}{dT}=\frac{16\pi acGM_c\mathcal R}{3\kappa_0L\mu}T^{15/2}.
$$

With the outer [pressure](../../../thermodynamics.md#pressure) [constant of integration](../../../calculus.md#constant-of-integration) neglected, [integration](../../../calculus.md#integral) yields

$$
\boxed{P=CT^{17/4},\qquad
C=\left(\frac{64\pi acGM_c\mathcal R}{51\kappa_0L\mu}\right)^{1/2},\qquad
\rho=\frac{\mu C}{\mathcal R}T^{13/4}.}
$$

Substitute this into [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium):

$$
\frac{17}4CT^{13/4}\frac{dT}{dr}
=-\frac{GM_c}{r^2}\frac{\mu C}{\mathcal R}T^{13/4},
\qquad
\frac{dT}{dr}=-\frac{4\mu GM_c}{17\mathcal Rr^2}.
$$

Define $B=4\mu GM_c/(17\mathcal R)$. The general [antiderivative](../../../calculus.md#antiderivative) is $T=B/r+T_0$. The [Kramers radiative-zero envelope around a stellar core](../../../stellar-structure.md#kramers-radiative-zero-envelope-around-a-stellar-core) sets $T_0=0$, giving

$$
\boxed{T=\frac{4\mu GM_c}{17\mathcal Rr}.}
$$

This is exact for the idealized boundary $T\to0$ as $r\to\infty$. With a finite outer [radius](../../../topology.md#radius) $R_s$ and [temperature](../../../thermodynamics.md#temperature) $T_s$, instead $T=T_s+B(1/r-1/R_s)$; the displayed profile is the deep-envelope approximation when $R_s\gg R_c$ and $|T_s-B/R_s|\ll B/R_c$. Small outer [pressure](../../../thermodynamics.md#pressure) alone does not eliminate this [temperature](../../../thermodynamics.md#temperature) [constant of integration](../../../calculus.md#constant-of-integration).

The specific [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning) rate becomes

$$
\epsilon=\epsilon_0\rho T^{67/4}
=\frac{\epsilon_0\mu C}{\mathcal R}T^{20}\propto r^{-20}.
$$

Consequently

$$
\boxed{\frac{\epsilon(1.05R_c)}{\epsilon(R_c)}=1.05^{-20}
=e^{-20\log(1.05)}\simeq0.377\simeq e^{-1}.}
$$

Its local radial e-folding length is $R_c/20$, so burning is concentrated within a small fraction of the [stellar core](../../../stellar-structure.md#stellar-core) [radius](../../../topology.md#radius). The volume heating is even steeper: $\rho\epsilon\propto C^2T^{93/4}$. Using the exterior envelope profile to estimate the thin shell's [luminosity](../../../astrophysics.md#luminosity) gives

$$
L\simeq4\pi\epsilon_0\left(\frac{\mu C}{\mathcal R}\right)^2B^{93/4}
\int_{R_c}^{\infty}r^{-85/4}dr
=\frac{16\pi\epsilon_0}{81}\left(\frac{\mu C}{\mathcal R}\right)^2B^{93/4}R_c^{-81/4}.
$$

A finite but very extended upper limit changes the factor by $1-(R_c/R_s)^{81/4}$. The large exponent makes this correction small and further verifies the [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning) thin-shell approximation. Since $C^2\propto M_c/L$ and $B\propto M_c$, the [integral](../../../calculus.md#integral) implies $L^2\propto M_c^{97/4}R_c^{-81/4}$. Hence

$$
\boxed{L\propto M_c^{97/8}R_c^{-81/8},\qquad
L\propto M_c^{97/8}\ \text{along the fixed-}R_c\text{ sequence}.}
$$

This is the [fixed-radius-core shell-burning luminosity relation](../../../stellar-astrophysics.md#fixed-radius-core-shell-burning-luminosity-relation). The proportionality coefficient is a thin-shell estimate: [luminosity](../../../astrophysics.md#luminosity) rises from its value beneath the shell to $L$ through the emitting layer, so treating it as constant there uses the exterior profile rather than resolving the burning region. The scaling holds while its [dimensionless](../../../physics.md#dimensionless-quantity) shell structure and [stellar composition](../../../stellar-astrophysics.md#stellar-chemical-abundance) remain fixed.

For consistency, $M_c/R_c$ must provide a hot [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning) shell while the [stellar core](../../../stellar-structure.md#stellar-core) remains inert to [core helium burning](../../../stellar-astrophysics.md#core-helium-burning); the [radiative envelope](../../../stellar-structure.md#radiative-envelope) [mass](../../../classical-mechanics.md#mass) must be much less than $M_c$, and $R_c$ must be well inside an extended [radiative envelope](../../../stellar-structure.md#radiative-envelope). At the shell base the gas must remain a [nondegenerate gas](../../../thermodynamics.md#nondegenerate-gas) and dominated by [gas pressure](../../../thermodynamics.md#gas-pressure), in particular $aT_b^4/3\ll CT_b^{17/4}$ with $T_b=B/R_c$. The assumed [stellar core](../../../stellar-structure.md#stellar-core) sequence must genuinely have nearly fixed $R_c$ over the [mass](../../../classical-mechanics.md#mass) interval considered. A cold [helium](../../../chemistry.md#helium) [stellar core](../../../stellar-structure.md#stellar-core) supported by a nonrelativistic [degenerate electron gas](../../../statistical-physics.md#degenerate-electron-gas) instead has the mass-radius law from part (a), so substituting that law would describe a different model and change the [luminosity](../../../astrophysics.md#luminosity) exponent.

## 4

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $M=M_1+M_2$. The [centre of mass](../../../classical-mechanics.md#center-of-mass) condition gives $a_1=aM_2/M$, $a_2=aM_1/M$. For [circular motion](../../../classical-mechanics.md#circular-motion) the component [angular momenta](../../../classical-mechanics.md#angular-momentum) are $J_i=M_ia_i^2\Omega$, so

$$
J=(M_1a_1^2+M_2a_2^2)\Omega
=\frac{M_1M_2}{M}a^2\Omega.
$$

Using [Kepler's third law](../../../physics.md#kepler-s-third-law), $a^3\Omega^2=GM$, and $\Omega=2\pi/P_{\rm orb}$ gives

$$
\boxed{J=\frac{M_1M_2}{M}a^2\Omega
=\frac{G^{2/3}P_{\rm orb}^{1/3}M_1M_2}{(2\pi)^{1/3}M^{1/3}}.}
$$

This is the [circular-binary orbital angular momentum](../../../stellar-astrophysics.md#circular-binary-orbital-angular-momentum). [Mass](../../../classical-mechanics.md#mass) received by the companion redistributes [angular momentum](../../../classical-mechanics.md#angular-momentum) within the [binary star](../../../stellar-astrophysics.md#binary-star); only the escaping [stellar wind](../../../stellar-astrophysics.md#stellar-wind) removes it under the prescribed model.

The [stellar wind](../../../stellar-astrophysics.md#stellar-wind) from the [donor star](../../../stellar-astrophysics.md#donor-star) has [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum)

$$
j_w=\frac{J_1}{M_1}=a_1^2\Omega,\qquad\frac{j_w}{J}=\frac{M_2}{M_1M}.
$$

Here $\dot M_1<0$, $\dot M_2=-f\dot M_1$ and $\dot M=(1-f)\dot M_1$. Thus [donor-wind angular-momentum loss](../../../stellar-astrophysics.md#donor-wind-angular-momentum-loss) gives

$$
\frac{\dot J}{J}=(1-f)\dot M_1\frac{M_2}{M_1M}.
$$

Taking the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) of the period expression for $J$ gives

$$
\frac{\dot P_{\rm orb}}{P_{\rm orb}}
=3\frac{\dot J}{J}-3\frac{\dot M_1}{M_1}-3\frac{\dot M_2}{M_2}+\frac{\dot M}{M}.
$$

Use $M_2/(M_1M)=1/M_1-1/M$ to simplify this to

$$
\frac{\dot P_{\rm orb}}{P_{\rm orb}}
=-3f\frac{\dot M_1}{M_1}-3\frac{\dot M_2}{M_2}-2\frac{\dot M}{M}.
$$

For constant $f$, [integration](../../../calculus.md#integral) therefore gives

$$
\boxed{P_{\rm orb}\propto M_1^{-3f}M_2^{-3}(M_1+M_2)^{-2}.}
$$

This is the [donor-wind period invariant with fixed retention fraction](../../../stellar-astrophysics.md#donor-wind-period-invariant-with-fixed-retention-fraction). If $f$ changes during the evolution, the differential equation remains valid but the integrated invariant is instead $P_{\rm orb}M_2^3M^2\exp(3\int f\,d\log M_1)=\mathrm{constant}$. The fixed-power expression cannot be used with a time-dependent exponent without this modification.

For the [Roche lobe](../../../stellar-astrophysics.md#roche-lobe), write $q=M_1/M_2$. The equivalent separation expression $J=M_1M_2\sqrt{Ga/M}$ gives

$$
\frac{\dot a}{a}=2\frac{\dot J}{J}-2\frac{\dot M_1}{M_1}-2\frac{\dot M_2}{M_2}+\frac{\dot M}{M}
=\frac{\dot M_1}{M_1}\left[2f(q-1)-(1-f)\frac q{1+q}\right].
$$

Taking the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) of $R_L=0.46a(M_1/M)^{1/3}$ then adds $\dot M_1/(3M_1)-\dot M/(3M)$, yielding

$$
\boxed{\frac{\dot R_L}{R_L}=\frac{\dot M_1}{M_1}\left[
f\left(2q+\frac{4q}{3(1+q)}-2\right)+\frac13-\frac{4q}{3(1+q)}\right].}
$$

This [donor-wind Roche-lobe response](../../../stellar-astrophysics.md#donor-wind-roche-lobe-response) uses only the instantaneous value of $f$ and thus still holds if it varies.

Define $A(q)=2q+4q/[3(1+q)]-2$ and $B(q)=1/3-4q/[3(1+q)]$. The [Roche-lobe radius response exponent](../../../stellar-astrophysics.md#roche-lobe-radius-response-exponent) is $\zeta_L=B+Af$, whereas the [donor star](../../../stellar-astrophysics.md#donor-star)'s [stellar radius response exponent](../../../stellar-astrophysics.md#stellar-radius-response-exponent) is $\zeta_*=-n$. Keeping $R_1=R_L$ requires the two [logarithmic derivatives](../../../analytic-number-theory.md#logarithmic-derivative) of [radius](../../../topology.md#radius) to agree, so

$$
\boxed{f\left(2q+\frac{4q}{3(1+q)}-2\right)=\frac{4q}{3(1+q)}-n-\frac13.}
$$

For $A\ne0$, this determines

$$
\boxed{f_{\rm req}=\frac{4q/[3(1+q)]-n-1/3}{2q+4q/[3(1+q)]-2}.}
$$

A physical mixture of [Roche-lobe overflow](../../../stellar-astrophysics.md#roche-lobe-overflow) and [stellar wind](../../../stellar-astrophysics.md#stellar-wind) from the [donor star](../../../stellar-astrophysics.md#donor-star) needs $0<f<1$. Equivalently, $-n$ must lie strictly between the pure-wind response $B$ and the conservative response $B+A=2q-5/3$. The values $f=0$ and $1$ are valid limiting prescriptions, respectively pure [stellar wind](../../../stellar-astrophysics.md#stellar-wind) and [conservative mass transfer](../../../stellar-astrophysics.md#conservative-binary-mass-transfer), rather than mixtures. If $f_{\rm req}$ lies outside $[0,1]$, no allowed division of the lost [mass](../../../classical-mechanics.md#mass) can maintain contact under this [radius](../../../topology.md#radius) law and angular-momentum-loss prescription. This is [feasibility of donor-wind binary contact](../../../stellar-astrophysics.md#feasibility-of-donor-wind-binary-contact).

The likely direction away from contact follows without assigning a nonphysical fraction. For any actual $f$, let $\Delta=\log(R_1/R_L)$. Then

$$
\dot\Delta=(-n-B-Af)\frac{\dot M_1}{M_1}
=A(f_{\rm req}-f)\frac{\dot M_1}{M_1}.
$$

Since $\dot M_1<0$, a positive value of $A(f_{\rm req}-f)$ makes the [donor star](../../../stellar-astrophysics.md#donor-star) move inside its lobe and detach; a negative value increases overfill and promotes stronger transfer. Thus if $A>0$, $f_{\rm req}<0$ gives increasing overfill and $f_{\rm req}>1$ gives detachment; if $A<0$, these outcomes are reversed. A runaway or a new equilibrium would require the [donor star](../../../stellar-astrophysics.md#donor-star)'s response or the angular-momentum-loss model to change, possibly with additional driving. The contact calculation alone does not prove a particular nonlinear endpoint.

There is also a genuine exceptional denominator: $A=0$ at $q=(\sqrt{10}-1)/3$. At this ratio both limiting lobe responses coincide. Contact is possible only if $-n=B$, namely $n=(\sqrt{10}-2)/(\sqrt{10}+2)$; then every $f$ gives the same instantaneous [radius](../../../topology.md#radius) response. Otherwise no fraction works, and the sign of $(-n-B)\dot M_1/M_1$ determines detachment or increasing overfill.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
