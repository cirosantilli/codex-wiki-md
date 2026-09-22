<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Particle candidate.** A stable, electrically neutral [weakly interacting massive particle](../../../../weakly-interacting-massive-particle.md) can become nonrelativistic before [cosmological particle freeze-out](../../../../cosmological-particle-freeze-out.md). Its [annihilation](../../../../annihilation.md) rate per particle $\Gamma=n\langle\sigma v\rangle$ eventually falls below the [Hubble parameter](../../../../hubble-parameter.md); the surviving comoving number then remains approximately fixed. A weak-scale [annihilation](../../../../annihilation.md) [cross section](../../../../cross-section-physics.md) can give a cosmologically significant [thermal relic](../../../../thermal-relic.md). This is a mechanism and a parameter-scale motivation, not a guarantee that every weakly interacting particle has the right abundance.

[supersymmetry](../../../../supersymmetry-split.md) supplies [neutralinos](../../../../neutralino.md), mixtures of neutral electroweak [gauginos](../../../../gaugino.md) and [higgsinos](../../../../higgsino.md). If a [neutralino](../../../../neutralino.md) is the [lightest supersymmetric particle](../../../../lightest-supersymmetric-particle.md) and [R-parity](../../../../r-parity.md) is conserved, it cannot decay solely into [Standard Model](../../../../standard-model-split.md) particles and is stable. Its [electroweak interactions](../../../../electroweak-interaction.md) can make it a [WIMP](../../../../weakly-interacting-massive-particle.md). Conservation of [R-parity](../../../../r-parity.md) and a neutral lightest state are additional assumptions; [R-parity violation](../../../../r-parity-violation.md), [coannihilation](../../../../coannihilation.md), composition and resonant [annihilation](../../../../annihilation.md) can substantially change the conclusion.

**An underground test.** [XENON100](../../../../xenon100.md) at Gran Sasso used a liquid-xenon target in a two-phase [time projection chamber](../../../../time-projection-chamber.md). A [WIMP](../../../../weakly-interacting-massive-particle.md) scattering elastically from a [xenon](../../../../xenon.md) nucleus could produce a low-energy [nuclear recoil](../../../../nuclear-recoil.md). The interaction makes prompt [particle scintillation](../../../../scintillation-physics.md), S1, and [ionization](../../../../ionization.md) electrons. An [electric field](../../../../electric-field-split.md) drifts the electrons upward; their extraction into [xenon](../../../../xenon.md) gas produces delayed [electroluminescence](../../../../electroluminescence.md), S2. The delay measures depth, while the S2 light pattern determines the transverse position. An inner [fiducial volume](../../../../fiducial-volume.md) suppresses surface backgrounds through [xenon](../../../../xenon.md) self-shielding; underground overburden reduces cosmic-ray [muons](../../../../muon.md), and shielding and material selection reduce [radioactivity](../../../../radioactive-decay.md).[Detector design, signal formation and background-rejection principles](../../../../the-xenon100-dark-matter-experiment-by-the-xenon100-collaboration.md)

The S2/S1 ratio separates most [electron recoils](../../../../electron-recoil.md) from [nuclear recoils](../../../../nuclear-recoil.md). Gamma-source [calibration](../../../../calibration-differential-geometry.md) maps the electron-recoil leakage; an americium–beryllium [neutron](../../../../neutron-split.md) source calibrates nuclear-recoil response and cut acceptance. Purity and position corrections must be measured, and selection fixed before unblinding the search region. [neutrons](../../../../neutron-split.md) can themselves produce single [nuclear recoils](../../../../nuclear-recoil.md), so discrimination is not perfect; material assays and transport simulations constrain this background. In the 224.6-live-day, 34-kg analysis, two candidate events were compatible with the expected $1.0\pm0.2$ background events. The result constrained scattering [cross sections](../../../../cross-section-physics.md) rather than establishing a discovery.[Pages 2–4, calibration, blinded selection, neutron background and candidate counts](../../../../dark-matter-results-from-225-live-days-of-xenon100-data-by-the-xenon100-collaboration.md)

