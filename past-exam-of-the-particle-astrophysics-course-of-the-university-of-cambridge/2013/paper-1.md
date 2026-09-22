# Paper 1

↑ **Parent:** [2013](../2013.md)

[Original public PDF, physical pages 583–585; dated 26 April 2013](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For an isolated approximately spherical [mass](../../classical-mechanics.md#mass) distribution outside its luminous extent, retain the gravitational [force](../../force.md) $GMm/r^2$ and use the specified low-acceleration inertial law. [circular motion](../../classical-mechanics.md#circular-motion) then gives

$$
\frac{GMm}{r^2}=\frac m{a_0}\left(\frac{v^2}{r}\right)^2,
\qquad\boxed{v^4=GMa_0}.
$$

The [radius](../../topology.md#radius) cancels when enclosed luminous [mass](../../classical-mechanics.md#mass) is effectively constant. This is the asymptotic [modified Newtonian dynamics](../../einstein-field-equations.md#modified-newtonian-dynamics) result associated with the [baryonic Tully-Fisher relation](../../galaxy.md#baryonic-tully-fisher-relation); an arbitrary extended disk cannot everywhere be replaced exactly by a point [mass](../../classical-mechanics.md#mass).

At the disk edge,

$$
a(R)=\frac{(9\times10^4)^2}{3\times10^{20}}
=\boxed{2.7\times10^{-11}\,\mathrm{m\,s^{-2}}=0.27a_0}.
$$

Using $G=6.67\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$ gives

$$
M_{\rm MOND}=\frac{v^4}{Ga_0}=9.84\times10^{39}\,\mathrm{kg}
=\boxed{4.9\times10^9M_\odot}.
$$

This is an order-of-magnitude isolated, low-acceleration estimate. The edge [acceleration](../../classical-mechanics.md#acceleration) is below $a_0$, but not extremely small compared with it; a full interpolation law, disk geometry and an external gravitational field can affect a more precise [mass](../../classical-mechanics.md#mass) fit.

For the [spherical mass profile for a flat rotation curve](../../galaxy.md#spherical-mass-profile-for-a-flat-rotation-curve), assume spherical symmetry where the halo dominates. A [flat rotation curve](../../galaxy.md#flat-galaxy-rotation-curve) gives $M(<r)=v^2r/G$, and differentiating $M(<r)=4\pi\int_0^r\rho(s)s^2\,ds$ yields

$$
\boxed{\rho(r)=\frac{v^2}{4\pi Gr^2}}.
$$

Here $\rho$ is the density of the spherical gravitating model; it is not an exact deprojection of a thin luminous disk or a proof that the central density must diverge. At the outermost stated measured [radius](../../topology.md#radius),

$$
M(<2R)=\frac{v^2(2R)}G=7.29\times10^{40}\,\mathrm{kg}
=\boxed{3.6\times10^{10}M_\odot}.
$$

This gives the requested galaxy-plus-halo [mass](../../classical-mechanics.md#mass) estimate if the model is truncated at the outermost observed [radius](../../topology.md#radius) $2R$. **The observation itself constrains enclosed [mass](../../classical-mechanics.md#mass) within $2R$**; any additional outer halo remains unconstrained. Extending $\rho\propto r^{-2}$ to infinity would give divergent [mass](../../classical-mechanics.md#mass). Subtracting the MOND-inferred luminous [mass](../../classical-mechanics.md#mass) to obtain a Newtonian halo [mass](../../classical-mechanics.md#mass) would mix independent model-dependent estimates without an independently measured luminous [mass](../../classical-mechanics.md#mass).

In the [Bullet Cluster](../../large-scale-structure-of-the-universe.md#bullet-cluster) collision, most observed baryonic [mass](../../classical-mechanics.md#mass) is hot gas. [ram pressure](../../fluid-mechanics.md#ram-pressure) slows and [shocks](../../transport-equation.md#shock-wave) the gas, while the galaxies pass through much more freely. [weak gravitational lensing](../../gravitational-lensing.md#weak-gravitational-lensing) maps the projected gravitational [mass](../../classical-mechanics.md#mass) without requiring that the gas be in [hydrostatic equilibrium](../../statistical-physics.md#hydrostatic-equilibrium). The dominant lensing peaks lie closer to the galaxies than to the displaced X-ray gas. This supports a dominant weakly collisional [dark matter](../../cosmology.md#dark-matter) component under the usual gravity model. It is stronger evidence than a mass-to-light discrepancy alone because distinct components separate during the same encounter. The inference needs background-source shape/redshift [calibration](../../differential-geometry.md#calibration-differential-geometry), projection control and uncertainty in the lensing reconstruction; it does not identify a [WIMP](../../cosmology.md#weakly-interacting-massive-particle) species or by itself exclude every modified-gravity theory.[Abstract and comparison of lensing mass, optical galaxies and X-ray gas](../../physics-bibliography.md#a-direct-empirical-proof-of-the-existence-of-dark-matter-by-douglas-clowe-and-others)

<a id="1/image-original-conceptual-merger-sketch-showing-galaxies-and-dominant-lensing-mass-displaced-from-slowed-x-ray-gas-illustrative-positions-not-observational-data"></a>
![](../../past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2013/paper-1-bullet-components.png)

**[Figure 1](#1/image-original-conceptual-merger-sketch-showing-galaxies-and-dominant-lensing-mass-displaced-from-slowed-x-ray-gas-illustrative-positions-not-observational-data). Original conceptual merger sketch showing galaxies and dominant lensing mass displaced from slowed X-ray gas; illustrative positions, not observational data**.

For [dark-matter direct detection](../../cosmology.md#dark-matter-direct-detection), consider [XENON100](../../particle-detection.md#xenon100) at Gran Sasso. A halo [WIMP](../../cosmology.md#weakly-interacting-massive-particle) can undergo [elastic scattering](../../quantum-scattering.md#elastic-scattering) from a [xenon](../../chemical-substance.md#xenon) [atomic nucleus](../../atomic-nucleus.md), leaving a recoil of only a few to tens of keV. The expected rate is very low, so a large target, low threshold and long exposure must be combined with background rejection. The [nuclear-recoil kinematics of WIMP scattering](../../atomic-nucleus.md#nuclear-recoil-kinematics-of-wimp-scattering) gives $E_{R,\max}=2\mu_{\chi N}^2v^2/m_N$ in the nonrelativistic limit, where $\mu_{\chi N}$ is the [reduced mass](../../classical-mechanics.md#reduced-mass) and [masses](../../classical-mechanics.md#mass) and [velocities](../../classical-mechanics.md#velocity) use consistent units. This explains why low-energy response [calibration](../../differential-geometry.md#calibration-differential-geometry) matters.

The dual-phase [xenon](../../chemical-substance.md#xenon) detector measures prompt [particle scintillation](../../physics.md#scintillation-physics) S1 and delayed [electroluminescence](../../optics.md#electroluminescence) S2 from [ionization](../../atomic-physics.md#ionization) electrons extracted into gas. Their time separation gives interaction depth; the S2 light pattern supplies transverse position. An inner [fiducial volume](../../particle-detection.md#fiducial-volume) uses [xenon](../../chemical-substance.md#xenon)'s self-shielding to suppress external backgrounds. The S2/S1 distribution statistically separates [nuclear recoils](../../atomic-nucleus.md#nuclear-recoil) from [electron recoils](../../particle-detection.md#electron-recoil); it is not perfect event-by-event identification. Underground siting reduces cosmic-ray backgrounds, while passive shielding, low-radioactivity components, [xenon](../../chemical-substance.md#xenon) purification and a surrounding [active detector veto](../../particle-detection.md#active-detector-veto) reduce other events.[Sections 2–3, two-phase detection, detector design and background control](../../physics-bibliography.md#the-xenon100-dark-matter-experiment-by-the-xenon100-collaboration)

Neutrons can also make [nuclear recoils](../../atomic-nucleus.md#nuclear-recoil), so charge-to-light discrimination alone cannot eliminate them. Multiple-scatter rejection, shielding and background modelling remain necessary. Gamma-source and neutron-source [calibrations](../../differential-geometry.md#calibration-differential-geometry) map electron- and nuclear-recoil distributions, [energy](../../energy.md) scale and selection acceptance. Position-dependent light collection and charge losses need correction; photon-counting fluctuations and uncertain low-energy yields limit threshold sensitivity. Blind event selection and independent sidebands guard against tuning cuts to apparent candidates. The 224.6-live-day, 34 kg search found two benchmark candidates against about one expected background event, consistent with background. Its interaction limit therefore depends on the assumed halo distribution, [WIMP](../../cosmology.md#weakly-interacting-massive-particle) [mass](../../classical-mechanics.md#mass) and nuclear response; it is not a detection or an exclusion of all [dark matter](../../cosmology.md#dark-matter).[Printed pp. 2–4, calibrations, blind selection and backgrounds; abstract for exposure and result](../../physics-bibliography.md#dark-matter-results-from-225-live-days-of-xenon100-data-by-the-xenon100-collaboration)

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [grand unified theory](../../classical-field-theory.md#grand-unified-theory) embeds the strong and electroweak [gauge groups](../../relativistic-quantum-field.md#gauge-group) in a larger group, for example $SU(3)_c\times SU(2)_L\times U(1)_Y\subset SU(5)$. [quarks](../../standard-model.md#quark) and [leptons](../../standard-model.md#lepton) can belong to common representations, while heavy extra gauge or scalar [bosons](../../tensor-product-of-quantum-systems.md#boson) connect them. The resulting interactions can violate [baryon number](../../standard-model.md#baryon-number), unlike ordinary perturbative Standard Model reactions. Running gauge couplings and proton-decay searches test such ideas; unification is a theoretical possibility, not an established observation.[Abstract, early-universe baryon-number-violating reactions in unified theories; later erratum noted in source record](../../physics-bibliography.md#unified-gauge-theories-and-the-baryon-number-of-the-universe-by-motohiko-yoshimura)

[baryogenesis](../../cosmology.md#baryogenesis) must explain why a nearly matter-antimatter-symmetric early state evolves into a surviving [baryon asymmetry](../../cosmology.md#baryon-asymmetry). In the usual local CPT-invariant framework, the [Sakharov conditions](../../cosmology.md#sakharov-conditions) require baryon-number violation, C and [CP violation](../../quantum-field-theory.md#cp-violation), and departure from [thermal equilibrium](../../thermal-equilibrium.md). [baryon](../../physics.md#baryon) conservation would forbid creating a net excess; exact conjugation symmetries would pair baryon-producing processes with equal antibaryon production; equilibrium with no imposed asymmetry would erase a source term through [detailed balance](../../markov-chain.md#detailed-balance).

For heavy particles $X$ and $\bar X$, let decay channels carry different [baryon numbers](../../standard-model.md#baryon-number). CP-violating interference can make their [branching fractions](../../relativistic-quantum-field.md#branching-fraction) differ, even though [CPT symmetry](../../quantum-field-theory.md#cpt-symmetry) requires equal total widths. Defining the mean [baryon number](../../standard-model.md#baryon-number) produced per decay as $\epsilon$, an out-of-equilibrium abundance can generate $n_B/s$ of order $\epsilon$ times its initial number per [entropy](../../entropy.md), reduced by inefficient production and washout. A rough condition is that decays become effective after inverse production has ceased, with the relevant reaction rate compared with the [Hubble parameter](../../cosmology.md#hubble-parameter). Complex couplings alone do not guarantee a nonzero rate asymmetry: a relative [absorptive phase](../../relativistic-quantum-field.md#absorptive-phase-of-a-decay-amplitude) is also needed.

Survival matters as much as production. Electroweak [sphalerons](../../standard-model.md#sphaleron) violate $B+L$ while conserving [baryon-minus-lepton number](../../standard-model.md#baryon-minus-lepton-number) $B-L$, so a minimal GUT-generated asymmetry with $B-L=0$ can be washed out if [sphalerons](../../standard-model.md#sphaleron) and the other relevant reactions equilibrate. Generating nonzero $B-L$, as in suitable heavy-Majorana-neutrino [leptogenesis](../../cosmology.md#leptogenesis), can avoid this problem. **A viable GUT [baryogenesis](../../cosmology.md#baryogenesis) model must generate an asymmetry and demonstrate that subsequent reactions do not erase it.** The [Sakharov conditions](../../cosmology.md#sakharov-conditions) are necessary ingredients under these assumptions, not a numerical prediction of the observed abundance.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[supersymmetry](../../supersymmetry.md) pairs bosonic and fermionic degrees of freedom; broken [supersymmetry](../../supersymmetry.md) permits partners heavier than known particles. At the [Large Hadron Collider](../../particle-accelerator.md#large-hadron-collider), strong production of [squarks](../../supersymmetry.md#squark) and [gluinos](../../supersymmetry.md#gluino) is an important channel. If [R-parity](../../supersymmetry.md#r-parity) is conserved, partners are produced in pairs and their cascades end in a stable [lightest supersymmetric particle](../../supersymmetry.md#lightest-supersymmetric-particle). A neutral weakly interacting [lightest supersymmetric particle](../../supersymmetry.md#lightest-supersymmetric-particle) escapes, giving [missing transverse momentum](../../particle-detection.md#missing-transverse-momentum) together with jets and possibly [leptons](../../standard-model.md#lepton). Conservation is tested transversely because the initial [parton](../../standard-model.md#parton) longitudinal momenta are unknown.

The experimental observable is

$$
\boldsymbol p_T^{\rm miss}=-\sum_{\rm reconstructed}\boldsymbol p_T.
$$

[neutrinos](../../standard-model.md#neutrino) produce genuine [missing transverse momentum](../../particle-detection.md#missing-transverse-momentum), and [calorimeter](../../calorimetry.md#calorimeter) mismeasurement or detector defects can imitate it. Searches use jet multiplicity, transverse momenta, missing [momentum](../../momentum.md), angular separation cuts and a [collider effective mass](../../particle-detection.md#collider-effective-mass) such as $m_{\rm eff}=p_T^{\rm miss}+\sum p_T^{\rm jet}$. Isolated-lepton selections explore complementary cascades. Trigger efficiency, jet [energy](../../energy.md) scale, [collision pileup](../../particle-detection.md#collision-pileup) and event cleaning affect acceptance.

A credible search estimates backgrounds from [particle-physics control regions](../../particle-detection.md#particle-physics-control-region) before inspecting the [signal region](../../particle-detection.md#signal-region). Invisible $Z\to\nu\bar\nu$ plus jets can be constrained using photon-plus-jets or visible $Z\to\ell^+\ell^-$ samples with [control-region transfer factors](../../particle-detection.md#control-region-transfer-factor). Lepton-enriched samples constrain $W$ and top backgrounds with lost [leptons](../../standard-model.md#lepton); multijet samples constrain fake missing [momentum](../../momentum.md). A joint [likelihood](../../maximum-likelihood-estimation.md#likelihood-function) includes these observations and [nuisance parameters](../../statistical-model.md#nuisance-parameter) for [systematic uncertainties](../../physics.md#systematic-uncertainty). Agreement with background gives upper bounds on signal rate and conditional [mass](../../classical-mechanics.md#mass) exclusions. The pre-examination ATLAS 7 TeV analysis is a concrete example of this strategy and reported no significant excess.[Sections III, IX and XI, control-region likelihood and background estimates; abstract for the null result](../../physics-bibliography.md#search-for-squarks-and-gluinos-with-the-atlas-detector-in-final-states-with-jets-and-missing-transverse-momentum-using-4-7-fb-1-of-sqrt-s-7-tev-proton-proton-collision-data-by-atlas-collaboration)

Electroweak production motivates multilepton searches; compressed spectra can give soft visible decay products and require special selections such as recoil against [initial-state radiation](../../particle-detection.md#initial-state-radiation). [R-parity](../../supersymmetry.md#r-parity) violation can instead remove the stable missing-particle signature, requiring other searches. **An exclusion always depends on [masses](../../classical-mechanics.md#mass), [branching fractions](../../relativistic-quantum-field.md#branching-fraction), production rates and decay assumptions; a null jets-plus-missing-momentum result does not exclude [supersymmetry](../../supersymmetry.md) as a whole.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A [gravitational wave](../../gravitational-wave.md) produces a time-dependent tidal distortion. For a normally incident plus-polarized wave in the long-wavelength limit, two perpendicular freely suspended arms change by $\delta L_x/L=h_+/2$ and $\delta L_y/L=-h_+/2$. Their differential length is therefore

$$
\boxed{\Delta L=Lh_+},\qquad
\delta\Phi=\frac{4\pi\Delta L}{\lambda}
$$

for a simple round-trip [Michelson interferometer](../../physical-optics.md#michelson-interferometer). [LIGO](../../physics.md#ligo) uses kilometre-scale orthogonal arms with [optical cavities](../../optical-instrument.md#optical-cavity) that enhance the phase response, a stabilized [laser](../../laser.md) and suspended mirrors in [vacuum](../../physics.md#vacuum). As an illustrative scale, $h=10^{-21}$ across a 4 km arm corresponds to differential length $4\times10^{-18}\,\mathrm m$. The measured quantity is returning light phase, not mirror displacement against a rigid external ruler. Optical storage and control loops give a frequency-dependent calibrated response.

Seismic and terrestrial disturbances dominate low [frequencies](../../wave.md#frequency), thermal motion of suspensions and mirror coatings contributes at intermediate [frequencies](../../wave.md#frequency), and [photon](../../quantum-mechanics.md#photon) [shot noise](../../electrical-engineering.md#shot-noise) limits high-frequency readout. Isolation and suspension systems reduce ground coupling; low-loss materials reduce [thermal noise](../../electrical-engineering.md#thermal-noise); [vacuum](../../physics.md#vacuum) suppresses gas scattering and [forces](../../force.md). Greater optical [power](../../energy.md#power) reduces [shot noise](../../electrical-engineering.md#shot-noise) but increases radiation-pressure fluctuations and thermal demands. Stable optical alignment and feedback are essential, yet their own sensor and actuator noise must be controlled. These are engineering requirements because the desired [strain](../../continuum-mechanics.md#strain) is extraordinarily small.[Instrument configuration and detector-noise discussion; primary initial-LIGO account](../../physics-bibliography.md#ligo-the-laser-interferometer-gravitational-wave-observatory-by-b-p-abbott-and-others)

A candidate should appear coherently at separated observatories with consistent propagation delay and antenna response. Auxiliary environmental monitors, [calibration](../../differential-geometry.md#calibration-differential-geometry) injections and time-shifted coincidence backgrounds test instrumental explanations. Matched filtering is powerful for modelled compact-binary chirps; coherent burst searches allow less predictable signals. Binary-pulsar orbital [energy](../../energy.md) loss already provided indirect evidence for [gravitational radiation](../../gravitational-wave.md) before 2013, but it is distinct from directly measuring passing waves.[Binary-pulsar orbital-decay test of relativistic gravity](../../physics-bibliography.md#binary-pulsars-and-relativistic-gravity-by-joseph-hooton-taylor-jr) At the examination date, direct detection remained a search objective. **Reliable detection requires both sufficient [strain](../../continuum-mechanics.md#strain) sensitivity and a demonstrated astrophysical signal rather than correlated or accidental noise.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [cosmic microwave background](../../cosmic-microwave-background.md) is relic thermal [radiation](../../physics.md#radiation) from the hot early universe. Its [temperature](../../temperature.md) anisotropy is expanded in [spherical harmonics](../../analysis.md#spherical-harmonic), with angular [power](../../energy.md#power) spectrum $C_\ell^{TT}$. [Thomson scattering](../../cosmic-microwave-background-anisotropy.md#thomson-scattering) of a local [radiation quadrupole](../../astrophysics.md#radiation-quadrupole) generates [linear polarization](../../electromagnetic-wave.md#linear-polarization) around last scattering and again during [reionization](../../cosmic-microwave-background.md#reionization). Polarization maps are decomposed into [E-mode polarization](../../cosmic-microwave-background-anisotropy.md#e-mode-polarization) and [B-mode polarization](../../cosmic-microwave-background-anisotropy.md#b-mode-polarization), giving spectra such as $EE$, $TE$ and $BB$ in addition to [temperature](../../temperature.md) information.

[Cosmic microwave background acoustic peak](../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-acoustic-peak) positions compare the [sound horizon](../../cosmic-microwave-background-anisotropy.md#sound-horizon) with the angular-diameter distance to last scattering, constraining geometry and expansion history. Relative peak heights constrain [baryon](../../physics.md#baryon) loading and [matter-radiation equality](../../cosmology.md#matter-radiation-equality); the damping tail constrains diffusion and other early-universe physics. The [scalar spectral index](../../cosmic-inflation.md#scalar-spectral-index) and [primordial scalar amplitude](../../cosmic-inflation.md#primordial-scalar-amplitude) constrain inflationary perturbations. Coherent acoustic structure and temperature-polarization correlations support predominantly adiabatic initial perturbations. Large-angle [E-mode polarization](../../cosmic-microwave-background-anisotropy.md#e-mode-polarization) measures the [reionization](../../cosmic-microwave-background.md#reionization) [optical depth](../../astrophysics.md#optical-depth), helping break its degeneracy with the scalar amplitude inferred from small-scale [temperature](../../temperature.md) anisotropy.

Under a specified cosmological model, these data constrain ordinary and [cold dark matter](../../cosmology.md#cold-dark-matter) densities, the [Hubble constant](../../cosmology.md#hubble-constant), spatial curvature and cosmic age. Complementary distance information helps break the geometrical degeneracy: [temperature](../../temperature.md) peaks alone do not uniquely establish a [cosmological constant](../../cosmology.md#cosmological-constant). The Planck 2013 parameter analysis used Planck [temperature](../../temperature.md) data and, in important combinations, [WMAP](../../cosmic-microwave-background.md#wilkinson-microwave-anisotropy-probe) low-multipole polarization; it should not be described as a full Planck polarization release.[Abstract and data-combination definitions, including WMAP polarization](../../physics-bibliography.md#planck-2013-results-xvi-cosmological-parameters-by-planck-collaboration)

Linear [scalar cosmological perturbations](../../linear-cosmological-perturbation-theory.md#scalar-cosmological-perturbation) generate [E-mode polarization](../../cosmic-microwave-background-anisotropy.md#e-mode-polarization) but no primordial [B-mode polarization](../../cosmic-microwave-background-anisotropy.md#b-mode-polarization) in the simplest treatment. [tensor cosmological perturbations](../../linear-cosmological-perturbation-theory.md#tensor-cosmological-perturbation) can generate [B-mode polarization](../../cosmic-microwave-background-anisotropy.md#b-mode-polarization), making them a possible probe of inflationary [gravitational waves](../../gravitational-wave.md). [gravitational lensing](../../gravitational-lensing.md) converts some E-mode [power](../../energy.md#power) into [B-mode polarization](../../cosmic-microwave-background-anisotropy.md#b-mode-polarization), however, and Galactic dust and [synchrotron radiation](../../electromagnetic-radiation.md#synchrotron-radiation) also contribute polarized foregrounds. Multifrequency observations, foreground modelling, beam [calibration](../../differential-geometry.md#calibration-differential-geometry) and control of [temperature-to-polarization leakage](../../cosmic-microwave-background-anisotropy.md#temperature-to-polarization-leakage) are therefore necessary. Polarization does not by itself establish a primordial tensor signal. **[temperature](../../temperature.md) and polarization jointly test the expansion history and primordial perturbations, while complementary data and foreground control determine how uniquely parameters can be inferred.**

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a homogeneous canonical [scalar field](../../classical-field-theory.md#scalar-field), $\rho_\phi=\dot\phi^2/2+V$ and $P_\phi=\dot\phi^2/2-V$. Potential-energy domination gives $P_\phi\simeq-\rho_\phi$, accelerated expansion and a decreasing [comoving Hubble radius](../../cosmology.md#comoving-hubble-radius). [Hubble friction](../../cosmology.md#hubble-friction) can permit slow roll down a sufficiently flat potential. Enough inflation stretches an initially small causally connected region to encompass our observable universe, suppresses the relative spatial-curvature term and dilutes unwanted massive relics. [quantum fluctuations](../../quantum-theory.md#quantum-fluctuation) supply possible seeds for cosmological structure; a successful model must also end inflation and create the hot post-inflationary universe. These statements do not imply that arbitrary initial conditions inevitably inflate.

Use the stated reduced-Planck units throughout the field calculation. Differentiating the Friedmann constraint and substituting the field equation gives

$$
2H\dot H=\frac13\dot\phi(\ddot\phi+m^2\phi)
=-H\dot\phi^2,\qquad
\boxed{\dot H=-\frac12\dot\phi^2}.
$$

Division assumes the nontrivial expanding branch $H>0$; the [vacuum](../../physics.md#vacuum) endpoint follows continuously.

During rapid [oscillations](../../wave.md#oscillation), require $m\gg H$ and $|\dot A|\ll mA$. To leading order, $\dot\phi\simeq-mA\sin mt$, while the Friedmann constraint gives $H_m^2\simeq m^2A^2/6$. Thus

$$
\dot H\simeq-\frac{m^2A^2}{2}\sin^2mt
=-\frac32H_m^2(1-\cos2mt).
$$

Averaging over many [oscillations](../../wave.md#oscillation) on a timescale still short compared with $H^{-1}$ gives

$$
\boxed{\dot H_m=-\frac32H_m^2}.
$$

The [quadratic-inflaton Hubble oscillations](../../cosmic-inflation.md#quadratic-inflaton-hubble-oscillations) obey, to leading order in $H_m/m$,

$$
H_{\rm fluct}\simeq\frac{3H_m^2}{4m}\sin2mt,
\qquad \frac{|H_{\rm fluct}|}{H_m}=O(H_m/m)\ll1.
$$

Differentiating this expression reproduces the cosine term, with smaller corrections from the slowly varying amplitude. Instantaneously $H$ remains nonincreasing because its exact [derivative](../../calculus.md#derivative) is $-\dot\phi^2/2$; an oscillatory correction does not mean oscillatory growth of the total [Hubble parameter](../../cosmology.md#hubble-parameter).

The mean equation integrates to

$$
\frac1{H_m(t)}=\frac1{H_m(t_i)}+\frac32(t-t_i),\qquad
\boxed{H_m(t)=\frac{2}{3(t-t_*)}},\qquad
\boxed{a(t)\propto(t-t_*)^{2/3}}.
$$

The shift $t_*$ is set by matching to the earlier evolution, not necessarily the Big Bang origin of the full solution. Averaged kinetic and [potential energies](../../energy.md#potential-energy) are equal, so $\langle P_\phi\rangle\simeq0$, $\langle\rho_\phi\rangle\propto a^{-3}$ and $A\propto a^{-3/2}$. **The coherent quadratic [oscillations](../../wave.md#oscillation) behave as [pressureless matter](../../cosmology.md#pressureless-matter), not [radiation](../../physics.md#radiation)**, even though they are a [scalar field](../../classical-field-theory.md#scalar-field) rather than a gas of cold particles. [radiation](../../physics.md#radiation) would instead give $a\propto t^{1/2}$. The averaged approximation is controlled only after [oscillations](../../wave.md#oscillation) are fast compared with expansion.

<a id="3/image-original-dimensionless-scalar-field-integration-showing-a-decaying-oscillation-envelope-and-a-nonincreasing-hubble-parameter-with-a-matter-like-average"></a>
![](../../past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2013/paper-1-inflaton-oscillations.png)

**[Figure 2](#3/image-original-dimensionless-scalar-field-integration-showing-a-decaying-oscillation-envelope-and-a-nonincreasing-hubble-parameter-with-a-matter-like-average). Original dimensionless scalar-field integration showing a decaying oscillation envelope and a nonincreasing Hubble parameter with a matter-like average**.

[reheating](../../cosmic-inflation.md#reheating) requires interactions beyond the isolated field equations above. The oscillating [inflaton](../../cosmic-inflation.md#inflaton) can decay into other particles, whose scattering and further decays establish a thermal bath. The [perturbative inflaton reheating equations](../../cosmic-inflation.md#perturbative-inflaton-reheating-equations) are

$$
\dot\rho_\phi+3H\rho_\phi=-\Gamma\rho_\phi,\qquad
\dot\rho_r+4H\rho_r=\Gamma\rho_\phi.
$$

Expansion redshifts the components differently; transfer becomes efficient around $H\sim\Gamma$, and [radiation](../../physics.md#radiation) domination follows when the transferred relativistic [energy](../../energy.md) dominates. For suitable couplings, nonperturbative [preheating](../../cosmic-inflation.md#preheating) by [parametric resonance](../../singular-perturbation.md#parametric-resonance) can precede thermalization, with backreaction and rescattering affecting its completion. Neither the decay rate nor thermalization is specified by $m$ and $V$ alone. Instantaneous [reheating](../../cosmic-inflation.md#reheating) idealizes all this as immediate conversion of the end-of-inflation [energy](../../energy.md) to [radiation](../../physics.md#radiation).[Abstract and Introduction: perturbative decay, resonant preheating, backreaction and thermalization](../../physics-bibliography.md#towards-the-theory-of-reheating-after-inflation-by-lev-kofman-and-others)

For [instantaneous-reheating horizon matching](../../cosmic-inflation.md#instantaneous-reheating-horizon-matching), specify the comparison: take the initial patch to be of order $H_i^{-1}$, compare the same-shaped inflationary history with approximately fixed $H_i/H_{\rm end}$, and assume instantaneous [reheating](../../cosmic-inflation.md#reheating) followed by [adiabatic expansion](../../first-law-of-thermodynamics.md#adiabatic-expansion). Ignoring changes in relativistic degrees of freedom, $a_0/a_{\rm reh}\propto T_{\rm reh}$, while [energy](../../energy.md) conservation and the [Friedmann equation](../../cosmology.md#friedmann-equations) give $H_{\rm end}\propto T_{\rm reh}^2$. The present size of this inflated patch therefore scales as

$$
\ell_0\sim H_i^{-1}e^N\frac{a_0}{a_{\rm reh}}
\propto\frac{e^N}{T_{\rm reh}}.
$$

At fixed present [Hubble radius](../../cosmology.md#hubble-radius), **a higher instantaneous [reheating](../../cosmic-inflation.md#reheating) scale requires more e-folds** in this standard comparison, approximately $\Delta N\simeq\ln(T_2/T_1)$, up to slow scale and entropy-degree corrections. Hotter [reheating](../../cosmic-inflation.md#reheating) gives more subsequent expansion, but the associated initial Hubble patch is smaller by a stronger [power](../../energy.md#power) of [temperature](../../temperature.md). If instead one artificially holds the initial physical patch or $H_i$ fixed while varying the end [energy](../../energy.md) independently, the post-inflationary geometric effect alone would give the opposite trend. [temperature](../../temperature.md) without an inflation-scale comparison convention does not fix that alternative problem; this is why the matching assumptions must be stated.[Section II, equations 2, 6–8: horizon-scale matching and its dependence on inflation and reheating energy scales](../../physics-bibliography.md#how-long-before-the-end-of-inflation-were-observable-perturbations-produced-by-andrew-r-liddle-and-samuel-m-leach)

## ↑ Ancestors (11)

1. [2013](../2013.md)
2. [Past exam of the particle Astrophysics course of the University of Cambridge](../../past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge.md)
3. [Particle Astrophysics course of the University of Cambridge](../../university-of-cambridge.md#particle-astrophysics-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
