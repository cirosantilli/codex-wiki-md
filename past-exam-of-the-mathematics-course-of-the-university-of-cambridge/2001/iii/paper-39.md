# Paper 39

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper39.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper39.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [specific intensity](../../../astrophysics.md#specific-intensity) of a [blackbody](../../../astrophysics.md#blackbody) is direction-independent over its outward hemisphere. Its outward flux per unit frequency is therefore

$$
F_\nu=\int_{\rm outward} B_\nu\cos\theta\,d\Omega
=2\pi B_\nu\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta=\pi B_\nu.
$$

Multiplying by the stellar surface area gives the [spectral luminosity](../../../astrophysics.md#spectral-luminosity)

$$
\boxed{L_\nu=4\pi^2R_s^2B_\nu.}
$$

Using the [Planck law](../../../statistical-physics.md#planck-s-law), the [hydrogen-ionizing photon production rate](../../../galaxy.md#hydrogen-ionizing-photon-production-rate) follows by dividing each spectral contribution by its [photon](../../../quantum-mechanics.md#photon) energy and integrating above the threshold:

$$
Q_H=\int_{I_H/h}^\infty\frac{L_\nu}{h\nu}\,d\nu
=\frac{8\pi^2R_s^2}{c^2}\int_{I_H/h}^\infty\frac{\nu^2}{e^{h\nu/kT_s}-1}\,d\nu.
$$

With $x=h\nu/(kT_s)$ and $y=I_H/(kT_s)$, this becomes

$$
Q_H=\frac{8\pi^2I_H^3}{h^3c^2}\frac{R_s^2}{y^3}
\int_y^\infty\frac{x^2}{e^x-1}\,dx.
$$

For the initial hydrogen-only [photon](../../../quantum-mechanics.md#photon) balance, assume an [ionization-bounded nebula](../../../galaxy.md#ionization-bounded-nebula) at steady [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium), negligible dust absorption and ionizing-photon leakage, negligible [collisional ionization](../../../physics.md#collisional-ionization), and local reabsorption of [photons](../../../quantum-mechanics.md#photon) from direct ground-state recombinations. A ground-state recombination then causes another [photoionization](../../../physics.md#photoionization) and produces no net removal of a proton. Net removal is counted by [Case B recombination](../../../galaxy.md#case-b-recombination), whose coefficient is $\beta=\sum_{n\geq2}\alpha_n$. Integrating the local balance gives

$$
\boxed{\int N_eN_+\beta\,dV=Q_H
=\frac{8\pi^2I_H^3}{h^3c^2}\frac{R_s^2}{y^3}
\int_y^\infty\frac{x^2}{e^x-1}\,dx.}
$$

The stellar [temperature](../../../thermodynamics.md#temperature) $T_s$ sets the [photon](../../../quantum-mechanics.md#photon) supply; the gas [temperature](../../../thermodynamics.md#temperature) sets the recombination coefficients. They are not generally equal. For uniform [hydrogen](../../../chemistry.md#hydrogen) and constant gas [temperature](../../../thermodynamics.md#temperature), the [Strömgren radius](../../../galaxy.md#stromgren-radius) is

$$
R_H=\left(\frac{3Q_H}{4\pi\beta_HN_eN_H}\right)^{1/3},
$$

with $N_e=N_H$ in fully ionized pure [hydrogen](../../../chemistry.md#hydrogen).

For the hydrogen-helium mixture, define the [blackbody ionizing photon function](../../../galaxy.md#blackbody-ionizing-photon-function)

$$
F(y)=\int_y^\infty\frac{x^2}{e^x-1}\,dx,\qquad
Q(E_0)=\frac{8\pi^2R_s^2(kT_s)^3}{h^3c^2}F(E_0/kT_s).
$$

The three relevant thresholds are approximately $13.6$, $24.6$ and $54.4\,\mathrm{eV}$, for $\mathrm H^0$, $\mathrm{He}^0$ and $\mathrm{He}^+$ respectively. Higher stellar [temperature](../../../thermodynamics.md#temperature) increases the relative supply of the harder [photons](../../../quantum-mechanics.md#photon). These cumulative [photon](../../../quantum-mechanics.md#photon) rates cannot be assigned independently to the three species: a [photon](../../../quantum-mechanics.md#photon) above a [helium](../../../chemistry.md#helium) threshold can instead ionize [hydrogen](../../../chemistry.md#hydrogen), and [helium](../../../chemistry.md#helium) recombination radiation can also ionize [hydrogen](../../../chemistry.md#hydrogen). The absorption cross-sections and the diffuse radiation determine the effective allocation.

A useful sharp-front model of [nested hydrogen-helium ionization zones](../../../galaxy.md#nested-hydrogen-helium-ionization-zones) has an inner $\mathrm{He}^{++}$ sphere of radius $R_2$, a $\mathrm{He}^+$ shell ending at $R_1$, and an outer hydrogen-ionized region ending at $R_H$, with $R_2\leq R_1\leq R_H$. Let $n_H,n_{He}$ be uniform nuclear number densities. The [electron number densities](../../../statistical-physics.md#electron-number-density) in these three regions are $n_H+2n_{He}$, $n_H+n_{He}$ and $n_H$. For constant gas [temperature](../../../thermodynamics.md#temperature), integrating the recombination rates gives

$$
\begin{aligned}
Q_H^{\rm eff}&=\frac{4\pi}{3}\beta_H n_H\{n_HR_H^3+n_{He}(R_1^3+R_2^3)\},\\
Q_{HeI}^{\rm eff}&=\frac{4\pi}{3}\beta_{HeI}n_{He}(n_H+n_{He})(R_1^3-R_2^3),\\
Q_{HeII}^{\rm eff}&=\frac{4\pi}{3}\beta_{HeII}n_{He}(n_H+2n_{He})R_2^3.
\end{aligned}
$$

Here the effective budgets mean net species-specific ionizations after eliminating local ground-state recycling. Their calculation must include [photon](../../../quantum-mechanics.md#photon) competition and any interspecies diffuse contribution; the [helium](../../../chemistry.md#helium) coefficients label the recombining [ion](../../../chemistry.md#ion)'s emitted spectrum. Once these budgets are specified, solve the third equation for $R_2^3$, the second for $R_1^3-R_2^3$, and the first for $R_H^3$.

For an isolated [helium](../../../chemistry.md#helium) front with approximately common [electron number density](../../../statistical-physics.md#electron-number-density), the useful scaling is

$$
\left(\frac{R_{He}}{R_H}\right)^3
\simeq\frac{Q_{He}^{\rm eff}}{Q_H^{\rm eff}}
\frac{n_H\beta_H}{n_{He}\beta_{He}}.
$$

Thus the small [helium](../../../chemistry.md#helium) abundance partly compensates for the smaller hard-photon supply. A cooler central star produces little $\mathrm{He}^{++}$ and can have a substantially smaller helium-ionized zone. A sufficiently hot star can ionize [helium](../../../chemistry.md#helium) throughout most of the [hydrogen](../../../chemistry.md#hydrogen) region. If independent radius estimates place a [helium](../../../chemistry.md#helium) front beyond the [hydrogen](../../../chemistry.md#hydrogen) front, the independent [photon](../../../quantum-mechanics.md#photon) allocations are inconsistent: the fronts and transfer must be treated together. **The radii depend on [photon](../../../quantum-mechanics.md#photon) hardness, abundance, [electron number density](../../../statistical-physics.md#electron-number-density) and recombination rates, not on thresholds alone.** The sharp-front equations are an approximation; they do not assert three exact independently conserved [photon](../../../quantum-mechanics.md#photon) budgets for a real mixed nebula.

For a nonuniform nebula, an observed [recombination line](../../../physics.md#recombination-line) with [effective recombination coefficient](../../../physics.md#effective-recombination-coefficient) $\alpha_\ell^{\rm eff}$ has [luminosity](../../../astrophysics.md#luminosity)

$$
L_\ell=h\nu_\ell\int N_eN_{\rm parent}\alpha_\ell^{\rm eff}\,dV.
$$

If gas [temperature](../../../thermodynamics.md#temperature) and density permit a known approximately constant ratio $\beta/\alpha_\ell^{\rm eff}$, the integrated line gives

$$
Q^{\rm eff}=\frac{\beta}{\alpha_\ell^{\rm eff}}\frac{L_\ell}{h\nu_\ell}.
$$

The unknown density distribution cancels because the same recombination integral appears in both quantities. For a stellar continuum measurement at a nonionizing frequency $\nu_o$,

$$
F_{\nu_o,*}=\pi B_{\nu_o}(T_s)\frac{R_s^2}{d^2}.
$$

When the inferred recombination budget traces the full appropriate ionizing-photon supply, define $\Phi_{E_0}(T)=\int_{E_0/h}^\infty B_\nu(T)/(h\nu)\,d\nu$ and obtain the [Zanstra method](../../../stellar-astrophysics.md#zanstra-method) equation

$$
\boxed{\frac{F_\ell}{h\nu_\ell F_{\nu_o,*}}\frac{\beta}{\alpha_\ell^{\rm eff}}
=\frac{\Phi_{E_0}(T_s)}{B_{\nu_o}(T_s)}.}
$$

Both $R_s$ and the distance $d$ cancel. [Hydrogen](../../../chemistry.md#hydrogen) and [helium](../../../chemistry.md#helium) recombination lines probe different hardness thresholds, so their ratios and the stellar continuum constrain $T_s$ and test the assumed spectrum and trapping. For a mixed nebula, use the corresponding transfer-corrected [photon](../../../quantum-mechanics.md#photon) budgets. [temperature](../../../thermodynamics.md#temperature) gradients require emission-weighted coefficients; dust, leakage, density-bounded [helium](../../../chemistry.md#helium) zones or departures from a [blackbody](../../../astrophysics.md#blackbody) can produce discrepant [hydrogen](../../../chemistry.md#hydrogen) and [helium](../../../chemistry.md#helium) Zanstra estimates. Line fluxes alone without an appropriate budget or continuum normalization need not uniquely determine $T_s$.

Finally, locate the derived $T_s$ and [luminosity](../../../astrophysics.md#luminosity) on the [Hertzsprung-Russell diagram](../../../stellar-astrophysics.md#hertzsprung-russell-diagram). The central stars are hot exposed cores following [post-asymptotic giant branch evolution](../../../stellar-astrophysics.md#post-asymptotic-giant-branch-evolution): envelope loss creates the [planetary nebula](../../../stellar-astrophysics.md#planetary-nebula), contraction heats the core, and continued shell burning can support an approximately constant [luminosity](../../../astrophysics.md#luminosity) as the star moves leftward. Later the [luminosity](../../../astrophysics.md#luminosity) falls and the remnant approaches the [white dwarf](../../../stellar-astrophysics.md#white-dwarf) cooling sequence. Comparing central-star positions with [stellar evolution](../../../stellar-astrophysics.md#stellar-evolution) tracks constrains core masses and evolutionary ages; comparison with nebular expansion ages tests whether the core heats rapidly enough to ionize the expelled envelope. **The central-star locus traces the transition from an envelope-losing giant to a compact stellar remnant.**

## 2

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Boltzmann distribution](../../../thermodynamics.md#boltzmann-distribution) for two atomic levels at thermodynamic equilibrium is

$$
\boxed{\frac{N_a}{N_b}=\frac{\omega_a}{\omega_b}
\exp\left[-\frac{E_a-E_b}{kT}\right],}
$$

where $\omega$ is the [statistical weight of an atomic level](../../../physics.md#statistical-weight-of-an-atomic-level). For a resolved level of total angular momentum $J$, $\omega=2J+1$ when magnetic substates are unresolved.

To extend this counting to the continuum, assume an ideal, nondegenerate [plasma](../../../physics.md#plasma-physics) with classical free [Electrons](../../../physics.md#electron) and neglect the small difference between the translational masses of the two heavy ionic species. Let $z_e=e^{\mu_e/kT}$ be the [electron fugacity in the Saha equation](../../../cosmology.md#electron-fugacity-in-the-saha-equation), with the [Electron](../../../physics.md#electron) [chemical potential](../../../thermodynamics.md#chemical-potential) measured relative to its rest energy. The two [Electron](../../../physics.md#electron) spin states and the phase-space cell volume $h^3$ give

$$
N_e=\frac{2z_e}{h^3}\int_{\mathbb R^3}e^{-p^2/(2mkT)}\,d^3p
=2z_e\left(\frac{2\pi mkT}{h^2}\right)^{3/2}.
$$

Chemical equilibrium for capture equates the bound species' [chemical potential](../../../thermodynamics.md#chemical-potential) to the sum for its parent [ion](../../../chemistry.md#ion) and free [Electron](../../../physics.md#electron). Thus applying [Boltzmann factors](../../../statistical-physics.md#boltzmann-factor) to a bound level at energy $-I_n$ gives $N_n/N_+=(\omega_n/\omega_+)z_e e^{I_n/kT}$. Eliminating the [Electron](../../../physics.md#electron) fugacity proves the level-specific [Saha ionization equation](../../../cosmology.md#saha-ionization-equation):

$$
\boxed{\frac{N_n}{N_eN_+}
=\frac{\omega_n}{2\omega_+}
\left(\frac{h^2}{2\pi mkT}\right)^{3/2}e^{I_n/kT}.}
$$

The factor two is the [Electron](../../../physics.md#electron) spin multiplicity; the factor with power $3/2$ is the inverse free-electron translational state density. A total-ionization Saha equation sums the bound states into an internal partition function, whereas this expression refers to one specified level.

For [dielectronic recombination](../../../physics.md#dielectronic-recombination), write the entrance [ion](../../../chemistry.md#ion) as $X^{(z+1)+}$ in ground state $i$, and the intermediate state of $X^{z+}$ as $d=(j,n\ell)$. Capture excites the core from $i$ to $j$ while binding the incident [Electron](../../../physics.md#electron). The resonance energy relative to the entrance continuum is $\bar E=E_{ij}-I_{n\ell}>0$. The doubly excited state can eject the [Electron](../../../physics.md#electron) by [autoionization](../../../physics.md#autoionization), or undergo [radiative stabilization](../../../physics.md#radiative-stabilization) to a bound state.

Let $A^a_{di}$ be the partial [autoionization](../../../physics.md#autoionization) rate back to the entrance [ion](../../../chemistry.md#ion), $A_a$ the total [autoionization](../../../physics.md#autoionization) rate, $A_r$ the total radiative decay rate, and $A_s$ the rate of radiative decays that stabilize into bound levels. For an isolated narrow resonance, the Saha-Boltzmann equilibrium ratio has the bound-state energy replaced by the positive resonance energy:

$$
\frac{N_d^{\rm eq}}{N_eN_i}
=\frac{g_d}{2g_i}\left(\frac{h^2}{2\pi mkT}\right)^{3/2}e^{-\bar E/kT}.
$$

At equilibrium, inverse [dielectronic capture](../../../physics.md#dielectronic-capture) and [autoionization](../../../physics.md#autoionization) fluxes balance: $N_eN_iC_d=N_d^{\rm eq}A^a_{di}$. This establishes the capture coefficient even when the actual [plasma](../../../physics.md#plasma-physics) is not in local thermodynamic equilibrium. In the low-density, weak-radiation recombining [plasma](../../../physics.md#plasma-physics), the intermediate level instead has the stationary balance

$$
N_eN_iC_d=N_d(A_a+A_r).
$$

Multiplying its population by the successful stabilization rate gives the actual recombination coefficient

$$
\boxed{\alpha_d(d)=\frac{g_d}{2g_i}
\left(\frac{h^2}{2\pi mkT}\right)^{3/2}
e^{-\bar E/kT}\frac{A^a_{di}A_s}{A_a+A_r}.}
$$

Here the equilibrium population was used only to determine the capture rate by detailed balance; it was not assumed to equal the intermediate population when [photons](../../../quantum-mechanics.md#photon) escape. This is precisely why the competing decay probabilities appear.

Use the supplied core-transition relation between the [Einstein coefficients](../../../physics.md#einstein-coefficients) and [atomic oscillator strength](../../../physics.md#atomic-oscillator-strength),

$$
A_{ji}=\frac{\alpha^4c}{2a_0}\left(\frac{E_{ij}}{I_H}\right)^2\frac{g_i}{g_j}f_{ij},
\qquad \frac{h^2}{2\pi m}=4\pi a_0^2I_H.
$$

Here $\alpha$ is the [fine-structure constant](../../../perturbative-quantum-field-theory.md#fine-structure-constant) and $a_0$ the [Bohr radius](../../../physics.md#bohr-radius), not a recombination coefficient. Factor out $A_{ji}$ and define

$$
\boxed{\beta_{j,n\ell}=\frac{g_d}{2g_j}\,
\frac{A^a_{di}A_s}{A_{ji}(A_a+A_r)}.}
$$

Substitution yields

$$
\begin{aligned}
\alpha_d(j,n\ell)
&=4\pi^{3/2}\alpha^4a_0^2c\,
\frac{E_{ij}^2}{I_H^{1/2}(kT)^{3/2}}
e^{-\bar E/kT}f_{ij}\beta_{j,n\ell}\\
&=\boxed{4\pi^{3/2}\alpha^4a_0^2c
\left(\frac{E_{ij}}{I_H}\right)^{1/2}
\left(\frac{E_{ij}}{kT}\right)^{3/2}
e^{-\bar E/kT}f_{ij}\beta_{j,n\ell}.}
\end{aligned}
$$

This definition accommodates several entrance and decay channels. In the common spectator-electron approximation with one [autoionization](../../../physics.md#autoionization) channel and stabilization by the core transition, $A_s=A_r=A_{ji}$ and $A^a_{di}=A_a$. If all coupled substates of the captured $n\ell$ [Electron](../../../physics.md#electron) are summed, $g_d=2(2\ell+1)g_j$, giving

$$
\boxed{\beta_{j,n\ell}=(2\ell+1)\frac{A_a}{A_a+A_{ji}}.}
$$

For an intermediate state resolved by [fine structure](../../../physics.md#fine-structure), retain its actual $g_d$ instead of that summed weight. The stabilization probability itself is $A_s/(A_a+A_r)$; **the requested $\beta_{j,n\ell}$ is not just this branching probability, because the prefactor has already factored out the core radiative rate and [statistical weights of atomic levels](../../../physics.md#statistical-weight-of-an-atomic-level).** Radiative transitions to another still-autoionizing state require that state's eventual survival probability, rather than automatically counting every emitted [photon](../../../quantum-mechanics.md#photon) as stabilization.

The total [dielectronic recombination](../../../physics.md#dielectronic-recombination) coefficient sums all accessible positive-energy resonances. In this isolated-resonance approximation it has the form

$$
\alpha_d(T)=T^{-3/2}\sum_d c_d e^{-\bar E_d/kT},\qquad c_d\geq0,
$$

with atomic factors included in $c_d$. The [resonance-temperature dependence of dielectronic recombination](../../../physics.md#resonance-temperature-dependence-of-dielectronic-recombination) follows by differentiating a single term's logarithm:

$$
\frac{d}{dT}\log\alpha_d(d)=-\frac{3}{2T}+\frac{\bar E_d}{kT^2},
\qquad \boxed{kT_{\rm peak}=\frac23\bar E_d.}
$$

Thus low temperatures suppress a positive-energy resonance, although resonances very near threshold can still matter; at sufficiently high [temperature](../../../thermodynamics.md#temperature) a fixed set of resonances falls as $T^{-3/2}$. Several core-excitation series can produce several peaks. When [autoionization](../../../physics.md#autoionization) is much faster than radiation, the capture-and-survival product is limited by the stabilizing radiative rate; when capture is weak, [autoionization](../../../physics.md#autoionization) is the limiting inverse-capture rate. For a fixed Rydberg angular channel, [autoionization](../../../physics.md#autoionization) typically decreases at high principal quantum number while the core radiative rate changes little. Capture into very high levels is vulnerable to subsequent collisional or field ionization, so finite-density survival can suppress the total rate. **[dielectronic recombination](../../../physics.md#dielectronic-recombination) is resonant and strongly temperature-selective; its magnitude can be important in coronal ionization balance.**

## 3

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [solar corona](../../../stellar-astrophysics.md#solar-corona) is a hot, dilute [plasma](../../../physics.md#plasma-physics) in which [collisional ionization](../../../physics.md#collisional-ionization) mainly proceeds by direct [Electron](../../../physics.md#electron) impact and by [excitation-autoionization](../../../physics.md#excitation-autoionization). The principal inverse ion-changing processes are [radiative recombination](../../../physics.md#radiative-recombination) and [dielectronic recombination](../../../physics.md#dielectronic-recombination). [Three-body recombination](../../../physics.md#three-body-recombination) is negligible at ordinary coronal densities. Photoionization, stimulated recombination and charge exchange are normally secondary in this fully ionized, collision-dominated regime, although they should be reconsidered near irradiated or neutral interfaces.

For [collisional ionization equilibrium](../../../physics.md#collisional-ionization-equilibrium), the adjacent [ion](../../../chemistry.md#ion) stages satisfy

$$
N_eN_qC_q(T_e)=N_eN_{q+1}\alpha_{q+1}(T_e),
$$

together with conservation of the element's total abundance. Thus the low-density [ion](../../../chemistry.md#ion) fraction depends primarily on $T_e$. This fixes the amount of Si X available for line emission, but not the populations of its excited levels: a [coronal approximation](../../../physics.md#coronal-approximation) does not impose a Boltzmann level distribution.

Within an [ion](../../../chemistry.md#ion), [Electrons](../../../physics.md#electron) collisionally excite, de-excite and redistribute levels. Their [collision rate coefficient for an atomic transition](../../../physics.md#collision-rate-coefficient-for-an-atomic-transition) is

$$
q_{ij}(T_e)=\int_0^\infty\sigma_{ij}(v)v f_{T_e}(v)\,dv.
$$

The rate per [ion](../../../chemistry.md#ion) is $N_eq_{ij}$. Maxwellian detailed balance gives, for $E_j>E_i$,

$$
q_{ji}=\frac{g_i}{g_j}e^{(E_j-E_i)/kT_e}q_{ij}.
$$

Strong allowed transitions undergo rapid [spontaneous emission](../../../physics.md#spontaneous-emission); forbidden magnetic-dipole and electric-quadrupole transitions give much smaller decay rates and can leave a [metastable atomic level](../../../physics.md#metastable-atomic-level) appreciably populated. [Radiative cascades](../../../physics.md#radiative-cascade) feed levels from higher states. Absorption and stimulated emission add rates proportional to the local radiation field through the [Einstein coefficients](../../../physics.md#einstein-coefficients) when significant. Proton collisions can also mix closely separated levels separated by [fine structure](../../../physics.md#fine-structure) and should be included when their rates matter.

Write $f_i=N_i/N(\mathrm{Si\ X})$. A stationary [collisional-radiative model](../../../physics.md#collisional-radiative-model) solves

$$
\boxed{\sum_{j\ne i}f_jP_{ji}-f_i\sum_{j\ne i}P_{ij}=0,
\qquad\sum_i f_i=1,}
$$

where, in the simplest electron-plus-radiative model, $P_{ij}=N_eq_{ij}+A_{ij}$ with $A_{ij}=0$ for an upward transition. Add proton and radiation rates when appropriate. Include enough levels and radiative branches to capture population feeding. The thermal collision data, radiative probabilities and wavelengths then determine each line's [optically thin atomic line intensity](../../../astrophysics.md#optically-thin-atomic-line-intensity):

$$
\boxed{I_{ul}=\frac{h\nu_{ul}}{4\pi}\int N(\mathrm{Si\ X})f_u(N_e,T_e)A_{ul}\,ds.}
$$

The factor $4\pi$ distributes isotropic emission over [solid angle](../../../geometry-and-topology.md#solid-angle). [photon](../../../quantum-mechanics.md#photon) intensities omit $h\nu$. A practical source of the necessary atomic rates and population calculations is the [CHIANTI reference guide](https://www.chiantidatabase.org/cug.pdf).

Label the two ground-configuration levels $1,2$ and the two indicated excited levels $3,4$:

$$
\begin{aligned}
1&:2s^22p\,{}^2P_{1/2},&2&:2s^22p\,{}^2P_{3/2},\\
3&:2s2p^2\,{}^2D_{3/2},&4&:2s2p^2\,{}^2D_{5/2}.
\end{aligned}
$$

The common $1s^2$ core is omitted. Si X is silicon with nine [Electrons](../../../physics.md#electron) removed, hence five bound [Electrons](../../../physics.md#electron); the left superscript $2$ on $P$ or $D$ is the spin multiplicity, not another electron-occupancy exponent.

The observed lines correspond to decays $3\to1$ and $4\to2$. For approximately uniform [plasma](../../../physics.md#plasma-physics) at the indicated $T_e\simeq1.3\times10^6\,\mathrm K$, form the theoretical energy-intensity ratio

$$
\boxed{R(N_e)=\frac{I_{356}}{I_{347}}
=\frac{\nu_{42}A_{42}f_4(N_e,T_e)}{\nu_{31}A_{31}f_3(N_e,T_e)}.}
$$

The common abundance, Si X fraction and path length cancel, leaving a ratio governed by level populations. The frequency factor is $\nu_{42}/\nu_{31}=347/356$ for the rounded wavelengths. With observed [photon](../../../quantum-mechanics.md#photon) counts, first apply the detector calibration and use the corresponding photon-ratio convention.

The [electron-density diagnostic from metastable populations](../../../physics.md#electron-density-diagnostic-from-metastable-populations) can be seen in a reduced rate model. The upper ground level $2$ has only a weak radiative decay to $1$. Ignoring higher-level feeding for this explanation, their balance gives

$$
r:=\frac{N_2}{N_1}=\frac{N_eq_{12}}{A_{21}+N_eq_{21}}.
$$

At low density $r\simeq N_eq_{12}/A_{21}$; above the [critical density of an atomic transition](../../../physics.md#critical-density-of-an-atomic-transition) $A_{21}/q_{21}$ it approaches $q_{12}/q_{21}=(g_2/g_1)e^{-\Delta E_{21}/kT_e}$, approximately two when the gap due to [fine structure](../../../physics.md#fine-structure) is small compared with $kT_e$. This saturation can occur while the strong upper-level transitions still remain radiatively dominated.

Let $A_3,A_4$ be the total radiative loss rates of levels $3,4$, and $b_{31}=A_{31}/A_3$, $b_{42}=A_{42}/A_4$ their line branching fractions. In that upper-level low-density regime,

$$
N_3\simeq\frac{N_e(N_1q_{13}+N_2q_{23})}{A_3},\qquad
N_4\simeq\frac{N_e(N_1q_{14}+N_2q_{24})}{A_4}.
$$

Thus

$$
R\simeq K\frac{q_{14}+r q_{24}}{q_{13}+r q_{23}},\qquad
K=\frac{\nu_{42}b_{42}}{\nu_{31}b_{31}}.
$$

The two lines receive different relative feeding from the two ground levels, so their ratio changes as collisions populate the metastable level. More explicitly,

$$
\frac{dR}{dr}=K\frac{q_{24}q_{13}-q_{14}q_{23}}{(q_{13}+r q_{23})^2}.
$$

Different, nonproportional feeding coefficients give a usable density-sensitive interval. With $s=R/K$, this reduced model even permits explicit inversion:

$$
\boxed{r=\frac{s q_{13}-q_{14}}{q_{24}-s q_{23}},\qquad
N_e=\frac{A_{21}r}{q_{12}-r q_{21}}.}
$$

Physical solutions require positive density and a ratio within the allowed calibration range. The actual Si X calibration should use the full multilevel population system, not discard cross-excitation, cascades or all competing branches simply to use this illustrative formula.

Operationally, evaluate the model ratio at the known [temperature](../../../thermodynamics.md#temperature) over a density grid and match the calibrated observed ratio to it, propagating line-flux and atomic-data uncertainties. No observed ratio or numerical atomic rate set is supplied here, so the result is this inference procedure rather than a numerical density. At low- or high-density saturation, the ratio constrains density poorly. Deconvolve blends or sum every unresolved transition in the theoretical feature; for example, the neighboring $^2D_{3/2}\to{}^2P_{3/2}$ branch can contribute near the 356-Angstrom feature when unresolved. Atomic line identifications and that nearby branch are tabulated in [Del Zanna's coronal-spectroscopy thesis](https://www.damtp.cam.ac.uk/user/astro/gd232/research/thesis/gdz_phd_thesis.pdf).

For a nonuniform sightline, the ratio is instead

$$
R_{\rm obs}=\frac{\int j_{347}(s)R(N_e(s),T_e(s))\,ds}{\int j_{347}(s)\,ds}.
$$

A single-density inversion gives an [emission-weighted effective density from a line ratio](../../../physics.md#emission-weighted-effective-density-from-a-line-ratio), generally not the volume-average [electron number density](../../../statistical-physics.md#electron-number-density). **The density estimate is meaningful within its [temperature](../../../thermodynamics.md#temperature), optical-depth, line-blending and spatial-uniformity assumptions.** This is the precise interpretation of an average density obtained from the observed pair.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
