# Paper 63

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper63.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper63.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Efficient [convection](../../../fluid-mechanics.md#convection) keeps the interior at nearly uniform [specific entropy](../../../thermodynamics.md#specific-entropy). For the fully ionized [monatomic gas](../../../thermodynamics.md#monatomic-gas), the [heat capacity ratio](../../../thermodynamics.md#heat-capacity-ratio) is $5/3$, so the [adiabatic process](../../../thermodynamics.md#adiabatic-process) gives $P=K_\rho\rho^{5/3}$, with $K_\rho$ spatially constant. The [ideal gas](../../../thermodynamics.md#ideal-gas) relation $P=\mathcal R\rho T/\mu$ then implies

$$
\boxed{P=KT^{5/2}},\qquad K=\left(\frac{\mathcal R}{\mu}\right)^{5/2}K_\rho^{-3/2}.
$$

The constant is spatial, not temporal: loss of [specific entropy](../../../thermodynamics.md#specific-entropy) during contraction changes it. This is a [stellar polytrope](../../../stellar-structure.md#stellar-polytrope) with [polytropic index](../../../stellar-structure.md#polytropic-index) $n=3/2$. We neglect [radiation pressure](../../../thermodynamics.md#radiation-pressure) and take the thin [photosphere](../../../stellar-structure.md#photosphere) as an atmospheric matching layer rather than a significant fraction of the stellar mass.

For a fixed dimensionless profile of the [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation), the [stellar homology](../../../stellar-structure.md#stellar-homology) relations have the form

$$
\rho_c=C_\rho\frac{M}{R^3},\qquad P_c=C_P\frac{GM^2}{R^4},\qquad T_c=\frac{C_P}{C_\rho}\frac{\mu GM}{\mathcal R R},
$$

where $C_\rho,C_P$ are positive dimensionless structure constants. More explicitly, write $\rho(r)=\rho_cf(x)$ and $m(r)=Mh(x)$ with $x=r/R$ and fixed dimensionless profiles. Mass conservation gives $M=4\pi\rho_cR^3\int_0^1f(x)x^2\,dx$. Integrating the [hydrostatic pressure support equation](../../../stellar-structure.md#hydrostatic-pressure-support-equation), with negligible surface pressure on the interior scale, gives $P_c=(GM\rho_c/R)\int_0^1h(x)f(x)x^{-2}\,dx$. Both integrals are fixed positive numbers, proving the two central scalings. Substituting these relations into $K=P_c/T_c^{5/2}$ gives

$$
\boxed{K=K_0\mu^{-5/2}M^{-1/2}R^{-3/2}},\qquad K_0=C_\rho^{5/2}C_P^{-3/2}\mathcal R^{5/2}G^{-3/2}.
$$

Thus the same [polytropic index](../../../stellar-structure.md#polytropic-index) fixes $K_0$ throughout this homologous sequence, while the dimensional [stellar polytrope](../../../stellar-structure.md#stellar-polytrope) constant changes.

At the [photosphere](../../../stellar-structure.md#photosphere), whose [optical depth](../../../astrophysics.md#optical-depth) is $2/3$, identify the temperature with the [effective temperature](../../../stellar-structure.md#effective-temperature) $T_e$. The [ideal gas](../../../thermodynamics.md#ideal-gas) relation and the interior adiabat give $\rho_{\rm ph}=\mu K T_e^{3/2}/\mathcal R$. With the prescribed [opacity](../../../stellar-structure.md#opacity) and [stellar surface boundary condition](../../../stellar-structure.md#stellar-surface-boundary-condition),

$$
\kappa P=\frac{\kappa_0\mu}{\mathcal R}K^2T_e^8=\frac{2GM}{3R^2}.
$$

Eliminating $K$ therefore proves

$$
\boxed{T_e^8=\frac{2G\mathcal R}{3\kappa_0K_0^2}\mu^4M^2R}.
$$

Using the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law), with $\sigma=ac/4$, gives the [luminosity](../../../astrophysics.md#luminosity)

$$
L=4\pi R^2\sigma T_e^4=\pi ac\left(\frac{2G\mathcal R}{3\kappa_0}\right)^{1/2}K_0^{-1}\mu^2MR^{5/2}.
$$

The [gravitational energy of a stellar polytrope](../../../stellar-structure.md#gravitational-energy-of-a-stellar-polytrope) is $\Omega=-6GM^2/(7R)$ for $n=3/2$. The [stellar virial theorem](../../../stellar-structure.md#stellar-virial-theorem) for a [monatomic gas](../../../thermodynamics.md#monatomic-gas) gives $2U+\Omega=0$, and hence the total energy is $E=U+\Omega=-3GM^2/(7R)$. With no appreciable [stellar nuclear fusion](../../../stellar-astrophysics.md#stellar-nuclear-fusion) or [accretion](../../../astrophysics.md#accretion), energy conservation gives

$$
L=-\frac{dE}{dt}=-\frac{3GM^2}{7R^2}\dot R.
$$

Combining the two expressions for $L$ yields

$$
\dot R=-\frac{7\pi ac}{3}\left(\frac{2\mathcal R}{3\kappa_0G}\right)^{1/2}K_0^{-1}\mu^2M^{-1}R^{9/2}.
$$

Multiplication by $-7R^{-9/2}/2$ and integration proves the [contraction law with density-linear fourth-power stellar opacity](../../../stellar-astrophysics.md#contraction-law-with-density-linear-fourth-power-stellar-opacity):

$$
\boxed{R^{-7/2}-R_0^{-7/2}=\frac{49\pi ac}{6}\left(\frac{2\mathcal R}{3\kappa_0G}\right)^{1/2}K_0^{-1}\mu^2M^{-1}(t-t_0)}.
$$

When the accumulated contraction term dominates the initial-radius term, $R\propto\mu^{-4/7}M^{2/7}(t-t_0)^{-2/7}$. Substitution into the central [ideal gas](../../../thermodynamics.md#ideal-gas) relation gives

$$
\boxed{T_c\propto\mu^{11/7}M^{5/7}(t-t_0)^{2/7}},
$$

which has the stated $t^{2/7}$ behavior when the time origin is negligible. This late-time approximation still requires the assumed [fully convective star](../../../stellar-structure.md#fully-convective-star), fixed composition and [opacity](../../../stellar-structure.md#opacity) law to remain applicable.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For fully ionized [hydrogen](../../../chemistry.md#hydrogen) and [helium](../../../chemistry.md#helium) with mass fractions $X$ and $Y=1-X$, the inverse [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight) counts nuclei plus free electrons:

$$
\mu^{-1}=2X+\frac34Y=\frac34+\frac54X.
$$

Thus $\mu_1=8/13$ for $X_1=0.7$, $\mu_2=4/7$ for $X_2=0.8$, and $\mu_1/\mu_2=14/13$. Keep the same $M,\kappa_0$ and dimensionless structure constants when comparing these toy sequences. From part (a),

$$
T_e\propto\mu^{1/2}M^{1/4}R^{1/8},\qquad L\propto\mu^2MR^{5/2}.
$$

Eliminating $R$ gives the [composition shift of a convective pre-main-sequence track](../../../stellar-astrophysics.md#composition-shift-of-a-convective-pre-main-sequence-track):

$$
\boxed{L\propto\mu^{-8}M^{-4}T_e^{20}}.
$$

Consequently the tracks in a [Hertzsprung-Russell diagram](../../../stellar-astrophysics.md#hertzsprung-russell-diagram) are almost vertical, with $d\log L/d\log T_e=20$. At equal [luminosity](../../../astrophysics.md#luminosity), $T_{e,1}/T_{e,2}=(14/13)^{2/5}\simeq1.030$: **the $X=0.7$ track lies to the hotter, left-hand side of the $X=0.8$ track**. Since contraction decreases $R$, both $L$ and $T_e$ decrease in this particular [opacity](../../../stellar-structure.md#opacity) model. Both arrows therefore point downward and slightly rightward on the conventional hot-left diagram.

<a id="1/b/image-convective-contraction-tracks-at-equal-mass-with-evolution-downward-and-rightward"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63-convective-tracks.png)

**[Figure 1](#1/b/image-convective-contraction-tracks-at-equal-mass-with-evolution-downward-and-rightward). Convective contraction tracks at equal mass, with evolution downward and rightward**.

The plotted reference scales are arbitrary; the horizontal separation is the predicted $\Delta\log_{10}T_e=(2/5)\log_{10}(14/13)$. They are schematic [Hayashi tracks](../../../stellar-astrophysics.md#hayashi-track) under the specified atmospheric [opacity](../../../stellar-structure.md#opacity) law, rather than calibrated stellar models.

A [protostar](../../../stellar-astrophysics.md#protostar) leaves this contraction sequence when its assumptions fail. Increasing [central stellar temperature](../../../stellar-structure.md#central-stellar-temperature) makes [stellar nuclear fusion](../../../stellar-astrophysics.md#stellar-nuclear-fusion) significant: burning of [deuterium](../../../chemistry.md#deuterium) can temporarily slow contraction, and sustained [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning) brings the star to the [main sequence](../../../stellar-astrophysics.md#main-sequence). In a sufficiently massive [pre-main-sequence star](../../../stellar-astrophysics.md#pre-main-sequence-star), a [radiative core](../../../stellar-structure.md#radiative-core) develops, the interior ceases to share one adiabat, and evolution can proceed along a hotter [Henyey track](../../../stellar-astrophysics.md#henyey-track). Changing atmospheric [opacity](../../../stellar-structure.md#opacity), partial [ionization](../../../physics.md#ionization), or substantial continuing [accretion](../../../astrophysics.md#accretion) also changes the predicted path. For sufficiently low mass, [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) instead limits the increase of central temperature, as in part (c).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Retain fixed dimensionless structure constants and fixed $M$. Write the assumed [stellar homology](../../../stellar-structure.md#stellar-homology) relations as $P_c=C_PGM^2/R^4$ and $\rho_c=C_\rho M/R^3$. The [equation of state](../../../thermodynamics.md#equation-of-state) gives

$$
T_c=\frac{\mu_i}{\mathcal R}\left(\frac{P_c}{\rho_c}-K_{\rm nr}\rho_c^{2/3}\right)=\frac{\mu_i}{\mathcal R}\left(AG\frac{M}{R}-BK_{\rm nr}\frac{M^{2/3}}{R^2}\right),
$$

where $A=C_P/C_\rho$ and $B=C_\rho^{2/3}$. The first term is the temperature required for ordinary thermal [pressure](../../../thermodynamics.md#pressure) support; the second subtracts the support supplied by nonrelativistic [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure).

As a function of $u=1/R$, this is a concave [quadratic polynomial](../../../polynomial.md#quadratic-polynomial). Differentiation gives

$$
u_{\max}=\frac{AG}{2BK_{\rm nr}}M^{1/3},\qquad R_{\max}=\frac{2BK_{\rm nr}}{AG}M^{-1/3},
$$

and substitution proves

$$
\boxed{T_{\max}=\frac{A^2G^2}{4B\mathcal R K_{\rm nr}}\mu_iM^{4/3}\propto\mu_iM^{4/3}}.
$$

The scaling holds at fixed $K_{\rm nr}$ and homologous profile; changing the [mean molecular weight per electron](../../../thermodynamics.md#mean-molecular-weight-per-electron) also changes $K_{\rm nr}$. At the maximum the ion thermal [pressure](../../../thermodynamics.md#pressure) and [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) contribute equally. Subsequent contraction lets [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) carry more of the load without raising the temperature; eventually the assumed positive-temperature branch approaches a cold, degenerate configuration.

**A sufficiently low-mass object never reaches the temperature needed for sustained [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning), so it becomes a cooling [brown dwarf](../../../stellar-astrophysics.md#brown-dwarf) rather than a hydrogen-burning [star](../../../stellar-astrophysics.md#star) on the [main sequence](../../../stellar-astrophysics.md#main-sequence).** The scaling explains a [hydrogen-burning minimum mass](../../../stellar-astrophysics.md#hydrogen-burning-minimum-mass); its numerical value additionally requires the composition, detailed structure and nuclear ignition conditions, which are not specified here.

## 2

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The event rate counts unordered pairs of reacting [nuclei](../../../physics.md#atomic-nucleus). For unlike species there are $n_in_j$ pairs per unit-volume normalization; for identical species there are approximately $n_i^2/2$ pairs, since counting ordered pairs counts each collision twice. The [Kronecker delta](../../../linear-algebra.md#kronecker-delta) therefore supplies exactly the required divisor $1+\delta_{ij}$. It is the event rate, not the destruction rate of identical nuclei: one identical-pair reaction destroys two nuclei.

The [temperature](../../../thermodynamics.md#temperature) dependence combines the high-energy tail of the [Maxwell-Boltzmann distribution](../../../statistical-physics.md#maxwell-boltzmann-distribution) with [quantum tunnelling](../../../quantum-mechanics.md#quantum-tunnelling) through the [Coulomb barrier](../../../physics.md#coulomb-barrier). The principal exponential factor in the energy integral is $\exp[-E/(k_BT)-b/\sqrt E]$. Its stationary point, the [Gamow peak](../../../stellar-astrophysics.md#gamow-peak), has $E_0\propto T^{2/3}$ and exponent $\eta=3E_0/(k_BT)\propto T^{-1/3}$. Integrating around this peak gives a prefactor proportional to $T^{-2/3}$, or $\eta^2$, when the nuclear factor varies slowly. Thus the supplied [thermonuclear reaction rate](../../../stellar-astrophysics.md#thermonuclear-reaction-rate) is locally proportional to $\eta^2e^{-\eta}$. The slow weak interaction in the proton-proton reaction also makes its overall coefficient very small; its local thermal slope follows the supplied formula.

At fixed [number densities](../../../statistical-physics.md#number-density), define the [local temperature exponent of a thermonuclear reaction](../../../stellar-astrophysics.md#local-temperature-exponent-of-a-thermonuclear-reaction) by a logarithmic derivative. Since $d\eta/d\log T=-\eta/3$,

$$
\frac{d\log\lambda_{ij}}{d\log T}=(2/\eta-1)(-\eta/3)=\frac{\eta-2}{3}.
$$

For proton-proton reactions, $A=1/2$ and $Z_1=1$. At $T_6=15$, $\eta_{11}=13.67$ and $\alpha=3.89$. For two [helium-3](../../../chemistry.md#helium-3) nuclei, $A=3/2$ and $Z_3^2Z_3^2=16$, giving $\eta_{33}=49.68$ and $\beta=15.89$. For [helium-3](../../../chemistry.md#helium-3) with [helium-4](../../../chemistry.md#helium-4), $A=12/7$ and the same charge product gives $\eta_{34}=51.95$ and $\gamma=16.65$. Hence

$$
\boxed{\alpha\simeq4,\qquad\beta\simeq16,\qquad\gamma\simeq16,\quad\gamma>\beta}.
$$

These are local powers near the specified temperature, not constant exponents over an arbitrarily large range. The greater reduced nuclear mass in the $34$ reaction increases its tunnelling exponent and its thermal sensitivity.

For the [effective proton-proton reaction network](../../../stellar-astrophysics.md#effective-proton-proton-reaction-network), denote the event rates by

$$
R_{11}=\tfrac12\lambda_{11}n_1^2,\quad R_{21}=\lambda_{21}n_2n_1,\quad R_{33}=\tfrac12\lambda_{33}n_3^2,\quad R_{34}=\lambda_{34}n_3n_4,\quad R_{17}=\lambda_{17}n_1n_7.
$$

The short-lived beryllium intermediate can be eliminated, so production through $R_{34}$ feeds $n_7$, representing predominantly lithium-7. This rapid conversion is [electron capture](../../../physics.md#electron-capture). Count the nuclei consumed and produced in each reaction: $11$ consumes two protons and makes one [deuterium](../../../chemistry.md#deuterium); $21$ consumes a proton and a [deuterium](../../../chemistry.md#deuterium) and makes one [helium-3](../../../chemistry.md#helium-3); $33$ consumes two [helium-3](../../../chemistry.md#helium-3) and makes one [helium-4](../../../chemistry.md#helium-4) and two protons; $34$ consumes one of each helium isotope; $17$ consumes a proton and lithium-7 and makes two [helium-4](../../../chemistry.md#helium-4). It follows that

$$
\begin{aligned}
\dot n_1&=-\lambda_{11}n_1^2-\lambda_{21}n_2n_1+\lambda_{33}n_3^2-\lambda_{17}n_1n_7,\\
\dot n_2&=\tfrac12\lambda_{11}n_1^2-\lambda_{21}n_2n_1,\\
\dot n_3&=\lambda_{21}n_2n_1-\lambda_{33}n_3^2-\lambda_{34}n_3n_4,\\
\dot n_4&=\tfrac12\lambda_{33}n_3^2-\lambda_{34}n_3n_4+2\lambda_{17}n_1n_7.
\end{aligned}
$$

For closure, $\dot n_7=\lambda_{34}n_3n_4-\lambda_{17}n_1n_7$. These nuclear terms conserve $n_1+2n_2+3n_3+4n_4+7n_7$, providing an independent stoichiometric check. They describe a fixed local volume; compression or mixing would add transport terms.

The roughly one-second destruction time of [deuterium](../../../chemistry.md#deuterium) is negligible compared with the proton-burning and [helium-3](../../../chemistry.md#helium-3) evolution times. Its abundance rapidly adjusts to the slowly evolving production rate. Set $\dot n_2\simeq0$, giving the [deuterium quasi-equilibrium in proton-proton burning](../../../stellar-astrophysics.md#deuterium-quasi-equilibrium-in-proton-proton-burning)

$$
\lambda_{21}n_2n_1\simeq\tfrac12\lambda_{11}n_1^2,\qquad n_2\simeq\frac{\lambda_{11}n_1}{2\lambda_{21}}.
$$

Substitution, without setting $\dot n_1=0$, gives

$$
\boxed{\begin{aligned}
\dot n_1&\simeq-\tfrac32\lambda_{11}n_1^2+\lambda_{33}n_3^2-\lambda_{17}n_1n_7,\\
\dot n_3&\simeq\tfrac12\lambda_{11}n_1^2-\lambda_{33}n_3^2-\lambda_{34}n_3n_4.
\end{aligned}}
$$

The [helium-3 relaxation time](../../../stellar-astrophysics.md#helium-3-relaxation-time) of about $6\times10^5$ years is likewise short compared with the central proton-burning time and the age of the [Sun](../../../stellar-astrophysics.md#sun). On this relaxation time the proton and [helium-4](../../../chemistry.md#helium-4) abundances, and the background temperature, can be treated as fixed. Put $A=\lambda_{33}$, $B=\lambda_{34}n_4$, $C=\lambda_{11}n_1^2/2$. Then $\dot n_3=C-An_3^2-Bn_3$, and its nonnegative equilibrium is

$$
\boxed{n_{3e}=-\frac{\lambda_{34}n_4}{2\lambda_{33}}+\sqrt{\left(\frac{\lambda_{34}n_4}{2\lambda_{33}}\right)^2+\frac{\lambda_{11}n_1^2}{2\lambda_{33}}}}.
$$

The other root is negative and unphysical. Write $n_3=n_{3e}+x$ and subtract the equilibrium equation. Exactly, for a fixed background,

$$
\dot x=-(2\lambda_{33}n_{3e}+\lambda_{34}n_4)x-\lambda_{33}x^2.
$$

Dropping the quadratic displacement gives

$$
\boxed{\dot x=-x/\tau,\qquad\tau=(2\lambda_{33}n_{3e}+\lambda_{34}n_4)^{-1}}.
$$

Thus small displacements decay exponentially. A slowly moving equilibrium introduces an additional $-\dot n_{3e}$ term, negligible to leading order when $\tau$ is short compared with background evolution.

To estimate the [temperature for helium-3 freeze-out](../../../stellar-astrophysics.md#temperature-for-helium-3-freeze-out), use the cooler pp-I-dominated region and neglect $B$ compared with $2An_{3e}$. Then $n_{3e}\simeq n_1\sqrt{\lambda_{11}/(2\lambda_{33})}$ and $\tau^{-1}\simeq n_1\sqrt{2\lambda_{11}\lambda_{33}}$. With the local powers just obtained and fixed proton [number density](../../../statistical-physics.md#number-density), $n_{3e}\propto T^{-6}$ and $\tau\propto T^{-10}$. Adopting $t_\odot\simeq4.6\times10^9\,\mathrm{yr}$ gives

$$
T\simeq15\times10^6\left(\frac{6\times10^5}{4.6\times10^9}\right)^{1/10}\!\mathrm K\simeq\boxed{6.1\times10^6\,\mathrm K}.
$$

This is an order-of-magnitude extrapolation of local exponents. Keeping the supplied exponential factors gives the [helium-3 freeze-out estimate with Gamow factors](../../../stellar-astrophysics.md#helium-3-freeze-out-estimate-with-gamow-factors)

$$
\frac{\tau(T)}{\tau(T_c)}=\left(\frac{T}{T_c}\right)^{2/3}\exp\!\left[\frac{\eta_{11,c}+\eta_{33,c}}2\left(\left(\frac{T_c}{T}\right)^{1/3}-1\right)\right],
$$

which yields about $6.8\times10^6\,\mathrm K$ with the same normalization and fixed-density approximation. Thus the robust estimate is several million kelvin. The supplied data do not fix the local density, composition or pp-II fraction away from the centre, so they cannot determine an exact transition temperature or radius. In particular, using $\tau\propto T^{-16}$ alone would omit the temperature dependence of the equilibrium [helium-3](../../../chemistry.md#helium-3) abundance.

The [solar hydrogen and helium-3 abundance profiles](../../../stellar-astrophysics.md#solar-hydrogen-and-helium-3-abundance-profiles) follow from burning, finite equilibration time and [convection](../../../fluid-mechanics.md#convection). Central [hydrogen](../../../chemistry.md#hydrogen) has been consumed, so $X_1$ is lowest in the centre and increases toward its much less processed outer value. In the hot centre, rapid destruction keeps [helium-3](../../../chemistry.md#helium-3) small. Moving outward initially raises its equilibrium abundance because $\lambda_{11}/\lambda_{33}$ rises strongly as temperature falls. Further out, equilibration is no longer reached within the solar age, and still farther out even production is slow. Hence $X_3$ has an off-centre maximum and then declines toward its small outer abundance. The outer convective envelope mixes each abundance toward a constant value.

<a id="2/image-present-solar-hydrogen-depletion-and-the-off-centre-helium-3-abundance-maximum"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63-solar-abundances.png)

**[Figure 2](#2/image-present-solar-hydrogen-depletion-and-the-off-centre-helium-3-abundance-maximum). Present solar hydrogen depletion and the off-centre helium-3 abundance maximum**.

The sketch shows these qualitative shapes; the helium-3 ordinate is scaled to its own maximum. The illustrated amplitudes, peak radius and envelope boundary are schematic, not a numerical solar-model solution.

## 3

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the secular, circular-orbit approximation: the wind escapes fast enough to avoid appreciable interaction with the companion, while the stellar masses change slowly enough that orbital elements describe the evolving [binary star](../../../stellar-astrophysics.md#binary-star). Neglect spin [angular momentum](../../../classical-mechanics.md#angular-momentum). Let $\omega=(GM/a^3)^{1/2}$ be the orbital angular speed. The donor's distance from the centre of mass is $a_1=aM_2/M$, and the [circular-binary orbital angular momentum](../../../stellar-astrophysics.md#circular-binary-orbital-angular-momentum) is

$$
J_{\rm orb}=\frac{M_1M_2}{M}a^2\omega=M_1M_2\left(\frac{Ga}{M}\right)^{1/2}.
$$

A spherically symmetric wind in the donor frame has zero mean additional angular momentum about the donor. Averaging its angular momentum about the binary centre of mass therefore gives the donor's orbital specific angular momentum, $j_1=a_1^2\omega$. Since $\dot M<0$ denotes mass removed from the system, $\dot J_{\rm orb}=j_1\dot M$, and

$$
\boxed{\frac{\dot J_{\rm orb}}{J_{\rm orb}}=\frac{M_2\dot M}{M_1M}}.
$$

This is [donor-wind angular-momentum loss](../../../stellar-astrophysics.md#donor-wind-angular-momentum-loss) in the [Jeans-mode mass loss](../../../stellar-astrophysics.md#jeans-mode-mass-loss) approximation.

First allow only wind loss, so $\dot M_1=\dot M$ and $\dot M_2=0$. The logarithmic derivative of $J_{\rm orb}$ gives

$$
\frac{M_2\dot M}{M_1M}=\frac{\dot M}{M_1}+\frac12\frac{\dot a}{a}-\frac12\frac{\dot M}{M}.
$$

Solving yields $\dot a/a=-\dot M/M$. By [Kepler's third law](../../../physics.md#kepler-s-third-law), $P^2=4\pi^2a^3/(GM)$, so $\dot P/P=-2\dot M/M$. Integrating gives

$$
\boxed{aM=\mathrm{constant},\qquad PM^2=\mathrm{constant}}.
$$

Wind loss thus expands the separation and lengthens the orbital period. These are secular relations; an impulsive loss on an orbital time could instead generate eccentricity and would need a different analysis.

To test contact, put $D=d\log(R_1/R_L)/dt$. The given short-time [stellar radius response exponent](../../../stellar-astrophysics.md#stellar-radius-response-exponent) gives $\dot R_1/R_1=-n\dot M_1/M_1$. Differentiating the [Roche lobe](../../../stellar-astrophysics.md#roche-lobe) approximation gives

$$
\frac{\dot R_L}{R_L}=\frac{\dot a}{a}+\frac13\left(\frac{\dot M_1}{M_1}-\frac{\dot M}{M}\right).
$$

For wind alone this becomes $\dot R_L/R_L=\dot M/(3M_1)-4\dot M/(3M)$. Hence, with the [binary mass ratio](../../../stellar-astrophysics.md#binary-mass-ratio) $q=M_1/M_2$,

$$
D_{\rm w}=-\left(n+\frac13\right)\frac{\dot M}{M_1}+\frac{4\dot M}{3M}=\frac{\dot M}{3M_1(1+q)}\left[3(1-n)q-(1+3n)\right].
$$

Because $\dot M$ is negative, increasing overfill, $D_{\rm w}>0$, occurs precisely when

$$
\boxed{q<\frac{1+3n}{3(1-n)}}.
$$

This is [wind-driven Roche-lobe overflow](../../../stellar-astrophysics.md#wind-driven-roche-lobe-overflow). For the reverse strict inequality, $D_{\rm w}<0$ and the [donor star](../../../stellar-astrophysics.md#donor-star) retreats inside its [Roche lobe](../../../stellar-astrophysics.md#roche-lobe), producing a [detached binary](../../../stellar-astrophysics.md#detached-binary). At equality the wind is neutral to contact at this order.

Now permit an additional [conservative binary mass transfer](../../../stellar-astrophysics.md#conservative-binary-mass-transfer) rate $x=\dot M_2$ to the [mass-gaining star](../../../stellar-astrophysics.md#mass-gaining-star). The total escaping wind remains $\dot M$, while $\dot M_1=\dot M-x$. Transfer retains orbital angular momentum within the binary under the assumed neglect of spins, so the same wind-loss formula for $\dot J_{\rm orb}$ applies. Logarithmic differentiation now gives

$$
\frac{\dot a}{a}=-\frac{\dot M}{M}+2x\left(\frac1{M_1}-\frac1{M_2}\right).
$$

Substituting this and $\dot M_1=\dot M-x$ into the two radius derivatives gives

$$
D=D_{\rm w}+\frac{x}{3M_1}(6q-5+3n).
$$

Steady contact requires $D=0$. If the wind is driving overflow and $6q<5-3n$, the transfer contribution reduces overfill and a positive contact rate exists:

$$
\boxed{\dot M_2=-\frac{1+3n-3(1-n)q}{(1+q)(5-3n-6q)}\dot M}.
$$

The numerator and denominator are positive in this regime, making $\dot M_2>0$. This explicitly establishes both the [contact transfer rate with Jeans-mode wind loss](../../../stellar-astrophysics.md#contact-transfer-rate-with-jeans-mode-wind-loss) and its stabilizing sign.

If the wind drives overflow but $6q>5-3n$, positive transfer instead increases $R_1/R_L$: the mass loss required to relieve overfill makes the overfill worse. The formal contact formula would require $\dot M_2<0$, which is not donor-to-companion transfer. **There is no stabilizing positive contact rate; overflow runs away.** For a [red giant](../../../stellar-astrophysics.md#red-giant) this can lead to a [common envelope](../../../stellar-astrophysics.md#common-envelope), followed by envelope ejection into a tighter binary or a merger. The criterion concerns the supplied short-time radius response; the actual runaway timescale and outcome require the donor's dynamical and thermal response. At $6q=5-3n$ transfer is neutral to contact at this order, so it cannot balance a nonzero wind driver. If the wind already causes detachment, the transfer instability condition alone does not initiate overflow.

## 4

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [stellar polytrope](../../../stellar-structure.md#stellar-polytrope) replaces a detailed [equation of state](../../../thermodynamics.md#equation-of-state) and thermal structure by $P=K\rho^{1+1/n}$ for $n>0$, with spatially constant $K$ and [polytropic index](../../../stellar-structure.md#polytropic-index) $n$. Together with spherical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) and mass conservation, it gives a tractable family of stellar density profiles. Introduce the [Lane-Emden variables for a stellar polytrope](../../../stellar-structure.md#lane-emden-variables-for-a-stellar-polytrope)

$$
\rho=\rho_c\theta^n,\qquad r=b\xi,\qquad b^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1}.
$$

Combining $dP/dr=-Gm\rho/r^2$ with $dm/dr=4\pi r^2\rho$ eliminates $m$ to give $r^{-2}d[r^2\rho^{-1}(dP/dr)]/dr=-4\pi G\rho$. Substitution of the pressure law and the dimensionless variables gives the [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation)

$$
\frac1{\xi^2}\frac{d}{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n,\qquad\theta(0)=1,\quad\theta'(0)=0.
$$

A regular finite-radius model for $0\leq n<5$ ends at the first zero $\xi_1$. Its radius and mass are

$$
R=b\xi_1,\qquad M=4\pi b^3\rho_c[-\xi_1^2\theta'(\xi_1)].
$$

These formulas supply central-to-mean density ratios and [stellar homology](../../../stellar-structure.md#stellar-homology) scalings without solving a full evolutionary model. Eliminating $\rho_c$, for $0<n<5$ and $n\ne3$, gives the [polytropic mass-radius relation](../../../stellar-structure.md#polytropic-mass-radius-relation)

$$
R\propto K^{n/(3-n)}G^{-n/(3-n)}M^{(1-n)/(3-n)}.
$$

An efficient-convection [monatomic gas](../../../thermodynamics.md#monatomic-gas) has $n=3/2$. The same index describes a cold, nonrelativistic [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) law; at fixed composition it gives $R\propto M^{-1/3}$ for a [white dwarf](../../../stellar-astrophysics.md#white-dwarf). Ultrarelativistic [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) has $n=3$, for which the mass is independent of $\rho_c$ and scales as $(K/G)^{3/2}$. This is the origin of the [Chandrasekhar limit](../../../stellar-astrophysics.md#chandrasekhar-limit). A radiation-dominated, approximately constant-entropy interior also approaches $P\propto\rho^{4/3}$ and $n=3$. The [polytrope of index zero](../../../stellar-structure.md#polytrope-of-index-zero) is an incompressible comparison model, useful for illustrating the role of central concentration.

The [gravitational energy of a stellar polytrope](../../../stellar-structure.md#gravitational-energy-of-a-stellar-polytrope), $\Omega=-3GM^2/[(5-n)R]$, and the [stellar virial theorem](../../../stellar-structure.md#stellar-virial-theorem) make polytropes useful for contraction-energy estimates. They also provide structural models for perturbation and stability calculations. **A polytrope is a structural approximation, not a complete stellar evolution calculation.** One must still specify [stellar nuclear fusion](../../../stellar-astrophysics.md#stellar-nuclear-fusion), [opacity](../../../stellar-structure.md#opacity), energy transport, composition and boundary conditions to determine the [luminosity](../../../astrophysics.md#luminosity) and history. Moreover, the structural exponent $1+1/n$ need not equal the [adiabatic exponent](../../../thermodynamics.md#heat-capacity-ratio) relevant to a rapid perturbation. Real stars can have different effective indices in their cores and envelopes, as well as [ionization](../../../physics.md#ionization) zones or varying [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The first argument is the energy budget. The gravitational energy reservoir is of order $GM^2/R$, so the [Kelvin-Helmholtz cooling time](../../../stellar-astrophysics.md#kelvin-helmholtz-cooling-time) is $t_{\rm KH}\sim GM^2/(RL)$. For the [Sun](../../../stellar-astrophysics.md#sun), $M\simeq2\times10^{30}\,\mathrm{kg}$, $R\simeq7\times10^8\,\mathrm m$ and $L\simeq3.8\times10^{26}\,\mathrm W$ give $t_{\rm KH}\sim3\times10^7$ years. This is much shorter than the approximately $4.6\times10^9$-year solar-system age. Chemical binding energies are only of order electronvolts per atom and provide an even smaller reservoir. Thus neither ordinary chemical energy nor continuing gravitational contraction can supply the long-term solar [luminosity](../../../astrophysics.md#luminosity).

[Stellar nuclear fusion](../../../stellar-astrophysics.md#stellar-nuclear-fusion) provides an adequate reservoir. Conversion of four [hydrogen](../../../chemistry.md#hydrogen) atoms into one [helium-4](../../../chemistry.md#helium-4) atom releases about $26.7\,\mathrm{MeV}$, corresponding to a mass defect of about $0.007$ of the initial mass; some energy leaves as [neutrinos](../../../standard-model.md#neutrino). If a fraction $f$ of stellar mass with hydrogen fraction $X$ is available for core burning, the energy scale is $0.007fXMc^2$. Taking $f\sim0.1$ and $X\sim0.7$ supplies roughly $9\times10^{43}\,\mathrm J$, enough for several billion years at the solar [luminosity](../../../astrophysics.md#luminosity), consistent with a [stellar nuclear timescale](../../../stellar-astrophysics.md#stellar-nuclear-timescale) of order $10^{10}$ years. The core temperature and density inferred from stellar structure permit the [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain); hotter stellar cores favor the [CNO cycle](../../../stellar-astrophysics.md#cno-cycle).

The most direct evidence is the detection of [solar neutrinos](../../../stellar-astrophysics.md#solar-neutrino). They are created in the weak reactions of the [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) and can escape from the core, unlike the [photons](../../../quantum-mechanics.md#photon) whose transport through the interior is slow. Measurements accounting for [neutrino oscillation](../../../standard-model.md#neutrino-oscillation) recover a total neutrino flux consistent with nuclear-powered solar models. Their spectra and reaction-dependent fluxes test the core reactions rather than merely the surface [effective temperature](../../../stellar-structure.md#effective-temperature).

There is also independent evidence from [stellar evolution](../../../stellar-astrophysics.md#stellar-evolution): the [main sequence](../../../stellar-astrophysics.md#main-sequence) is a long-lived core-hydrogen-burning phase, more massive luminous stars consume fuel more quickly, and the [main-sequence turnoff](../../../stellar-astrophysics.md#main-sequence-turnoff) of a star cluster records its age. Subsequent evolution and the production of heavier elements fit further [nuclear reactions](../../../physics.md#nuclear-reaction). Agreement among these observations, nuclear energy release and stellar-model lifetimes is much stronger than the energy-budget argument alone. **The combination of a sufficient nuclear reservoir, measured core neutrinos and the observed evolutionary sequence identifies nuclear reactions as the main long-term power source of ordinary stars.**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

A [Type Ia supernova](../../../stellar-astrophysics.md#type-ia-supernova) is a thermonuclear disruption associated with a [carbon-oxygen white dwarf](../../../stellar-astrophysics.md#carbon-oxygen-white-dwarf) in a binary system. [Electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) supports the dense star, and initially depends much less on temperature than an [ideal gas](../../../thermodynamics.md#ideal-gas) pressure does. Once carbon burning heats degenerate material, the immediate pressure response is insufficient to produce the usual expansion-and-cooling thermostat. The strongly temperature-sensitive [nuclear reactions](../../../physics.md#nuclear-reaction) can therefore undergo a [thermonuclear runaway](../../../stellar-astrophysics.md#thermonuclear-runaway).

One channel involves [accretion](../../../astrophysics.md#accretion) toward the [Chandrasekhar limit](../../../stellar-astrophysics.md#chandrasekhar-limit), about $1.4$ solar masses for a typical electron composition. Other proposed channels involve merging [white dwarfs](../../../stellar-astrophysics.md#white-dwarf) or an initial helium-layer detonation that triggers carbon burning below that mass. Thus the [Chandrasekhar limit](../../../stellar-astrophysics.md#chandrasekhar-limit) motivates an important model, but it is not an assumption that every [Type Ia supernova](../../../stellar-astrophysics.md#type-ia-supernova) has exactly the same progenitor mass or ignition history. Burning carbon and oxygen into more tightly bound nuclei releases enough [nuclear binding energy](../../../physics.md#nuclear-binding-energy) to overcome the stellar gravitational binding energy. An ordinary successful event ejects the star rather than leaving the compact core characteristic of a [core-collapse supernova](../../../stellar-astrophysics.md#core-collapse-supernova).

The ejecta contain iron-group material, including radioactive nickel-56, and intermediate-mass elements from incomplete burning. The [radioactively powered Type Ia supernova light curve](../../../stellar-astrophysics.md#radioactively-powered-type-ia-supernova-light-curve) is powered largely by the nickel-56 to cobalt-56 to iron-56 decay chain: its energetic products heat the ejecta, and [radiative diffusion](../../../astrophysics.md#radiative-diffusion) delays the emerging radiation. Near maximum light, ordinary [Type Ia supernovae](../../../stellar-astrophysics.md#type-ia-supernova) show prominent silicon absorption and lack the hydrogen lines defining Type II events. The spectral classification and the thermonuclear mechanism provide complementary descriptions.

The similar progenitors and radioactive power make [Type Ia supernovae](../../../stellar-astrophysics.md#type-ia-supernova) useful [standard candles](../../../astrophysics.md#standard-candle), but their peak [luminosities](../../../astrophysics.md#luminosity) are not identical. The relation between [light curve](../../../astrophysics.md#light-curve) width and peak brightness, together with color corrections, allows standardization for distance measurements. Extinction, composition and explosion diversity still introduce systematic uncertainties. **A Type Ia event is a white-dwarf thermonuclear explosion with a radioactively powered light curve; its corrected luminosity makes it a valuable distance indicator.**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

An [X-ray binary](../../../stellar-astrophysics.md#x-ray-binary) contains a compact accretor supplied by a [donor star](../../../stellar-astrophysics.md#donor-star). Most bright systems contain a [neutron star](../../../stellar-astrophysics.md#neutron-star) or [black hole](../../../general-relativity.md#black-hole). Gas arrives by [Roche-lobe overflow](../../../stellar-astrophysics.md#roche-lobe-overflow), a captured [stellar wind](../../../stellar-astrophysics.md#stellar-wind), or donor outflows, commonly forming an [accretion disk](../../../astrophysics.md#accretion-disk). The primary energy source is the release of gravitational binding energy during [accretion](../../../astrophysics.md#accretion), with a characteristic [accretion luminosity](../../../stellar-astrophysics.md#accretion-luminosity)

$$
L\sim\frac{GM\dot M_{\rm acc}}{R_{\rm in}}\sim\epsilon\dot M_{\rm acc}c^2.
$$

For a [neutron star](../../../stellar-astrophysics.md#neutron-star), $R_{\rm in}$ can be near its material radius; for a [black hole](../../../general-relativity.md#black-hole), radiation is produced by the flow outside the horizon. For $M\sim1.4M_\odot$ and $R\sim10\,\mathrm{km}$, $GM/(Rc^2)\sim0.2$, so accretion can release much more energy per unit mass than hydrogen burning. The hot inner flow, boundary layer or accretion column emits [X-rays](../../../electromagnetism.md#x-ray).

In a [high-mass X-ray binary](../../../stellar-astrophysics.md#high-mass-x-ray-binary), a massive, relatively short-lived donor often supplies gas through a strong wind or an equatorial outflow; some systems instead undergo [Roche-lobe overflow](../../../stellar-astrophysics.md#roche-lobe-overflow). These objects trace young stellar populations. In a [low-mass X-ray binary](../../../stellar-astrophysics.md#low-mass-x-ray-binary), a lower-mass donor commonly fills its [Roche lobe](../../../stellar-astrophysics.md#roche-lobe) and feeds a disk. Such systems can persist in older populations. These mass labels refer to the donor, not the compact accretor.

A magnetized [neutron star](../../../stellar-astrophysics.md#neutron-star) can channel accretion onto its poles, producing an [accreting X-ray pulsar](../../../stellar-astrophysics.md#accreting-x-ray-pulsar) as the star rotates. Accretion transfers [angular momentum](../../../classical-mechanics.md#angular-momentum), so changes in spin constrain the flow and magnetic coupling. A [Type I X-ray burst](../../../stellar-astrophysics.md#type-i-x-ray-burst) has a different origin: accumulated [hydrogen](../../../chemistry.md#hydrogen) or [helium](../../../chemistry.md#helium) undergoes unstable thermonuclear burning on a [neutron star](../../../stellar-astrophysics.md#neutron-star) surface. It rises rapidly and then cools as the fuel is exhausted. A [black hole](../../../general-relativity.md#black-hole) has no material surface supporting the same surface-fuel mechanism.

Orbital motion and optical observations of the donor constrain masses, with inclination and donor-model uncertainties. A compact mass exceeding plausible stable [neutron star](../../../stellar-astrophysics.md#neutron-star) masses supports a [black hole](../../../general-relativity.md#black-hole) interpretation. Rapid variability probes the small emitting region, while disk spectra and recurrent outbursts probe [accretion](../../../astrophysics.md#accretion) and its instabilities. The [Eddington luminosity](../../../stellar-structure.md#eddington-luminosity),

$$
L_{\rm Edd}=\frac{4\pi GMc}{\kappa},
$$

is obtained by balancing radiative acceleration $\kappa L/(4\pi r^2c)$ against $GM/r^2$; it is a useful luminosity scale under the assumed isotropic, opacity-controlled force law. Geometry and time dependence can complicate its application. **X-ray binaries reveal compact stars through efficient gravitational accretion, with pulsations, bursts and orbital dynamics distinguishing their physical components.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