A predicted count also depends on the local [dark matter halo](../../../../dark-matter-halo.md) density, distribution of [velocities](../../../../velocity.md), recoil threshold and nuclear response. Thus a null result constrains a particle model under stated astrophysical assumptions; it does not exclude all [dark matter](../../../../dark-matter.md). A collider missing-momentum signal would likewise need independent evidence for a cosmological lifetime.

<a id="2/image-original-functional-schematic-of-prompt-light-and-delayed-charge-readout-in-a-two-phase-xenon-detector"></a>
![](../../../../past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2015/paper-1-xenon-signals.png)

**[Figure 2](#2/image-original-functional-schematic-of-prompt-light-and-delayed-charge-readout-in-a-two-phase-xenon-detector). Original functional schematic of prompt light and delayed charge readout in a two-phase xenon detector**.

**Relic [energy density](../../../../energy-density.md) in the stipulated freeze-out approximation.** Let $M=mc^2=1900\ \mathrm{GeV}$ and $\theta=k_BT$. Writing the given distribution in [energy](../../../../energy-split.md) units gives

$$
n_f=6\left(\frac{M\theta_f}{(\hbar c)^2}\right)^{3/2}e^{-P},
\qquad
\theta_f=\frac{M}{P}=52.78\ \mathrm{GeV}.
$$

By [sharp-freeze-out relic dilution](../../../../sharp-freeze-out-relic-dilution.md), after [cosmological particle freeze-out](../../../../cosmological-particle-freeze-out.md) conserve [particle number](../../../../particle-number.md), $n a^3=\mathrm{constant}$. In the approximation $aT=\mathrm{constant}$ for the background bath,

$$
n_0=n_f\left(\frac{\theta_0}{\theta_f}\right)^3
=6P^{3/2}e^{-P}\left(\frac{\theta_0}{\hbar c}\right)^3.
$$

Inserting the printed inputs yields

$$
n_f=5.5242\times10^{39}\ \mathrm{m^{-3}},\qquad
n_0=4.8766\times10^{-4}\ \mathrm{m^{-3}},
$$

and hence

$$
\boxed{\rho_0c^2=M n_0=0.927\ \mathrm{GeV\,m^{-3}},
\qquad\Omega_\chi=\frac{0.927}{5}=0.185.}
$$

This is approximately $93\%$ of the stipulated dark-matter [energy density](../../../../energy-density.md), $0.2\times5=1\ \mathrm{GeV\,m^{-3}}$, so the toy calculation gives the right order and is close to the target. At fixed $P$ the cancellation of $M$ in $n_0$ is exact for the given prefactor, while the present [energy density](../../../../energy-density.md) remains proportional to $M$.

The equilibrium exponential must be evaluated at freeze-out, **not at today's [temperature](../../../../temperature-split.md)**: equilibrium no longer maintains the [particle number](../../../../particle-number.md) afterward. More accurately, [comoving entropy conservation](../../../../comoving-entropy-conservation.md) gives $a^3g_{*s}T^3=\mathrm{constant}$ and multiplies the displayed $n_0$ by $g_{*s,0}/g_{*s,f}$, when both counts use the same bath-temperature convention. Thus $0.185$ is the constant-$g_{*s}$ estimate supported by the supplied toy model. A refined abundance would require additional [entropy degrees of freedom](../../../../entropy-degrees-of-freedom.md) and [annihilation](../../../../annihilation.md) history: realistic [entropy](../../../../entropy-split.md) release, gradual freeze-out and the model's [annihilation](../../../../annihilation.md) channels matter.

<a id="2/image-original-calculation-of-the-relic-density-sensitivity-to-freeze-out-parameter-with-the-printed-mass-and-constant-entropy-degrees-approximation"></a>
![](../../../../past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2015/paper-1-relic-sensitivity.png)

**[Figure 3](#2/image-original-calculation-of-the-relic-density-sensitivity-to-freeze-out-parameter-with-the-printed-mass-and-constant-entropy-degrees-approximation). Original calculation of the relic-density sensitivity to freeze-out parameter, with the printed mass and constant-entropy-degrees approximation**.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the particle Astrophysics course of the University of Cambridge](../../../split.md)
5. [Particle Astrophysics course of the University of Cambridge](../../../../particle-astrophysics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
