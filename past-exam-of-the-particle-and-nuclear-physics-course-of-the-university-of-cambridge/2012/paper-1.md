# Paper 1

↑ **Parent:** [2012](../2012.md)

[Original public PDF, physical pages 219–222; dated 31 May 2012](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1)

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
- [3](#3)
  - [Solution](#3/solution)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The static [one-pion exchange](../../nuclear-force.md#one-pion-exchange) [propagator](../../quantum-field-theory.md#propagator) gives a [Yukawa potential](../../electromagnetism.md#yukawa-potential) proportional to $e^{-m_\pi cr/\hbar}/r$. Its characteristic range is therefore the [Reduced Compton wavelength](../../mathematical-physics.md#reduced-compton-wavelength),

$$
\boxed{R\sim\frac{\hbar c}{m_\pi c^2}=\frac{197.3}{140}\,\mathrm{fm}\simeq1.4\,\mathrm{fm}}.
$$

This is an exponential falloff scale, not a sharp interaction cutoff. The ordinary [Compton wavelength](../../mathematical-physics.md#compton-wavelength) would introduce an unwanted factor $2\pi$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Neglect atomic [binding energy](../../energy.md#binding-energy) and take the target [electron](../../physics.md#electron) at rest. Use [natural units](../../mathematical-physics.md#natural-units) temporarily. The final state contains three [electrons](../../physics.md#electron) and one [Positron](../../physics.md#positron), so its threshold [invariant mass](../../special-relativity.md#invariant-mass) is $4m_e$. For incident total [energy](../../energy.md) $E$,

$$
s=(p_1+p_2)^2=2m_e^2+2m_eE=16m_e^2,
\qquad \boxed{E_{\rm th}=7m_ec^2=3.577\,\mathrm{MeV}\simeq3.58\,\mathrm{MeV}}.
$$

The corresponding incident [kinetic energy](../../energy.md#kinetic-energy) is $6m_ec^2=3.066\,\mathrm{MeV}$. At threshold the products have no relative [momentum](../../momentum.md) in the [centre-of-momentum frame](../../special-relativity.md#center-of-momentum-frame); their common laboratory motion requires more [energy](../../energy.md) than merely the pair's rest [energy](../../energy.md).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [nuclear quadrupole vibration](../../atomic-nucleus.md#nuclear-quadrupole-vibration) has five one-phonon magnetic substates, $m=-2,-1,0,1,2$. [Bose-Einstein statistics](../../quantum-ideal-gas-statistics.md#bose-einstein-statistics) restrict three identical [phonons](../../quantum-ideal-gas-statistics.md#phonon) to the [symmetric power](../../multilinear-algebra.md#symmetric-power) $S^3(V_2)$, of dimension $\binom{5+3-1}{3}=35$. Count occupation states $(n_{-2},\ldots,n_2)$ with $\sum n_m=3$ and $\sum mn_m=M$. For nonnegative $M$ the counts are

$$
\begin{array}{c|rrrrrrrr}M&0&1&2&3&4&5&6&7\\\hline d_M&5&4&4&3&2&1&1&0\end{array}.
$$

Each spin-$J$ [irreducible representation](../../representation-theory.md#irreducible-representation) contributes one state at every projection from $-J$ to $J$. [magnetic-substate subtraction](../../angular-momentum-operator.md#magnetic-substate-subtraction) therefore gives multiplicity $d_J-d_{J+1}$: one each at $J=0,2,3,4,6$, and none at $1,5$. Thus the [three-quadrupole-phonon multiplet](../../atomic-nucleus.md#three-quadrupole-phonon-multiplet) is

$$
\boxed{S^3(V_2)=V_0\oplus V_2\oplus V_3\oplus V_4\oplus V_6,\qquad J^P=0^+,2^+,3^+,4^+,6^+}.
$$

The dimension check is $1+5+7+9+13=35$. The [parity](../../quantum-mechanics.md#parity) is positive because each constituent [phonon](../../quantum-ideal-gas-statistics.md#phonon) has positive [parity](../../quantum-mechanics.md#parity). Pairwise angular-momentum triangle rules alone would include states incompatible with complete boson symmetrization.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A bare [gauge boson](../../relativistic-quantum-field.md#gauge-boson) mass would spoil the electroweak gauge structure. In the [Standard Model](../../standard-model.md) a complex [Higgs doublet](../../standard-model.md#higgs-field) instead has a symmetry-breaking potential. Choose the convention

$$
V=-\mu^2\Phi^\dagger\Phi+\lambda(\Phi^\dagger\Phi)^2,\qquad
\Phi=\frac1{\sqrt2}\binom{0}{v+h},\qquad v^2=\mu^2/\lambda.
$$

The [Higgs mechanism](../../standard-model.md#higgs-mechanism) rearranges three scalar components into the [longitudinal polarizations](../../wave-equation.md#longitudinal-polarization) of the massive [W bosons](../../standard-model.md#w-boson) and [Z bosons](../../standard-model.md#z-boson); the unbroken [electromagnetic gauge symmetry](../../relativistic-quantum-field.md#electromagnetic-gauge-symmetry) leaves the [photon](../../quantum-mechanics.md#photon) massless. One physical scalar excitation, the [Higgs boson](../../standard-model.md#higgs-boson) $h$, remains.[pp. 508–509, gauge-field mass generation in a symmetry-breaking scalar model](../../physics-bibliography.md#broken-symmetries-and-the-masses-of-gauge-bosons-by-peter-higgs) Using [tree-level Feynman diagrams](../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram),

$$
\boxed{m_W=gv/2,\quad m_Z=\sqrt{g^2+g'^2}\,v/2,\quad m_h^2=2\lambda v^2,\quad m_f=y_fv/\sqrt2}.
$$

These equations use [natural units](../../mathematical-physics.md#natural-units). [Yukawa interactions](../../standard-model.md#yukawa-interaction) generate charged-fermion masses and Higgs couplings proportional to those masses; the minimal model does not account for observed [neutrino masses](../../standard-model.md#neutrino-mass). The gauge kinetic term supplies Higgs couplings to W and Z pairs. The physical Higgs exchange also cancels the otherwise excessive high-energy growth of longitudinal vector-boson scattering. The mechanism does not fix the [Yukawa couplings](../../standard-model.md#yukawa-interaction) or the Higgs self-coupling, and most [proton](../../physics.md#proton) mass arises from strong-interaction dynamics rather than directly from the light-quark Higgs masses.

The mass-generation mechanism is a statement about the field and its [vacuum expectation value](../../quantum-field-theory.md#vacuum-expectation-value); the observable boson is the excitation about that vacuum.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[beta decay](../../physics.md#beta-decay) is a [weak charged current](../../standard-model.md#charged-current) process. At [quark](../../standard-model.md#quark) level $d\to uW^{-*}\to ue^-\bar\nu_e$, with amplitude proportional to $G_FV_{ud}$ at low [momentum transfer](../../quantum-scattering.md#momentum-transfer). A [neutron](../../neutron.md) in a [nucleus](../../atomic-nucleus.md) can thereby become a [proton](../../physics.md#proton):

$$
n\to pe^-\bar\nu_e,\qquad p\to ne^+\nu_e,\qquad pe^-\to n\nu_e.
$$

The second reaction denotes an energetically allowed nuclear conversion, not a decay of an isolated free [proton](../../physics.md#proton). In a nuclear beta transition the [mass number](../../chemical-substance.md#mass-number) stays fixed and the [atomic number](../../chemical-substance.md#atomic-number) changes by one. [baryon number](../../standard-model.md#baryon-number) and [electric charge](../../electric-charge.md) are conserved; the [neutrino](../../standard-model.md#neutrino) or [antineutrino](../../standard-model.md#antineutrino) supplies the missing [energy](../../energy.md), [momentum](../../momentum.md) and [angular momentum](../../momentum.md#angular-momentum). The three-body final state produces a continuous [electron](../../physics.md#electron) spectrum rather than a single [electron](../../physics.md#electron) [energy](../../energy.md). Neglecting [neutrino mass](../../standard-model.md#neutrino-mass) and recoil, an allowed spectrum in [electron](../../physics.md#electron) total [energy](../../energy.md) is

$$
\frac{d\Gamma}{dE_e}\propto F(Z,E_e)\,p_eE_e(E_0-E_e)^2
\left(g_V^2|M_F|^2+g_A^2|M_{GT}|^2\right).
$$

The [Fermi function](../../physics.md#fermi-function) accounts for the [electron](../../physics.md#electron)'s [Coulomb interaction](../../electrostatics.md#coulomb-interaction) with the daughter; $E_0$ is the [electron](../../physics.md#electron) total-energy endpoint. [forbidden beta decay](../../physics.md#forbidden-beta-decay) adds momentum-dependent nuclear shape factors. The [V-A interaction](../../standard-model.md#v-a-interaction) violates [parity](../../quantum-mechanics.md#parity): it couples left-chiral [fermion](../../tensor-product-of-quantum-systems.md#fermion) fields, not an equal mixture of left and right currents.

For [allowed beta decay](../../physics.md#allowed-beta-decay) the leading [leptons](../../standard-model.md#lepton) have zero [orbital angular momentum](../../quantum-mechanics.md#orbital-angular-momentum). [Fermi transitions](../../physics.md#fermi-transition) have $\Delta J=0$; [Gamow-Teller transitions](../../physics.md#gamow-teller-transition) have $\Delta J=0,1$ with $0\to0$ excluded. Both preserve nuclear [parity](../../quantum-mechanics.md#parity). Higher [lepton](../../standard-model.md#lepton) partial waves permit forbidden transitions with extra suppression. Nuclear matrix elements and [phase space](../../hamiltonian-mechanics.md#phase-space), as well as these [selection rules](../../atomic-physics.md#selection-rule), determine lifetimes. Particle-physics examples include free-neutron decay and [pion beta decay](../../physics.md#pion-beta-decay), $\pi^+\to\pi^0e^+\nu_e$. [semileptonic decays](../../physics.md#semileptonic-decay) test [quark](../../standard-model.md#quark) mixing and the universality of the [weak charged current](../../standard-model.md#charged-current). **[beta decay](../../physics.md#beta-decay) changes [quark flavour](../../standard-model.md#quark-flavor) through virtual W exchange; its continuous spectrum reflects an additional [lepton](../../standard-model.md#lepton) in the final state.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

[nuclear radius scaling](../../atomic-nucleus.md#nuclear-radius-scaling) follows approximately $R=r_0A^{1/3}$ with $r_0\simeq1.2\,\mathrm{fm}$ for a sharp matter-radius convention. Consequently the interior [nucleon](../../physics.md#nucleon) density is nearly independent of [mass number](../../chemical-substance.md#mass-number): [nuclear forces](../../nuclear-force.md) are short range and exhibit [nuclear matter saturation](../../nuclear-force.md#nuclear-matter-saturation). A diffuse [nuclear charge distribution](../../atomic-nucleus.md#nuclear-charge-distribution) has a charge-weighted [root mean square](../../analysis.md#root-mean-square) radius, not a hard surface. For a uniform sphere, $r_{\rm ch}=\sqrt{3/5}R$; charge radii and matter radii need not coincide, especially with [neutron](../../neutron.md) skins.

Elastic [electron scattering](../../physics.md#electron-scattering) measures the [nuclear charge form factor](../../atomic-nucleus.md#nuclear-charge-form-factor). In a simple one-photon, spherical approximation, with $q$ a wave number,

$$
F(q)=\frac{1}{Ze}\int\rho_{\rm ch}(\mathbf r)e^{i\mathbf q\cdot\mathbf r}\,d^3r,
\qquad F(q)=1-\frac{q^2\langle r^2\rangle}{6}+\cdots.
$$

The scattering [cross section](../../physics.md#cross-section-physics) relative to a point-charge prediction is proportional to $|F|^2$, so its low-$q$ slope constrains the radius and [diffraction](../../quantum-scattering.md#diffraction) structure constrains the radial distribution. Finite [momentum](../../momentum.md) coverage and [Coulomb distortion in electron scattering](../../quantum-scattering.md#coulomb-distortion-in-electron-scattering) limit reconstruction. In [Robert Hofstadter](../../physicist.md#robert-hofstadter)'s experiment a [magnetic spectrometer](../../optical-instrument.md#magnetic-spectrometer) separated elastic and inelastic [electron](../../physics.md#electron) peaks; beam-charge normalization and closed-slit background checks prevented raw count structure from being mistaken for a [nuclear charge form factor](../../atomic-nucleus.md#nuclear-charge-form-factor).[§III(b)(1), pp. 222–223; §IV(a), pp. 227–231](../../physics-bibliography.md#electron-scattering-and-nuclear-structure-by-robert-hofstadter)

A useful intrinsic-shape description is $R(\theta,\phi)=R_0[1+\sum_{\mu=-2}^{2}\alpha_{2\mu}Y_{2\mu}(\theta,\phi)+\cdots]$. An [intrinsic nuclear quadrupole moment](../../atomic-nucleus.md#intrinsic-nuclear-quadrupole-moment) $Q_0=\int\rho_{\rm ch}(3z^2-r^2)\,d^3r$ distinguishes prolate and oblate positive-charge distributions by positive and negative signs. The laboratory [spectroscopic nuclear quadrupole moment](../../atomic-nucleus.md#spectroscopic-nuclear-quadrupole-moment) is state dependent: an $I=0$ state has zero laboratory quadrupole moment even when its intrinsic shape is deformed. [nuclear rotational bands](../../atomic-nucleus.md#nuclear-rotational-band) approximately follow $E_I\propto I(I+1)$; harmonic [nuclear quadrupole vibrations](../../atomic-nucleus.md#nuclear-quadrupole-vibration) instead have equally spaced [phonon](../../quantum-ideal-gas-statistics.md#phonon) energies and multiphonon [spin](../../angular-momentum-operator.md#spin) multiplets. Measured [electric quadrupole transitions](../../quantum-mechanics.md#electric-quadrupole-transition) test the collective interpretation in addition to level energies. **Radius probes spatial extent; quadrupole observables and collective spectra probe shape.**

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [Feynman diagram](../../perturbative-quantum-field-theory.md#feynman-diagram) specifies a term in the perturbative [scattering amplitude](../../quantum-scattering.md#scattering-amplitude), not a measured microscopic trajectory. Assign external [spinors](../../algebra-over-a-field.md#spinor) or [polarization vectors](../../relativistic-quantum-field.md#polarization-vector), an interaction factor to each [Feynman vertex](../../perturbative-quantum-field-theory.md#interaction-vertex) and a [propagator](../../quantum-field-theory.md#propagator) to each internal line; impose [four-momentum](../../special-relativity.md#four-momentum) conservation and integrate over independent [loop momenta](../../perturbative-quantum-field-theory.md#loop-momentum). Sum amplitudes for indistinguishable alternatives, then square, sum final [spins](../../angular-momentum-operator.md#spin) and average unpolarized initial [spins](../../angular-momentum-operator.md#spin). A [decay rate](../../relativistic-quantum-field.md#decay-width) uses $d\Gamma=|\mathcal M|^2d\Phi_n/(2M)$ in [natural units](../../mathematical-physics.md#natural-units); a [cross section](../../physics.md#cross-section-physics) also divides by incident flux. [interference](../../physical-optics.md#interference-wave-propagation) means probabilities of individual diagrams must not simply be added.

The electromagnetic [fermion](../../tensor-product-of-quantum-systems.md#fermion) vertex is $f\bar f\gamma$, with coupling proportional to $eQ_f\gamma^\mu$; it preserves [fermion](../../tensor-product-of-quantum-systems.md#fermion) flavour. There is no elementary three-photon or four-photon vertex in [quantum electrodynamics](../../perturbative-quantum-field-theory.md#quantum-electrodynamics). The [weak charged current](../../standard-model.md#charged-current) has $W\ell\nu$ and $Wu_id_j$ vertices, with a left-chiral projector and a [Cabibbo-Kobayashi-Maskawa matrix](../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) element at the [quark](../../standard-model.md#quark) vertex. The [weak neutral current](../../standard-model.md#neutral-current) has $Zf\bar f$ vertices with vector and axial couplings; it includes [neutrinos](../../standard-model.md#neutrino) and is flavour diagonal at tree level. Electroweak gauge interactions also include $WW\gamma$, $WWZ$ and quartic $WWWW$, $WWZZ$, $WWZ\gamma$ and $WW\gamma\gamma$ vertices. Higgs-fermion and Higgs-vector interactions complete the mass-related scalar sector.[§10.1, Eqs. 10.2–10.7 and discussion of bosonic interactions](../../physics-bibliography.md#electroweak-model-and-constraints-on-new-physics-by-j-erler-and-a-freitas-2024)

[Quantum chromodynamics](../../standard-model.md#quantum-chromodynamics) has $q\bar qg$ vertices proportional to $g_s\gamma^\mu T^a$, plus three-gluon and four-gluon [Feynman vertices](../../perturbative-quantum-field-theory.md#interaction-vertex) because [gluons](../../standard-model.md#gluon) carry [color charge](../../standard-model.md#color-charge). A quark-gluon vertex preserves [quark flavour](../../standard-model.md#quark-flavor). Internal particles need not be on their [mass shells](../../special-relativity.md#mass-shell), but [electric charge](../../electric-charge.md) and [four-momentum](../../special-relativity.md#four-momentum) are conserved at each vertex. The figures below show representative leading flavour topologies; binding and [hadronization](../../standard-model.md#hadronization) are implicit, and additional strong-interaction contributions can modify hadronic amplitudes.

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [weak charged current](../../standard-model.md#charged-current) spectator topology is $c\to qW^{+*}$, $W^{+*}\to u\bar q'$, with the initial $\bar u$ a spectator. The pair $q\bar u$ forms the negative [meson](../../physics.md#meson) and $u\bar q'$ the positive [meson](../../physics.md#meson). The amplitude contains $V_{cq}^*V_{uq'}$ in one common charged-current convention; complex conjugating all factors changes no rate classification. With $c_C=\cos\theta_C$ and $s_C=\sin\theta_C$, the CKM magnitudes are

$$
\begin{array}{c|c|c}
\text{mode}&(q,q')&\text{amplitude order}\\\hline
\pi^+K^-&(s,d)&c_C^2\\
\pi^+\pi^-&(d,d)&s_Cc_C\\
K^+K^-&(s,s)&s_Cc_C\\
K^+\pi^-&(d,s)&s_C^2
\end{array}.
$$

Thus **$\pi^+K^-$ is favoured, both equal-flavour pairs are singly Cabibbo suppressed, and $K^+\pi^-$ is doubly suppressed**. The corresponding parametric rate hierarchy is $1:\tan^2\theta_C:\tan^4\theta_C$ after normalizing to the favoured mode. [Cabibbo suppression](../../standard-model.md#cabibbo-suppression) counting alone does not rank the middle two: [phase space](../../hamiltonian-mechanics.md#phase-space), different matrix elements and [hadronic final-state interactions](../../standard-model.md#hadronic-final-state-interaction) matter. With identical constant matrix elements, the larger [pion](../../standard-model.md#pion) [phase space](../../hamiltonian-mechanics.md#phase-space) would favour $\pi^+\pi^-$, whereas experimentally $K^+K^-$ is faster. The empirical decreasing order is

$$
\boxed{\Gamma(\pi^+K^-) > \Gamma(K^+K^-) > \Gamma(\pi^+\pi^-) > \Gamma(K^+\pi^-)}.
$$

As a later cross-check, [HFLAV](../../physics.md#hflav)'s 2024 averages give approximately $4.00\%$, $0.411\%$, $0.149\%$ and $0.0138\%$ respectively. The exact middle ordering is an experimental input, not a consequence of the supplied masses and [Cabibbo angle](../../standard-model.md#cabibbo-angle) alone.[final branching-fraction average table and final doubly suppressed-mode estimate](../../physics-bibliography.md#d0-hadronic-branching-fractions-and-final-state-radiation-by-hflav-2024)

<a id="3/a/image-charm-spectator-topology"></a>
![](../../past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2012/paper-1-charm-topology.png)

**[Figure 1](#3/a/image-charm-spectator-topology). Charm spectator topology**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The initial [strangeness](../../standard-model.md#strangeness) is $-2$. The $\Lambda\pi^0$ final state has [strangeness](../../standard-model.md#strangeness) $-1$, so its allowed nonleptonic amplitude is weak. One representative topology is $s\to uW^{-*}$ followed by $W^{-*}\to d\bar u$; spectator $u,s$ combine with the produced $d$ into the $\Lambda$, while $u\bar u$ contributes to the neutral [pion](../../standard-model.md#pion). The available rest [energy](../../energy.md) is $1314.8-1115.7-135.0=64.1\,\mathrm{MeV}$.

The $\Lambda\bar K^0$ state would conserve [strangeness](../../standard-model.md#strangeness) and could have a strong vertex, but its threshold exceeds the parent mass by $1115.7+497.6-1314.8=298.5\,\mathrm{MeV}$. **It is kinematically forbidden.** Coupling strength cannot rescue a closed decay channel.

The radiative channel also changes [strangeness](../../standard-model.md#strangeness). It is a [weak radiative hyperon decay](../../standard-model.md#weak-radiative-hyperon-decay), not an ordinary electromagnetic decay between states of the same flavour. A representative two-quark contribution is W exchange $su\to ud$ with a [photon](../../quantum-mechanics.md#photon) attached to a charged line; the other allowed attachments, hadronic intermediate states and short-distance loop contributions must be included for a complete amplitude. Its extra electromagnetic coupling and hadronic dynamics suppress it relative to the nonleptonic channel. Consequently

$$
\boxed{\Gamma(\Lambda\pi^0)\gg\Gamma(\Lambda\gamma)>\Gamma(\Lambda\bar K^0)=0}.
$$

[NA48 Collaboration](../../physics.md#na48-collaboration) measured a radiative [branching fraction](../../relativistic-quantum-field.md#branching-fraction) of about $1.16\times10^{-3}$, corroborating the suppression rather than a purely electromagnetic interpretation.[abstract and branching-fraction result, 2004](../../physics-bibliography.md#measurement-of-the-xi0-to-lambda-gamma-decay-asymmetry-and-branching-fraction-by-na48-collaboration)

<a id="3/b/image-hyperon-and-radiative-meson-topologies"></a>
![](../../past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2012/paper-1-hyperon-and-rho.png)

**[Figure 2](#3/b/image-hyperon-and-radiative-meson-topologies). Hyperon and radiative meson topologies**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the neutral quark-antiquark [mesons](../../physics.md#meson) here, $C=(-1)^{L+S}$. Thus $C(\eta')=C(\pi^0)=+1$, while $C(\rho^0)=C(\gamma)=-1$. The radiative $\rho^0\gamma$ mode conserves [charge conjugation](../../quantum-field-theory.md#charge-conjugation) and admits a quark-line photon-emission diagram. Both components of the supplied $\rho^0$ [wavefunction](../../wave-function.md) contribute: the charge-weighted flavour overlap is proportional to $Q_u-Q_d=1$, so it does not cancel. Its [photon](../../quantum-mechanics.md#photon) [energy](../../energy.md) is $(m_{\eta'}^2-m_\rho^2)/(2m_{\eta'})\simeq165\,\mathrm{MeV}$.

The $\pi^0\gamma$ mode changes [charge conjugation](../../quantum-field-theory.md#charge-conjugation) and, more decisively, a spin-zero particle cannot decay into another spin-zero particle and one real [photon](../../quantum-mechanics.md#photon). In the parent rest frame the [photon](../../quantum-mechanics.md#photon) has [helicity](../../special-relativity.md#helicity) $\pm1$, while the opposite-moving [pion](../../standard-model.md#pion) has [helicity](../../special-relativity.md#helicity) zero; the [spin-zero two-body helicity selection](../../standard-model.md#spin-zero-two-body-helicity-selection) rule cannot be satisfied. **Its on-shell two-body amplitude vanishes even if a [weak interaction](../../standard-model.md#weak-interaction) violates C.** A virtual [photon](../../quantum-mechanics.md#photon) subsequently making another pair is a different final state.

For $\pi^0\rho^0$, angular-momentum conservation requires relative [orbital angular momentum](../../quantum-mechanics.md#orbital-angular-momentum) $L=1$. Its [parity](../../quantum-mechanics.md#parity) is then negative, matching the parent, but its charge-conjugation eigenvalue is $C_\pi C_\rho=-1$: the two distinct self-conjugate particles are not interchanged by C, so there is no additional $(-1)^L$ factor in this C eigenvalue. The decay is forbidden by strong and electromagnetic charge-conjugation conservation despite being above threshold. A weak contribution would require [CP violation](../../quantum-field-theory.md#cp-violation) as well. At the strong/electromagnetic accuracy of the diagram classification,

$$
\boxed{\Gamma(\rho^0\gamma)>\Gamma(\pi^0\rho^0)=\Gamma(\pi^0\gamma)=0}.
$$

If extremely small weak CP-violating amplitudes are retained, $\pi^0\rho^0$ need not be exactly zero; the one-real-photon [spin](../../angular-momentum-operator.md#spin) prohibition remains exact for $\pi^0\gamma$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For [electron-positron annihilation into a muon pair](../../perturbative-quantum-field-theory.md#electron-positron-annihilation-into-a-muon-pair) the gauge diagrams are s-channel [photon](../../quantum-mechanics.md#photon) and Z exchange. For [electron-positron annihilation into electron neutrinos](../../relativistic-quantum-field.md#electron-positron-annihilation-into-electron-neutrinos) there is s-channel Z exchange and t-channel W exchange, with [interference](../../physical-optics.md#interference-wave-propagation). For [electron-positron annihilation into W-boson pairs](../../relativistic-quantum-field.md#electron-positron-annihilation-into-w-boson-pairs) there are s-channel [photon](../../quantum-mechanics.md#photon) and Z diagrams and a t-channel electron-neutrino diagram. All three gauge amplitudes are required for the proper high-energy cancellation. Electron-Yukawa-suppressed s-channel Higgs diagrams can also produce the massive [muon](../../standard-model.md#muon) or W pair; they vanish in the usual zero-electron-mass approximation used for the leading gauge comparison.

<a id="3/d/image-lepton-and-w-pair-gauge-diagrams"></a>
![](../../past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2012/paper-1-lepton-topologies.png)

**[Figure 3](#3/d/image-lepton-and-w-pair-gauge-diagrams). Lepton and W-pair gauge diagrams**.

There is **no energy-independent ordering**. For unpolarized beams and inclusive Born [cross sections](../../physics.md#cross-section-physics) the useful regimes are:

- Below the [muon](../../standard-model.md#muon) threshold only the [neutrino](../../standard-model.md#neutrino) channel is open, ignoring its tiny mass threshold. Immediately above $2m_\mu$, [muon](../../standard-model.md#muon) [phase space](../../hamiltonian-mechanics.md#phase-space) initially vanishes.
- Well above $2m_\mu$ but well below the weak-boson masses, [photon](../../quantum-mechanics.md#photon) exchange gives $\sigma_{\mu\mu}\simeq4\pi\alpha^2/(3s)$, whereas $\sigma_{\nu_e\bar\nu_e}=O(G_F^2s)$. Hence the [muon](../../standard-model.md#muon) channel dominates and real W-pair production is closed.
- Near the Z pole, W pairs are still closed and the Z resonance dominates both open channels. The ratio is approximately $\Gamma(Z\to\nu_e\bar\nu_e)/\Gamma(Z\to\mu^+\mu^-)\simeq2$, from their neutral-current couplings: [neutrinos](../../standard-model.md#neutrino) rank above [muons](../../standard-model.md#muon). This is for one [neutrino](../../standard-model.md#neutrino) flavour.
- At $\sqrt s=2m_W\simeq160.806\,\mathrm{GeV}$ the on-shell W-pair channel opens from zero [phase space](../../hamiltonian-mechanics.md#phase-space). Its position in the ordering changes across threshold and must be obtained from the summed amplitudes, rather than inferred solely from a weak/electromagnetic label.
- Far above the weak masses, forward t-channel W exchange makes the inclusive electron-neutrino [cross section](../../physics.md#cross-section-physics) approach a nonzero scale of order $g^4/m_W^2$. The W-pair [cross section](../../physics.md#cross-section-physics) behaves as $O[g^4\log(s/m_W^2)/s]$ and the [muon](../../standard-model.md#muon) [cross section](../../physics.md#cross-section-physics) as $O(g^4/s)$. Thus asymptotically the decreasing order is $\nu_e\bar\nu_e$, then $W^+W^-$, then $\mu^+\mu^-$. Fixed angular cuts, [beam spin polarization](../../angular-momentum-operator.md#beam-spin-polarization) and radiative corrections modify these comparisons.

The Z-pole ratio follows $[\tfrac12]^2/[(-\tfrac12+\sin^2\theta_W)^2+\sin^4\theta_W]\simeq1.99$. Treating every weak reaction as uniformly slower misses both the resonance and forward exchange.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For projectile velocity $v$ and a resting target, let $M=m_x+m_X$, $\mu=m_xm_X/M$, and $V=m_xv/M$. Subtract the [kinetic energy](../../energy.md#kinetic-energy) of the centre of mass from the laboratory [kinetic energy](../../energy.md#kinetic-energy):

$$
T^*=\tfrac12m_xv^2-\tfrac12MV^2
=T_x\frac{m_X}{M}=\boxed{\frac{\mu}{m_x}T_x}.
$$

In the [centre-of-momentum frame](../../special-relativity.md#center-of-momentum-frame) the two momenta are opposite with equal magnitude, so

$$
T^*=\frac{p^{*2}}{2m_x}+\frac{p^{*2}}{2m_X}=\frac{p^{*2}}{2\mu},
\qquad\boxed{p^*=\sqrt{2\mu T^*}}.
$$

For masses quoted in $\mathrm{MeV}/c^2$, use $p^*c=\sqrt{2(\mu c^2)T^*}$. These are the nonrelativistic relations stipulated for this question; no relativistic correction should be silently mixed into the numerical results.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [partial decay width](../../relativistic-quantum-field.md#partial-decay-width) $\Gamma_x$ is the [energy](../../energy.md) width associated with decay of the [compound nucleus](../../physics.md#compound-nucleus) back into the entrance channel $x+X$; by [time reversal](../../quantum-field-theory.md#t-symmetry) it also controls formation from that channel. The [partial decay width](../../relativistic-quantum-field.md#partial-decay-width) $\Gamma_y$ describes the selected exit channel $y+Y$. The total [decay width](../../relativistic-quantum-field.md#decay-width) sums all energetically accessible channels, including these: $\boxed{\Gamma=\sum_i\Gamma_i=\hbar/\tau}$. The [branching fraction](../../relativistic-quantum-field.md#branching-fraction) for channel $i$ is $\Gamma_i/\Gamma$. Widths have [energy](../../energy.md) units, whereas $\Gamma_i/\hbar$ is a decay probability per unit time. The isolated-resonance formula assumes approximately constant widths over the resonance and neglects a nonresonant interfering background.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

An unstable isolated level has survival amplitude $a(t)=\theta(t)e^{-iE_0t/\hbar}e^{-\Gamma t/(2\hbar)}$, because its [survival probability](../../markov-chain.md#survival-probability) falls as $e^{-\Gamma t/\hbar}$. Its energy-domain amplitude is proportional to

$$
\int_0^\infty e^{i(E-E_0)t/\hbar}e^{-\Gamma t/(2\hbar)}dt
=\frac{\hbar}{\Gamma/2-i(E-E_0)}.
$$

Taking the modulus squared gives the denominator of the [Breit-Wigner resonance cross section](../../quantum-scattering.md#breit-wigner-resonance-cross-section)

$$
\boxed{(E-E_0)^2+(\Gamma/2)^2}.
$$

At $E-E_0=\pm\Gamma/2$ the resonant factor is half its peak, so $\Gamma$ is the [full width at half maximum](../../analysis.md#full-width-at-half-maximum). [exponential decay](../../analysis.md#exponential-decay) is the isolated-level approximation; energy-dependent thresholds or overlapping levels need a more general lineshape.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Unpolarized projectile and target [spins](../../angular-momentum-operator.md#spin) supply $(2J_x+1)(2J_X+1)$ equally weighted [spin](../../angular-momentum-operator.md#spin) orientations. An isolated compound-nucleus level of [spin](../../angular-momentum-operator.md#spin) $J$ has $2J+1$ degenerate magnetic substates. Sum over these resonance substates and average over the entrance [spins](../../angular-momentum-operator.md#spin) to obtain

$$
\boxed{g=\frac{2J+1}{(2J_x+1)(2J_X+1)}}.
$$

This [resonance spin statistical factor](../../quantum-scattering.md#resonance-spin-statistical-factor) is a statistical [spin](../../angular-momentum-operator.md#spin) weight, not always a probability smaller than one: [orbital angular momentum](../../quantum-mechanics.md#orbital-angular-momentum) also participates in forming the resonance. The partial-wave resonance [cross section](../../physics.md#cross-section-physics) carries the corresponding angular-momentum multiplicity. Polarized beams or unresolved overlapping [spin](../../angular-momentum-operator.md#spin) channels require a different average or a sum over channels.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Using the supplied masses,

$$
\mu_\alpha c^2=\frac{3728.34(11177.76)}{14906.10}=2795.801\,\mathrm{MeV},
\quad T_\alpha^*=10.10\frac{11177.76}{14906.10}=7.573770\,\mathrm{MeV}.
$$

Therefore $\boxed{p_\alpha^*=205.790\,\mathrm{MeV}/c\simeq206\,\mathrm{MeV}/c}$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For [resonance channel threshold conversion](../../physics.md#resonance-channel-threshold-conversion), equate the compound-state [energy](../../energy.md) measured from the two different channel thresholds. The proton-plus-nitrogen threshold exceeds the alpha-plus-carbon threshold by

$$
\Delta=(938.26+13973.30-3728.34-11177.76)\,\mathrm{MeV}=5.46\,\mathrm{MeV}.
$$

Thus $T_p^*=T_\alpha^*-\Delta=2.113770\,\mathrm{MeV}$ and

$$
\boxed{T_{p,\mathrm{lab}}=T_p^*\frac{938.26+13973.30}{13973.30}=2.25570\,\mathrm{MeV}\simeq2.26\,\mathrm{MeV}}.
$$

The positive centre-of-momentum [energy](../../energy.md) verifies that the [proton](../../physics.md#proton) channel is open. These numbers use the stipulated nonrelativistic kinematics and rounded nuclear masses.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The gamma width is $0.10\,\mathrm{eV}=10^{-7}\,\mathrm{MeV}$, so the remaining [proton](../../physics.md#proton) width is $\Gamma_p=0.20-0.15-10^{-7}=0.0499999\,\mathrm{MeV}$. At the peak of the same resonance the total-width denominator and gamma exit width cancel. [alpha particles](../../atomic-nucleus.md#alpha-particle) and [carbon-12](../../chemical-substance.md#carbon-12) have [spin](../../angular-momentum-operator.md#spin) zero; the [proton](../../physics.md#proton) and the stated nitrogen level each have [spin](../../angular-momentum-operator.md#spin) $1/2$. Hence $g_\alpha/g_p=4$, independently of the unspecified resonance [spin](../../angular-momentum-operator.md#spin). The [proton](../../physics.md#proton) [reduced mass](../../classical-mechanics.md#reduced-mass) and [momentum](../../momentum.md) are

$$
\mu_pc^2=879.223\,\mathrm{MeV},\qquad p_p^*c=\sqrt{2(879.223)(2.113770)}=60.967\,\mathrm{MeV}.
$$

The [same-resonance entrance-channel cross-section ratio](../../quantum-scattering.md#same-resonance-entrance-channel-cross-section-ratio) is therefore

$$
\boxed{\frac{\sigma_\alpha}{\sigma_p}
=\frac{g_\alpha}{g_p}\frac{p_p^{*2}}{p_\alpha^{*2}}\frac{\Gamma_\alpha}{\Gamma_p}
=4\frac{60.967^2}{205.790^2}\frac{0.15}{0.0499999}\simeq1.053}.
$$

The ratio compares each reaction at its own laboratory resonance [energy](../../energy.md). Factors of $\hbar^2$ restoring the [cross section](../../physics.md#cross-section-physics)'s area units cancel. Only the supplied nitrogen [spin](../../angular-momentum-operator.md#spin) magnitude is used: its printed positive [parity](../../quantum-mechanics.md#parity) is immaterial to this [spin](../../angular-momentum-operator.md#spin) average, so no orbital-parity inference is made from that assignment.

## ↑ Ancestors (11)

1. [2012](../2012.md)
2. [Past exam of the particle and nuclear physics course of the University of Cambridge](../../past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge.md)
3. [Particle and Nuclear Physics course of the University of Cambridge](../../university-of-cambridge.md#particle-and-nuclear-physics-course-of-the-university-of-cambridge)
4. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
