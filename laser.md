# Laser

↑ **Parent:** [Optics](optics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laser)

A laser generates amplified [light](optics.md#light) through [stimulated emission](#stimulated-emission). Its name abbreviates “light amplification by stimulated emission of radiation”. Lasers supply the intense beams used in [optical tweezers](optics.md#optical-tweezers); [optical coherence](physical-optics.md#optical-coherence) also makes them useful for [wave interference](physical-optics.md#interference-wave-propagation) measurements. [OpenStax University Physics 3, §8.6: lasers](https://openstax.org/books/university-physics-volume-3/pages/8-6-lasers).

In the usual material picture, a gain medium stores [energy](energy.md) supplied by pumping, for example by incident [light](optics.md#light) or an [electric current](electric-charge.md#electric-current). [Stimulated emission](#stimulated-emission) transfers that stored [energy](energy.md) to a selected optical [normal mode](wave-equation.md#normal-mode), while competing [photon absorption](quantum-mechanics.md#photon-absorption) removes [light](optics.md#light). Producing net [optical gain](#optical-gain) requires a suitable population distribution, such as [population inversion](#population-inversion) in the simple model below.

A familiar [laser](laser.md) oscillator uses mirrors to return [light](optics.md#light) through the gain medium. This optical feedback favours resonant [normal modes](wave-equation.md#normal-mode); a partly transmitting mirror lets useful [power](energy.md#power) escape. Feedback and mode selection have different implementations, including ring arrangements: every [laser](laser.md) need not resemble the same two-mirror device. The [laser threshold](#laser-threshold) example treats just that device. [Shaoul Ezekiel, MIT, Laser fundamentals I: Simple laser, transcript](https://ocw.mit.edu/courses/res-6-006-video-demonstrations-in-lasers-and-optics-spring-2008/37b4c2aa5a6e3e0c119688024ce90ce5_Iqp7NxnwaGY.pdf) [Franz Kärtner, MIT 6.974, Chapter 7, §7.1: laser oscillator concept](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/18f30fad63a62ef4dd894d3752b55a60_chapter7.pdf).

The useful combination is concentrated [power](energy.md#power) and controlled optical [normal modes](wave-equation.md#normal-mode). It gives [optical tweezers](optics.md#optical-tweezers) a localized source of [force](force.md) and [wave interference](physical-optics.md#interference-wave-propagation) measurements a source with useful [optical coherence](physical-optics.md#optical-coherence). A [laser](laser.md) can nevertheless emit several [frequencies](wave.md#frequency); “laser” alone does not guarantee a single [frequency](wave.md#frequency). [Shaoul Ezekiel, MIT, Laser fundamentals I: Spectrum of laser light, transcript](https://ocw.mit.edu/courses/res-6-006-video-demonstrations-in-lasers-and-optics-spring-2008/674c0c322cf0d87072e31de3e51f8e27_--Zi_cn4kPE.pdf).

An original experimental landmark is T. H. Maiman's 1960 report of stimulated optical radiation from optically pumped ruby at about $694.3\,\mathrm{nm}$. His paper describes both the pumping path and the observed emission, connecting stored material [energy](energy.md) with amplified [light](optics.md#light). [T. H. Maiman, Stimulated Optical Radiation in Ruby, Nature 187, 493–494, 1960, original paper](physics-bibliography.md#stimulated-optical-radiation-in-ruby-by-theodore-harold-maiman).

**Table of contents**

- [Vertical-cavity surface-emitting laser](#vertical-cavity-surface-emitting-laser)
- [Excimer laser](#excimer-laser)
- [Laser ablation](#laser-ablation)
- [Semiconductor laser](#semiconductor-laser)
  - [Laser diode](#laser-diode)
- [Dye laser](#dye-laser)
- [Three-level laser](#three-level-laser)
  - [Three-level ground-state inversion threshold](#three-level-ground-state-inversion-threshold)
  - [Ruby laser](#ruby-laser)
    - [Maiman ruby laser experiment](#maiman-ruby-laser-experiment)
  - [Three-level laser rate equation](#three-level-laser-rate-equation)
    - [Laser gain clamping](#laser-gain-clamping)
    - [Stored excitation in a pulsed laser](#stored-excitation-in-a-pulsed-laser)
- [Laser detuning](#laser-detuning)
- [Stimulated emission](#stimulated-emission)
  - [Photon occupation enhancement of emission](#photon-occupation-enhancement-of-emission)
  - [Population inversion](#population-inversion)
    - [Lower-level depopulation in a four-level laser](#lower-level-depopulation-in-a-four-level-laser)
- [Optical gain](#optical-gain)
  - [Gain bandwidth](#gain-bandwidth)
    - [Gain narrowing](#gain-narrowing)
  - [Laser threshold](#laser-threshold)
    - [Round-trip laser threshold condition](#round-trip-laser-threshold-condition)
- [Helium-neon laser](#helium-neon-laser)
- [Optical frequency comb](#optical-frequency-comb)
  - [Mode locking](#mode-locking)
    - [Mode-locked laser](#mode-locked-laser)
  - [Carrier-envelope offset frequency](#carrier-envelope-offset-frequency)
  - [Comb self-referencing](#comb-self-referencing)
    - [Octave-spanning comb phase-control experiment](#octave-spanning-comb-phase-control-experiment)
  - [Optical frequency measurement with a comb](#optical-frequency-measurement-with-a-comb)
    - [Comb tooth index ambiguity](#comb-tooth-index-ambiguity)
- [Chirped pulse amplification](#chirped-pulse-amplification)
  - [Chirped pulse amplification energy budget](#chirped-pulse-amplification-energy-budget)
  - [Spectral phase in pulse compression](#spectral-phase-in-pulse-compression)
  - [Gaussian chirped pulse compression](#gaussian-chirped-pulse-compression)
  - [Strickland-Mourou chirped pulse amplification experiment](#strickland-mourou-chirped-pulse-amplification-experiment)
- [Attosecond physics](#attosecond-physics)
  - [High harmonic generation](#high-harmonic-generation)
    - [Three-step model of high harmonic generation](#three-step-model-of-high-harmonic-generation)
  - [Attosecond pulse train](#attosecond-pulse-train)
    - [Coherent harmonic pulse-train model](#coherent-harmonic-pulse-train-model)
  - [Isolated attosecond pulse](#isolated-attosecond-pulse)
  - [Reconstruction of attosecond beating by interference of two-photon transitions](#reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions)
    - [Two-path attosecond phase reconstruction](#two-path-attosecond-phase-reconstruction)
    - [2001 attosecond pulse-train experiment](#2001-attosecond-pulse-train-experiment)
  - [Attosecond streaking](#attosecond-streaking)
    - [2001 isolated attosecond pulse experiment](#2001-isolated-attosecond-pulse-experiment)

## Vertical-cavity surface-emitting laser

↑ **Parent:** [Laser](laser.md)

A [semiconductor](semiconductor.md) laser with a cavity normal to the wafer surface and emission through that surface.

## Excimer laser

↑ **Parent:** [Laser](laser.md)

A laser based on an excited molecular species. ArF systems commonly provide 193 nm radiation for projection lithography.

## Laser ablation

↑ **Parent:** [Laser](laser.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laser_ablation)

In [laser ablation](#laser-ablation), concentrated optical energy removes or disrupts material locally. Cutting a loaded cellular structure and observing recoil can probe its mechanics, but the recoil also depends on dissipation and surrounding constraints.

## Semiconductor laser

↑ **Parent:** [Laser](laser.md)

### Laser diode

↑ **Parent:** [Semiconductor laser](#semiconductor-laser)

## Dye laser

↑ **Parent:** [Laser](laser.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dye_laser)

A [laser](laser.md) whose gain medium contains dye [molecules](molecule.md). Its tunable [wavelength](wave-equation.md#wavelength) permits [laser spectroscopy](atomic-physics.md#laser-spectroscopy) of different [spectral lines](stellar-astrophysics.md#spectral-line).

## Three-level laser

↑ **Parent:** [Laser](laser.md)

A [three-level laser](#three-level-laser) pumps emitters out of their [ground state](quantum-mechanics.md#ground-state) into a higher pump state, which rapidly relaxes into the upper lasing state. The lower lasing state is the [ground state](quantum-mechanics.md#ground-state) itself. [Photon absorption](quantum-mechanics.md#photon-absorption) on the lasing transition therefore competes with [stimulated emission](#stimulated-emission) until enough emitters have been removed from the ground state. This is the [ground state](quantum-mechanics.md#ground-state) depletion problem implicit in [population inversion](#population-inversion).

The model below treats nondegenerate lasing [energy levels](quantum-mechanics.md#energy-level) with equal absorption and emission cross-sections. Its inversion condition is $N_2>N_1$. Real materials require the relevant sublevel populations, degeneracies and transition strengths; the simple half-population condition should not be imposed on every optical transition. Extra levels let the pump and the emitted [light](optics.md#light) act on different transitions, avoiding the steady two-level saturation limit discussed in [population inversion](#population-inversion).

### Three-level ground-state inversion threshold

↑ **Parent:** [Three-level laser](#three-level-laser)

In a [three-level laser](#three-level-laser) whose lower lasing level is the ground state, fast relaxation from a pumped higher level feeds a long-lived upper lasing level. With equal lasing-level degeneracies, negligible pump-level population and pump rate R per ground-state emitter, the no-light stationary rate equation gives $N_2/N_1=R\tau_{21}$. Positive [population inversion](#population-inversion) therefore requires more than half the active emitters to leave the ground state. This is a transparency threshold; [optical resonator](optical-instrument.md#optical-cavity) loss imposes an additional positive-gain requirement. Degenerate sublevels require population comparisons weighted by their statistical weights and transition strengths.

### Ruby laser

↑ **Parent:** [Three-level laser](#three-level-laser)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ruby_laser)

A [ruby laser](#ruby-laser) uses [chromium](chemical-substance.md#chromium) [ions](chemistry.md#ion) in [ruby](chemical-substance.md#ruby) as its amplifying medium. Maiman's report identifies a metastable state fed by optical excitation and red emission near $694.3\,\mathrm{nm}$.[Stimulated Optical Radiation in Ruby, opening and level-scheme paragraphs](physics-bibliography.md#stimulated-optical-radiation-in-ruby-by-theodore-harold-maiman) The pump stores excitation in the medium; [stimulated emission](#stimulated-emission) transfers it into the optical field. The simplified [three-level laser rate equation](#three-level-laser-rate-equation) explains why the stored population and the output pulse evolve together.

#### Maiman ruby laser experiment

↑ **Parent:** [Ruby laser](#ruby-laser)

[Theodore Harold Maiman](physicist.md#theodore-harold-maiman) and [Irnee J. D'Haenens](physics-author.md#irnee-j-d-haenens) obtained laser action in May 1960. Their arrangement put a ruby rod inside a helical xenon flashlamp. Increasing excitation produced a marked intensity threshold, with subsequent measurements showing narrowing of the ruby emission line.[Participant recollection: apparatus opening; paragraphs beginning In early 1960 and Subsequent measurements](physics-bibliography.md#theodore-harold-maiman-by-irnee-j-d-haenens) The 1960 letter describes silvered parallel crystal faces and compares low- and high-excitation spectra.[Apparatus paragraph and Fig. 2, low- and high-power spectra](physics-bibliography.md#stimulated-optical-radiation-in-ruby-by-theodore-harold-maiman)

<a id="image-pump-a-crystal-store-excitation-and-return-light-through-the-gain-medium"></a>
![](ruby-laser-flashlamp-and-three-level-cycle.png)

**[Figure 1](#image-pump-a-crystal-store-excitation-and-return-light-through-the-gain-medium). Pump a crystal, store excitation, and return light through the gain medium**. Original functional [ruby laser](#ruby-laser) diagram and simplified [three-level laser](#three-level-laser) cycle, not a construction plan or a copy of a historical drawing. The end faces provide optical feedback; no measured reflectivity, dimensions or output-coupling geometry are assigned. The energy sketch uses a chosen $550\,\mathrm{nm}$ pump photon and $694.3\,\mathrm{nm}$ emitted photon, with a fast nonradiative step. Actual crystal sublevels and the broadband flashlamp are not resolved by this three-state sketch.

The controls answer different questions. Increased brightness establishes neither optical feedback nor narrow-band emission by itself: ordinary [fluorescence](fluorescence.md) can also brighten with pumping. Comparing spectra at lower and higher excitation, retaining the same optical collection geometry, tests a change in the emission process. Spectrometer resolution, response saturation and heating can alter an apparent line profile; a bright spot alone cannot distinguish those effects. These are interpretation requirements, rather than additional measurements attributed to the short original letter.

Several experimental models were made. The Smithsonian's surviving head has uncertain priority, and its installed crystal came from a later experiment.[Description: multiple experimental models, uncertain first-unit identification and replacement crystal](physics-bibliography.md#head-piece-from-maiman-laser-by-smithsonian-institution) The functional diagram therefore describes the optical mechanism rather than claiming to reconstruct the first surviving unit.

### Three-level laser rate equation

↑ **Parent:** [Three-level laser](#three-level-laser)

Consider an original reduced model with a fixed number $N$ of active emitters. Let $u=N_2/N$ be the upper lasing-state fraction, $1-u=N_1/N$ the ground-state fraction, and $s=n/N$ the number of cavity [photons](quantum-mechanics.md#photon) per emitter. Assume the pump state empties rapidly, so its population can be neglected. Measure time by $x=t/\tau$, where $\tau$ is the upper state's spontaneous lifetime. Let $r=W\tau$ be the effective pump rate, $C>0$ the dimensionless stimulated-coupling coefficient, $K>0$ the photon-loss rate in these units, and $0\leq\beta\leq1$ the fraction of spontaneous decays feeding this optical [normal mode](wave-equation.md#normal-mode). The [rate equations](mathematical-biology.md#rate-equation) are

$$
\frac{du}{dx}=r(1-u)-u-C(2u-1)s,
\qquad
\frac{ds}{dx}=\bigl[C(2u-1)-K\bigr]s+\beta u.
$$

Each term has a physical role. Pumping transfers emitters out of the ground state; [spontaneous emission](atomic-physics.md#spontaneous-emission) removes upper-state population. The net stimulated term includes emission from fraction $u$ and absorption by fraction $1-u$, giving their difference $2u-1$. A stimulated transition removes one stored excitation and creates one cavity [photon](quantum-mechanics.md#photon), or does the reverse. The factor $\beta$ accounts for spontaneous emission into the selected mode without pretending that all [spontaneous emission](atomic-physics.md#spontaneous-emission) enters it.

For negligible cavity light, the upper-state equation is linear. A constant pump applied to $u(0)=0$ gives

$$
u(x)=\frac{r}{r+1}\left(1-e^{-(r+1)x}\right),\qquad
u_\infty=\frac{r}{r+1}.
$$

Thus this model first permits [population inversion](#population-inversion) at $r>1$. Positive [optical gain](#optical-gain) is still insufficient for an oscillator: the gain must exceed the complete [laser threshold](#laser-threshold), including photon loss. The small-signal photon growth coefficient changes sign when

$$
C(2u-1)=K,\qquad
u_{\rm th}=\frac{1+K/C}{2},\qquad
\boxed{r_{\rm th}=\frac{C+K}{C-K}\quad(C>K).}
$$

If $C\leq K$, even complete inversion cannot exceed the assumed loss in this model. For chosen $C=100$ and $K=20$, the threshold population is $u_{\rm th}=0.6$ and the pump threshold is $r_{\rm th}=1.5$. At $r=2$, the unsaturated population first reaches $0.6$ at $x=(\log10)/3\simeq0.7675$. These numbers are stipulated examples, not ruby material parameters.

#### Laser gain clamping

↑ **Parent:** [Three-level laser rate equation](#three-level-laser-rate-equation)

In the steady limit with nonzero cavity light and negligible spontaneous seeding, the photon equation requires $C(2u-1)=K$. The upper-state fraction is therefore fixed near $u_{\rm th}$ while increased pumping principally increases the photon population. Substituting into the population equation gives

$$
u=u_{\rm th},\qquad
s=\frac{r(1-u_{\rm th})-u_{\rm th}}{K}\quad(r>r_{\rm th}).
$$

For $C=100$, $K=20$ and $r=3$, this predicts $u=0.6$ and $s=0.03$. The inversion does not rise indefinitely above threshold. A finite $\beta$ supplies seed photons and smooths the ideal onset; with $\beta=0$ and exactly $s(0)=0$, the deterministic equations remain on the zero-photon solution even when that solution is unstable. This distinguishes instability of an unseeded state from actual startup of a noisy optical field.

#### Stored excitation in a pulsed laser

↑ **Parent:** [Three-level laser rate equation](#three-level-laser-rate-equation)

A short optical pulse can draw on previously stored excitation. In the original calculation below, $C=100$, $K=20$, $\beta=10^{-4}$, $u(0)=s(0)=0$, and $r=3$ for $0\leq x<4$, followed by $r=0$. The cavity field initially remains small while pumping fills the upper state. Once sufficient gain develops, the photon population grows and depletes the stored inversion. Continuing pump action can refill it, giving [relaxation oscillations](dynamical-systems.md#relaxation-oscillation) in this simple model. This is not a fit to Maiman's recorded output.

<a id="image-ground-state-depletion-delays-startup-and-cavity-light-then-drains-stored-excitation"></a>
![](three-level-laser-pump-threshold-and-pulse.png)

**[Figure 2](#image-ground-state-depletion-delays-startup-and-cavity-light-then-drains-stored-excitation). Ground-state depletion delays startup, and cavity light then drains stored excitation**. Original [three-level laser rate equation](#three-level-laser-rate-equation) calculations. Left: negligible-light upper-state fractions for several constant pumps, compared with the chosen $u_{\rm th}=0.6$. Right: coupled upper-state and cavity-photon populations for $C=100$, $K=20$, $\beta=10^{-4}$ and a pump of $r=3$ switched off at $t/\tau=4$. The rates and times are dimensionless teaching inputs, not measured ruby lifetimes or a historical pulse trace.

The equations expose the excitation budget underlying [conservation of energy](mathematical-physics.md#conservation-of-energy). Adding them cancels the stimulated exchange:

$$
\frac{d(u+s)}{dx}=r(1-u)-(1-\beta)u-Ks.
$$

Pumping supplies excitations; nonlasing decay and cavity loss remove them. Integrating gives the bound

$$
\int_0^X Ks\,dx\leq u(0)+s(0)+\int_0^Xr(1-u)\,dx.
$$

Only part of the cavity loss may be useful output; passive absorption is also a loss. The pulse's instantaneous power can draw on stored excitation, while its total extracted energy still obeys the integrated budget. The model also preserves $0\leq u\leq1$ and $s\geq0$: at each boundary its derivatives point inward or along the boundary.

There is a further energy cost in the pump cycle. For one absorbed pump photon producing at most one emitted laser photon, the ideal energy-conversion bound is

$$
\eta\leq\frac{h\nu_{\rm laser}}{h\nu_{\rm pump}}
=\frac{\lambda_{\rm pump}}{\lambda_{\rm laser}}.
$$

Chosen wavelengths $550\,\mathrm{nm}$ and $694.3\,\mathrm{nm}$ give about $0.7922$ before other losses. The missing energy can leave through nonradiative relaxation and heating. Actual efficiency also depends on how much pump light is absorbed, unwanted decays and optical losses; a population model alone cannot predict it.

## Laser detuning

↑ **Parent:** [Laser](laser.md)

[Laser detuning](#laser-detuning) is the difference between a [laser](laser.md) [angular frequency](lagrangian-mechanics.md#angular-frequency) and a specified atomic resonance [angular frequency](lagrangian-mechanics.md#angular-frequency). Red detuning has $\delta<0$; blue detuning has $\delta>0$. The sign matters in [laser cooling](atomic-physics.md#laser-cooling): a moving atom can see a red-detuned [laser](laser.md) closer to resonance because of the [Doppler effect](wave.md#doppler-effect).

## Stimulated emission

↑ **Parent:** [Laser](laser.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stimulated_emission)

Stimulated emission is emission induced by incident [light](optics.md#light), in contrast with the unprompted decay in [spontaneous emission](atomic-physics.md#spontaneous-emission). It supplies the amplification mechanism of a [laser](laser.md). [OpenStax, §8.6: stimulated emission](https://openstax.org/books/university-physics-volume-3/pages/8-6-lasers).

For an emitter with upper and lower [energy](energy.md) values $E_2>E_1$, the resonant [photon](quantum-mechanics.md#photon) has [frequency](wave.md#frequency) $\nu$ satisfying

$$
\Delta E=E_2-E_1=h\nu,
$$

where $h$ is the [Planck constant](quantum-mechanics.md#planck-constant). In the elementary [photon](quantum-mechanics.md#photon) picture, an incident [photon](quantum-mechanics.md#photon) stimulates an emitter in the upper [quantum state](quantum-system.md#quantum-state) to emit an additional [photon](quantum-mechanics.md#photon) into the same optical [normal mode](wave-equation.md#normal-mode), with the same [frequency](wave.md#frequency), propagation direction and [photon polarization](quantum-mechanics.md#photon-polarization). The emitter supplies the extra [energy](energy.md); the stimulating [photon](quantum-mechanics.md#photon) is not consumed. This builds the existing field and its [optical coherence](physical-optics.md#optical-coherence). An emitter in the lower [quantum state](quantum-system.md#quantum-state) can instead undergo [photon absorption](quantum-mechanics.md#photon-absorption), so [stimulated emission](#stimulated-emission) alone does not establish net [optical gain](#optical-gain).

For example, a $2.0\,\mathrm{eV}$ gap corresponds to $\nu\approx4.8360\times10^{14}\,\mathrm{Hz}$ and a [vacuum](physics.md#vacuum) [wavelength](wave-equation.md#wavelength) of about $620\,\mathrm{nm}$. One ideal [stimulated emission](#stimulated-emission) event converts one incoming [photon](quantum-mechanics.md#photon) into two outgoing [photons](quantum-mechanics.md#photon) in the selected optical [normal mode](wave-equation.md#normal-mode), adding $2.0\,\mathrm{eV}$ of [light](optics.md#light) [energy](energy.md) while lowering the emitter's [energy](energy.md) by that amount.

<a id="image-stimulated-emission-and-one-illustrative-four-level-laser-pumping-cycle"></a>
![](laser-stimulated-emission-cycle.png)

**[Figure 3](#image-stimulated-emission-and-one-illustrative-four-level-laser-pumping-cycle). Stimulated emission and one illustrative four-level laser pumping cycle**. Left: one incoming [photon](quantum-mechanics.md#photon) induces an additional [photon](quantum-mechanics.md#photon) while the emitter falls from $E_2$ to $E_1$. Right: pumping supplies [energy](energy.md), rapid relaxation feeds the upper lasing state, [stimulated emission](#stimulated-emission) supplies [light](optics.md#light), and rapid lower-state relaxation completes a four-level cycle. These paths are schematic, not universal to all [lasers](laser.md); line spacing is not to scale.

### Photon occupation enhancement of emission

↑ **Parent:** [Stimulated emission](#stimulated-emission)

The creation-operator [matrix element](vector-space.md#matrix-element) $\langle n+1|a^\dagger|n\rangle=\sqrt{n+1}$ makes emission into a radiation mode proportional to $n+1$. The $n$ part is [stimulated emission](#stimulated-emission) and the remaining part is [spontaneous emission](atomic-physics.md#spontaneous-emission). Absorption has the corresponding occupation factor $n$.

### Population inversion

↑ **Parent:** [Stimulated emission](#stimulated-emission)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Population_inversion)

A [population inversion](#population-inversion) puts more emitters in the upper than in the lower [quantum state](quantum-system.md#quantum-state) of a transition in the nondegenerate two-level model. Let $N_2,N_1$ be their number densities. Equal stimulated-transition strengths make the emission rate proportional to $N_2$ and the competing [photon absorption](quantum-mechanics.md#photon-absorption) rate proportional to $N_1$, so net [optical gain](#optical-gain) is proportional to $N_2-N_1$. For $N_2=6\times10^{20}\,\mathrm{m^{-3}}$ and $N_1=4\times10^{20}\,\mathrm{m^{-3}}$, the difference is positive; swapping them makes the medium absorb. Equal populations give zero net stimulated contribution. With degenerate levels, the relevant comparison uses populations per [statistical weight of an atomic level](atomic-physics.md#statistical-weight-of-an-atomic-level), rather than simply $N_2>N_1$.

Why pump through extra levels? Ordinary steady resonant pumping of a nondegenerate two-level system drives both [photon absorption](quantum-mechanics.md#photon-absorption) and [stimulated emission](#stimulated-emission). With equal induced rate $W$ and upper-state decay rate $\Gamma$, its elementary population equation is

$$
\dot N_2=W(N_1-N_2)-\Gamma N_2,
\qquad
\frac{N_2}{N_1}=\frac{W}{W+\Gamma}\leq1
$$

at a stationary population. Increasing this pump saturates towards $N_2=N_1$; it cannot sustain [population inversion](#population-inversion) in this model. This is a steady rate-equation conclusion, not a universal prohibition on all driven two-level dynamics or all possible [laser](laser.md) gain mechanisms. [Franz Kärtner, MIT 6.974, Chapter 6, §§6.7–6.8: saturation and rate equations](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/2641db6431ea70989c29e8512d5d91a7_chapter6.pdf).

In a familiar three-level path, pumping excites a higher level which relaxes into the upper lasing level; the lower lasing level is the ground state, so substantial ground-state depletion is needed. A four-level path also provides rapid emptying of the lower lasing level into a separate ground state. Suitable lifetimes then allow accumulation above and depletion below the lasing transition. Pumping still supplies the [energy](energy.md): extra levels provide a route to [population inversion](#population-inversion), not free [energy](energy.md). [Franz Kärtner, MIT 6.974, §7.2.1: three- and four-level laser media](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/18f30fad63a62ef4dd894d3752b55a60_chapter7.pdf).

#### Lower-level depopulation in a four-level laser

↑ **Parent:** [Population inversion](#population-inversion)

A pump feeds an auxiliary high level, rapid relaxation populates the upper [laser](laser.md) level, and rapid decay empties the lower [laser](laser.md) level. This separates pumping from the [laser](laser.md) transition and helps sustain net stimulated gain. Gain saturation and cavity loss still determine the oscillating steady state.

## Optical gain

↑ **Parent:** [Laser](laser.md)

[Optical gain](#optical-gain) is amplification of [light](optics.md#light) by a medium. Here the small-signal intensity gain coefficient $g$ has units $\mathrm{m^{-1}}$: for fixed populations, a weak beam obeys

$$
\frac{dI}{dz}=gI,
\qquad I(z)=I(0)e^{gz},
\qquad g=\sigma(N_2-N_1)
$$

in the nondegenerate resonant two-level model, with common transition cross-section $\sigma$. Thus $g$ includes the competition between [stimulated emission](#stimulated-emission) and [photon absorption](quantum-mechanics.md#photon-absorption) on that transition. Separate passive intensity loss $\alpha$ gives $I(z)=I(0)e^{(g-\alpha)z}$. Both coefficients describe [light intensity](wave.md#light-intensity), not [wave amplitude](wave.md#wave-amplitude); the corresponding field-amplitude exponent is half as large. [Franz Kärtner, MIT 6.974, §§6.7–6.8: amplification and stimulated-transition cross-section](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/2641db6431ea70989c29e8512d5d91a7_chapter6.pdf).

For $g=0.30\,\mathrm{m^{-1}}$, $\alpha=0.10\,\mathrm{m^{-1}}$ and $z=0.50\,\mathrm m$, the single-pass intensity multiplier is $e^{0.10}\approx1.10517$. This is amplification during one passage, before mirror losses. [Population inversion](#population-inversion) can therefore yield positive [optical gain](#optical-gain) while the complete oscillator remains below [laser threshold](#laser-threshold).

### Gain bandwidth

↑ **Parent:** [Optical gain](#optical-gain)

The [frequency](wave.md#frequency) range over which an amplifying medium supplies appreciable [optical gain](#optical-gain). Its width must be stated with a gain-profile convention.

#### Gain narrowing

↑ **Parent:** [Gain bandwidth](#gain-bandwidth)

Narrowing of a pulse spectrum when the central [frequencies](wave.md#frequency) receive larger [optical gain](#optical-gain) than its wings. Phase correction alone cannot restore the suppressed spectrum.

### Laser threshold

↑ **Parent:** [Optical gain](#optical-gain)

In a simple two-mirror oscillator, [laser threshold](#laser-threshold) is the small-signal [optical gain](#optical-gain) at which a resonant optical [normal mode](wave-equation.md#normal-mode) exactly replaces its round-trip intensity loss. Assume constant intensity coefficients $g$ and $\alpha$ throughout a one-way distance $L$, and mirror intensity reflectivities $0<R_1,R_2\leq1$. One round trip has multiplier

$$
M=R_1R_2\exp\bigl(2(g-\alpha)L\bigr),
\qquad
I_{n+1}=MI_n.
$$

Two traversals give the distance $2L$; multiplying the two mirror factors completes the bookkeeping. Setting $M=1$ and taking a [logarithm](calculus.md#logarithm) gives

$$
g_{\mathrm{th}}=\alpha-\frac{\ln(R_1R_2)}{2L}.
$$

The reflectivities here are intensity fractions, not field-amplitude reflectivities. A shorter gain region or nonuniform loss requires replacing the path exponent by the appropriate path integral. The balance also presumes a permitted resonant optical [normal mode](wave-equation.md#normal-mode). [Franz Kärtner, MIT 6.974, §§7.1 and 7.5: round-trip balance and steady state; intensity convention specified here](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/18f30fad63a62ef4dd894d3752b55a60_chapter7.pdf).

For $L=0.50\,\mathrm m$, $R_1=1$, $R_2=0.90$ and $\alpha=0.10\,\mathrm{m^{-1}}$, the threshold is $g_{\mathrm{th}}\approx0.2053605\,\mathrm{m^{-1}}$. At $g=0.15\,\mathrm{m^{-1}}$, $M\approx0.946144$: a small circulating signal decays even though the material has positive [optical gain](#optical-gain). At $g=0.30\,\mathrm{m^{-1}}$, $M\approx1.099262$: the signal initially grows. Raising passive loss or lowering mirror reflectivity raises [laser threshold](#laser-threshold).

<a id="image-round-trip-intensity-balance-and-laser-threshold-in-a-two-mirror-model"></a>
![](laser-round-trip-gain-threshold.png)

**[Figure 4](#image-round-trip-intensity-balance-and-laser-threshold-in-a-two-mirror-model). Round-trip intensity balance and laser threshold in a two-mirror model**. The curve uses $M=R_1R_2e^{2(g-\alpha)L}$ with intensity reflectivities $R_1=1$, $R_2=0.90$, one-way length $L=0.50\,\mathrm m$ and passive intensity loss $\alpha=0.10\,\mathrm{m^{-1}}$. The two worked cases straddle $M=1$. The right panel shows how a smaller output-mirror reflectivity raises the required small-signal intensity gain.

For $M>1$, the fixed-gain recurrence predicts startup amplification, not infinite actual output. Growing [light intensity](wave.md#light-intensity) depletes the available [population inversion](#population-inversion), reducing [optical gain](#optical-gain) through saturation. In the simplest steady oscillator, the saturated round-trip gain balances loss and pumping supplies the outgoing [power](energy.md#power) and dissipated [energy](energy.md). The small-signal model locates the onset; it does not determine the final output [power](energy.md#power). [Franz Kärtner, MIT 6.974, §7.5: gain saturation and steady output](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/18f30fad63a62ef4dd894d3752b55a60_chapter7.pdf).

#### Round-trip laser threshold condition

↑ **Parent:** [Laser threshold](#laser-threshold)

If $g$ and $\alpha_i$ are intensity gain and loss per length, a linear cavity has round-trip intensity multiplier $R_1R_2e^{2(g-\alpha_i)L}$. Threshold occurs when it equals one, giving $g_{\rm th}=\alpha_i+\log[1/(R_1R_2)]/(2L)$. Phase resonance and the gain bandwidth determine which modes can oscillate.

## Helium-neon laser

↑ **Parent:** [Laser](laser.md)

A [helium-neon laser](#helium-neon-laser) is a gas [laser](laser.md) using a mixture of [helium](chemical-substance.md#helium) and [neon](chemical-substance.md#neon).

## Optical frequency comb

↑ **Parent:** [Laser](laser.md)

An [optical frequency comb](#optical-frequency-comb) has evenly spaced optical [spectral lines](stellar-astrophysics.md#spectral-line), or teeth. A [mode-locked laser](#mode-locked-laser) supplies short [optical pulses](optics.md#optical-pulse) at repetition [frequency](wave.md#frequency) $f_r$, the tooth spacing. The [carrier-envelope offset frequency](#carrier-envelope-offset-frequency) $f_0$ positions the whole ruler:

$$
f_n=n f_r+f_0,\qquad n\in\mathbb Z,\qquad 0\leq f_0<f_r.
$$

Only teeth within the emitted [optical spectrum](optics.md#optical-spectrum) are present; the extrapolated intercept need not be an emitted tooth.[Passion for Precision, p.157: tooth relation](physics-bibliography.md#passion-for-precision-by-theodor-w-hansch)

The achievement associated with [John L. Hall](physicist.md#john-l-hall) and [Theodor W. Hänsch](physicist.md#theodor-w-hansch) is a practical bridge between optical [frequencies](wave.md#frequency) and countable electronic [frequencies](wave.md#frequency). Instead of constructing a separate chain of [lasers](laser.md) for each optical measurement, a broad comb supplies many linked reference teeth. Stable [lasers](laser.md), short [optical pulses](optics.md#optical-pulse) and strong [nonlinear optics](optics.md#nonlinear-optics) in [optical fibers](optical-instrument.md#optical-fiber) came together around 1999–2000.[Nobel Lecture: Defining and measuring optical frequencies, pp.1288–1291: chains and comb development](physics-bibliography.md#nobel-lecture-defining-and-measuring-optical-frequencies-by-john-l-hall)

### Mode locking

↑ **Parent:** [Optical frequency comb](#optical-frequency-comb)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mode-locking)

[Mode locking](#mode-locking) fixes relative [phases](wave.md#phase-waves) between longitudinal [normal modes](wave-equation.md#normal-mode) of a [laser](laser.md), allowing short [optical pulses](optics.md#optical-pulse). The same [optical spectrum](optics.md#optical-spectrum) with wandering relative [phases](wave.md#phase-waves) would not supply that stable pulse train.[Passion for Precision, p.157: coupled modes](physics-bibliography.md#passion-for-precision-by-theodor-w-hansch)

Here is an original finite-mode model, with the convention that a positive [frequency](wave.md#frequency) has time dependence $e^{2\pi i f t}$:

$$
E(t)=\sum_{n=24}^{40}a_n e^{2\pi i(n f_r+f_0)t},\qquad
a_n=\frac{e^{-(n-32)^2/18}}{\sum_{j=24}^{40}e^{-(j-32)^2/18}}.
$$

These field coefficients follow a [Gaussian function](calculus.md#gaussian-function) and have aligned [phases](wave.md#phase-waves) at $t=0$. Choose $f_0=f_r/4$ and write $T=1/f_r$. Since $e^{2\pi i n}=1$ for every [integer](integer.md) $n$,

$$
E(t+T)=e^{2\pi i f_0T}E(t)=iE(t),\qquad |E(t+T)|^2=|E(t)|^2.
$$

The pulse [light intensity](wave.md#light-intensity) repeats every $T$ although the field needs four periods to repeat. At the pulse centers, $E(0)=1$, $E(T)=i$, $E(2T)=-1$ and $E(3T)=-i$. A detector of [light intensity](wave.md#light-intensity) alone therefore cannot distinguish this offset from zero. This model has far fewer teeth than a practical optical comb; its normalized time and [frequency](wave.md#frequency) scales are chosen to make the carrier oscillations visible.

<a id="image-repeated-pulse-envelopes-can-conceal-a-changing-carrier-phase"></a>
![](optical-frequency-comb-pulses-and-teeth.png)

**[Figure 5](#image-repeated-pulse-envelopes-can-conceal-a-changing-carrier-phase). Repeated pulse envelopes can conceal a changing carrier phase**. Original finite sum of 17 [normal modes](wave-equation.md#normal-mode) weighted using a [Gaussian function](calculus.md#gaussian-function), with $f_0/f_r=1/4$. Both panels represent the same complex field: the upper panel shows its real part and magnitude; the lower panel shows its field-amplitude coefficients. This is a dimensionless model, not historical measurement data.

A short proof of the converse uses the [Fourier series](fourier-series.md). If $E(t+T)=e^{i\Delta\phi}E(t)$, then $E(t)e^{-i\Delta\phi t/T}$ is periodic with period $T$. Its [Fourier series](fourier-series.md) has [frequencies](wave.md#frequency) $n/T$; restoring the removed factor shifts every tooth by $\Delta\phi/(2\pi T)$. A finite observation time broadens the spectral peaks; it does not change this ideal infinite-train relation.

#### Mode-locked laser

↑ **Parent:** [Mode locking](#mode-locking)

A [laser](laser.md) operating with [mode locking](#mode-locking).

### Carrier-envelope offset frequency

↑ **Parent:** [Optical frequency comb](#optical-frequency-comb)

The [carrier-envelope offset frequency](#carrier-envelope-offset-frequency) expresses the carrier's pulse-to-pulse [phase](wave.md#phase-waves) slip relative to its envelope. Fixing the repetition [frequency](wave.md#frequency) leaves this slip undetermined.[Defining and Measuring Optical Frequencies: The Optical Clock Opportunity – and More, p.131: offset](physics-bibliography.md#defining-and-measuring-optical-frequencies-the-optical-clock-opportunity-and-more-by-john-l-hall) With the positive-exponential convention derived above, $f_0=f_r\Delta\phi/(2\pi)$ modulo $f_r$. Changing $f_0$ translates every tooth equally; differentiating $f_n=n f_r+f_0$ at fixed $n$ gives

$$
\delta f_n=n\,\delta f_r+\delta f_0.
$$

Thus at $n=2\times10^6$, a chosen $1\,\mathrm{Hz}$ change in spacing moves that tooth by $2\,\mathrm{MHz}$ if $f_0$ stays fixed. The large multiplier is why a stable-looking pulse train is insufficient for accurate optical [metrology](physics.md#metrology).

### Comb self-referencing

↑ **Parent:** [Optical frequency comb](#optical-frequency-comb)

[Comb self-referencing](#comb-self-referencing) compares two parts of one [optical frequency comb](#optical-frequency-comb). Coherent broadening supplies an octave, a factor of two in [frequency](wave.md#frequency). [Second-harmonic generation](optics.md#second-harmonic-generation) doubles a red tooth; a [photodiode](optical-instrument.md#photodiode) detects its [beat](physical-optics.md#beat) with an original blue tooth.[Introduction to Self-reference Comb Laser, Fig.1 explanation](physics-bibliography.md#introduction-to-self-reference-comb-laser-by-comblaser-laboratory-department-of-physics-national-central-university) Applying the tooth formula gives

$$
2f_n-f_{2n}=2(n f_r+f_0)-(2n f_r+f_0)=f_0.
$$

The doubled branch carries $2f_0$, while the original high-frequency branch carries $f_0$: their difference retains exactly one offset.

<a id="image-read-the-tooth-spacing-and-offset-through-separate-electronic-signals"></a>
![](optical-frequency-comb-self-reference.png)

**[Figure 6](#image-read-the-tooth-spacing-and-offset-through-separate-electronic-signals). Read the tooth spacing and offset through separate electronic signals**. Original functional [comb self-referencing](#comb-self-referencing) scheme. Solid optical paths bring doubled red light and original blue light to one detector. Dashed electronic paths connect both readouts to a common reference and feedback controls. Actuators can affect both parameters.

The displayed difference uses the order doubled tooth minus original tooth. An ordinary electronic [frequency counter](electrical-engineering.md#frequency-counter) returns a nonnegative [beat](physical-optics.md#beat) magnitude; spectral selection and known electronic shifts must identify whether it represents $f_0$, $f_r-f_0$, or a shifted version. Coherent broadening, overlapping [photon polarization](quantum-mechanics.md#photon-polarization), spatial alignment and temporal overlap are required. Merely producing a broad patch of colored [light](optics.md#light) does not establish a usable offset signal.

#### Octave-spanning comb phase-control experiment

↑ **Parent:** [Comb self-referencing](#comb-self-referencing)

The 2000 experiment prepared [optical pulses](optics.md#optical-pulse) with a [mode-locked laser](#mode-locked-laser) and broadened them in an air-silica microstructure [optical fiber](optical-instrument.md#optical-fiber). A wavelength-selective [beam splitter](optical-instrument.md#beam-splitter) separated red and blue light. A nonlinear crystal doubled the red branch; the blue branch received a known acousto-optic shift. A filter selected recombined light for an avalanche [photodiode](optical-instrument.md#photodiode), supplying an electronic [beat](physical-optics.md#beat). Mirror translation controlled repetition [frequency](wave.md#frequency); mirror tilt controlled offset with coupled effects. Separate delayed-pulse [interference](physical-optics.md#interference-wave-propagation) tested programmed [phase](wave.md#phase-waves) changes. Alternative envelope fits and unmatched optical reflections were examined as checks and limitations.[Science 288, pp.636–638, Figs.2,4–5: apparatus and temporal check; Tokushima mirror](physics-bibliography.md#carrier-envelope-phase-control-of-femtosecond-mode-locked-lasers-and-direct-optical-frequency-synthesis-by-david-j-jones-and-others)

These readouts answer different questions. The electronic [beat](physical-optics.md#beat) closes a feedback loop; changing its setpoint and checking the delayed-pulse [phase](wave.md#phase-waves) tests whether that control reaches the optical waveform. Neither readout alone establishes the accuracy of an unknown optical [frequency](wave.md#frequency). That additionally requires a calibrated time reference, the correct tooth number and [beat](physical-optics.md#beat) sign, and checks for missed cycles and drift. The ideal unshifted diagram above omits the experiment's known acousto-optic shift; its actual raw detector [frequency](wave.md#frequency) must be corrected for that shift before identifying $f_0$.

### Optical frequency measurement with a comb

↑ **Parent:** [Optical frequency comb](#optical-frequency-comb)

Mix an unknown single-frequency [laser](laser.md) with a nearby comb tooth on a [photodiode](optical-instrument.md#photodiode). Define the signed [beat](physical-optics.md#beat) $b=f_L-f_n$, so

$$
f_L=n f_r+f_0+b.
$$

The [beat](physical-optics.md#beat) arises from the cross term in [light intensity](wave.md#light-intensity):

$$
\left|A e^{2\pi i f_Lt}+B e^{2\pi i f_nt}\right|^2
=|A|^2+|B|^2+2\operatorname{Re}\!\left(AB^*e^{2\pi i b t}\right).
$$

An electronic detector can follow this slow difference even though it cannot resolve either optical oscillation. The square-law expression also shows why a real-valued intensity trace by itself loses the sign of $b$. A small known upward shift of the chosen tooth decreases $|b|$ when the unknown lies above it and increases $|b|$ when it lies below, provided the tooth assignment remains unchanged.

For an original example, stipulate

$$
f_r=250\,\mathrm{MHz},\qquad f_0=20\,\mathrm{MHz},\qquad b=+30\,\mathrm{MHz},\qquad n=2{,}000{,}000.
$$

Then $f_n=500{,}000.020\,\mathrm{GHz}$ and $f_L=500{,}000.050\,\mathrm{GHz}$. Choosing the opposite sign would give $499{,}999.990\,\mathrm{GHz}$ instead. The stipulated optical [frequency](wave.md#frequency) is countable because the large optical value is expressed using the [integer](integer.md) $n$ and three electronic [frequencies](wave.md#frequency); the diagram's two controls establish the comb, and this additional [beat](physical-optics.md#beat) places the unknown against it.

Both comb readouts use one calibrated [microwave](electromagnetic-radiation.md#microwave) reference. Feedback fixes $f_r$ and $f_0$, determining each tooth once $n$ is identified. A [frequency counter](electrical-engineering.md#frequency-counter) measures the slow [beat](physical-optics.md#beat), transferring the calibration to the optical [frequency](wave.md#frequency).[Passion for Precision, p.158: microwave link](physics-bibliography.md#passion-for-precision-by-theodor-w-hansch)

#### Comb tooth index ambiguity

↑ **Parent:** [Optical frequency measurement with a comb](#optical-frequency-measurement-with-a-comb)

One [beat](physical-optics.md#beat) magnitude does not tell us the [integer](integer.md) $n$. In the example, every proposed optical [frequency](wave.md#frequency) $n(250\,\mathrm{MHz})+50\,\mathrm{MHz}$ produces the same signed [beat](physical-optics.md#beat) with its corresponding tooth. A coarse independent optical measurement can select the [integer](integer.md): once the [beat](physical-optics.md#beat) sign is known, an error bound below $f_r/2$ suffices if the candidate is selected by nearest distance.

There is also a useful two-spacing check. Keep the unknown [laser](laser.md) and $f_0$ fixed, track the same tooth continuously, and increase $f_r$ by a stipulated $5\,\mathrm{Hz}$. Its [frequency](wave.md#frequency) rises by $10\,\mathrm{MHz}$, so the signed [beat](physical-optics.md#beat) falls from $30$ to $20\,\mathrm{MHz}$. Hence

$$
n=-\frac{\Delta b}{\Delta f_r}=\frac{10{,}000{,}000}{5}=2{,}000{,}000.
$$

This inference fails if the unknown drifts appreciably, the offset changes unnoticed, the [beat](physical-optics.md#beat) sign is lost, or the tracker jumps to another tooth. The assumed tooth motion stays well below half the spacing in this example. If $f_0$ also changes by a measured amount, use $n=-(\Delta b+\Delta f_0)/\Delta f_r$.

For a fixed verified tooth number, the first-order [frequency](wave.md#frequency) error is $\delta f_L=n\delta f_r+\delta f_0+\delta b$. Errors in these readings can be correlated because they share a reference. A small [beat](physical-optics.md#beat) uncertainty therefore does not imply the same absolute optical accuracy: the reference's calibration and the factor $n$ remain in the error budget. A wrong tooth number is a separate discrete error, not a small correction. The beauty of the comb is that two controlled parameters organize millions of optical reference points, while the unknown's position is read electronically.

## Chirped pulse amplification

↑ **Parent:** [Laser](laser.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chirped_pulse_amplification)

[Chirped pulse amplification](#chirped-pulse-amplification) increases an [optical pulse](optics.md#optical-pulse)'s [energy](energy.md) while keeping its [peak power](energy.md#peak-power) lower during amplification: stretch the pulse, amplify it, then compress it. A [chirp](wave.md#chirp) is a changing instantaneous [frequency](wave.md#frequency). Stretching separates the arrival times of different [frequencies](wave.md#frequency); [pulse compression](optics.md#pulse-compression) brings their contributions back together. The gain medium supplies [energy](energy.md), whereas the compressor concentrates the surviving [energy](energy.md) into a shorter time.

[Donna Strickland](physicist.md#donna-strickland) and [Gérard Mourou](physicist.md#gerard-mourou) demonstrated [chirped pulse amplification](#chirped-pulse-amplification) at Rochester in 1985. Their experiment used an [optical fiber](optical-instrument.md#optical-fiber), a regenerative amplifier and a [diffraction grating](physical-optics.md#diffraction-grating) compressor.[Strickland and Mourou, corrected December 1985 paper, pp.219–221](physics-bibliography.md#compression-of-amplified-chirped-optical-pulses-by-donna-strickland-and-gerard-mourou)

<a id="image-stretch-add-energy-then-recover-a-short-pulse"></a>
![](chirped-pulse-amplification-stretch-amplify-compress.png)

**[Figure 7](#image-stretch-add-energy-then-recover-a-short-pulse). Stretch, add energy, then recover a short pulse**. Original functional [chirped pulse amplification](#chirped-pulse-amplification) diagram using chosen [Gaussian functions](calculus.md#gaussian-function) for pulse [power](energy.md#power). The common time axes show the stretching; each vertical axis has its own labelled scale. The idealized amplifier has flat [optical gain](#optical-gain) across the occupied spectrum, and the compressor transmits 80 percent of the incident [energy](energy.md). These are teaching assumptions, not a reconstruction of the 1985 apparatus or a measured pulse trace.

The useful idea is to arrange where the large [peak power](energy.md#peak-power) occurs. Lower [light intensity](wave.md#light-intensity) in the amplifier reduces unwanted [self-focusing](optics.md#self-focusing) and [self-phase modulation](optics.md#self-phase-modulation); the compressed output can still drive strong [nonlinear optics](optics.md#nonlinear-optics). Stretching does not remove every damage mechanism, and compression does not manufacture [energy](energy.md).

### Chirped pulse amplification energy budget

↑ **Parent:** [Chirped pulse amplification](#chirped-pulse-amplification)

Let $P(t)$ be the pulse's [power](energy.md#power) integrated over its transverse section, and $U$ its [energy](energy.md). Its [peak power](energy.md#peak-power) is $\max_t P(t)$. For a chosen Gaussian power envelope with [full width at half maximum](analysis.md#full-width-at-half-maximum) $\tau$,

$$
P(t)=P_{\rm pk}e^{-4\ln2\,t^2/\tau^2},\qquad
U=P_{\rm pk}\tau\sqrt{\frac{\pi}{4\ln2}},\qquad
P_{\rm pk}=\sqrt{\frac{4\ln2}{\pi}}\frac{U}{\tau}.
$$

The numerical shape factor is approximately $0.9394$. It matters when comparing quoted [peak powers](energy.md#peak-power); the estimate $U/\tau$ assumes a shape and a width convention.

If an otherwise unchanged pulse is stretched by a factor $S$ without loss, its [energy](energy.md) stays fixed and its [peak power](energy.md#peak-power) falls by $S$. For energy gain $G$ and compressor energy transmission $\eta$, ideal restoration of the original shape gives

$$
U_{\rm out}=\eta G U_{\rm in},\qquad
\frac{P_{{\rm pk},\,\rm out}}{P_{{\rm pk},\,\rm amplified}}=\eta S.
$$

These relations require a specified shape and preserved spectrum; they do not model amplifier saturation. For the diagram's chosen $1\,\mathrm{nJ}$, $30\,\mathrm{fs}$ seed, $S=9.2959$, $G=1000$ and $\eta=0.8$, the successive [peak powers](energy.md#peak-power) are $31.31\,\mathrm{kW}$, $3.369\,\mathrm{kW}$, $3.369\,\mathrm{MW}$ and $25.05\,\mathrm{MW}$. The last pulse contains $0.8\,\mathrm{\mu J}$: the compressor increases [peak power](energy.md#peak-power) while losing some [energy](energy.md).

[Fluence](radiometry.md#fluence) is time-integrated [light intensity](wave.md#light-intensity), $F(x,y)=\int I(x,y,t)\,dt$, measured in $\mathrm{J\,m^{-2}}$. For a uniform beam of area $\mathcal A$, $F=U/\mathcal A$ and $I_{\rm pk}=P_{\rm pk}/\mathcal A$. At fixed transverse profile, lossless temporal stretching lowers peak [light intensity](wave.md#light-intensity) but leaves [fluence](radiometry.md#fluence) unchanged. Absorbed [energy](energy.md), heat removal, beam size, coatings and pulse duration still constrain optical components. For nonoverlapping identical pulses at repetition [frequency](wave.md#frequency) $f_r$, the average [power](energy.md#power) is $U f_r$; it is a different quantity from [peak power](energy.md#peak-power).

### Spectral phase in pulse compression

↑ **Parent:** [Chirped pulse amplification](#chirped-pulse-amplification)

Use a complex envelope $A(t)$ normalized so that $|A(t)|^2=P(t)$; its units are $\mathrm{W}^{1/2}$. The optical carrier convention is $e^{-i\omega_0t}$: the physical [electric field](electric-field.md) is proportional to the real part of $A(t)e^{-i\omega_0t}$ for a fixed transverse mode. With [angular frequency](lagrangian-mechanics.md#angular-frequency) offset $\Omega=\omega-\omega_0$, fix the [Fourier transform](fourier-transform.md) convention

$$
\widetilde A(\Omega)=\int_{-\infty}^{\infty}A(t)e^{i\Omega t}\,dt,\qquad
A(t)=\frac{1}{2\pi}\int_{-\infty}^{\infty}\widetilde A(\Omega)e^{-i\Omega t}\,d\Omega.
$$

Write $\widetilde A=B e^{i\phi}$ with real $B\geq0$. A dispersive element adds [spectral phase](physical-optics.md#spectral-phase)

$$
\phi(\Omega)=\phi_0+\phi_1\Omega+\frac{\phi_2}{2}\Omega^2+\frac{\phi_3}{6}\Omega^3+\cdots.
$$

Constant [phase](wave.md#phase-waves) rotates the envelope; the linear term delays it by $\phi_1$. The [group delay](physical-optics.md#group-delay) is $d\phi/d\Omega$. The quadratic coefficient $\phi_2$ is [group delay dispersion](physical-optics.md#group-delay-dispersion), abbreviated GDD, with units of time squared. Positive GDD makes higher [frequencies](wave.md#frequency) arrive later with this convention. It is accumulated dispersion of a component; material [group velocity dispersion](dispersion-relation.md#group-velocity-dispersion) is its corresponding coefficient per unit length.

To undo a quadratic stretcher [spectral phase](physical-optics.md#spectral-phase), the compressor must supply opposite GDD. Include the amplifier and all intervening optics in the sum:

$$
\phi_{2,\rm total}=\phi_{2,\rm stretch}+\phi_{2,\rm amplifier}+\phi_{2,\rm compress}.
$$

Setting this sum to zero does not cancel [third-order dispersion](physical-optics.md#third-order-dispersion), $\phi_3$, or still higher orders. Residual [spectral phase](physical-optics.md#spectral-phase) can produce asymmetry and satellite pulses even when the quadratic term vanishes. A [diffraction grating](physical-optics.md#diffraction-grating) system can make path length depend on [frequency](wave.md#frequency); matching the complete [spectral phase](physical-optics.md#spectral-phase) over the occupied spectrum is more demanding than merely choosing opposite quadratic coefficients.

There is a useful proof of what phase correction can accomplish. By [Parseval's identity](fourier-analysis.md#parseval-identity),

$$
U=\int |A|^2\,dt=\frac{1}{2\pi}\int B^2\,d\Omega.
$$

For a smooth decaying spectrum, the [Fourier transform](fourier-transform.md) of $tA$ is $-i\,d\widetilde A/d\Omega$. Consequently the power-weighted mean arrival time and [variance](variance.md) obey

$$
\bar t=\frac{\int B^2\phi'\,d\Omega}{\int B^2\,d\Omega},\qquad
\sigma_t^2=\frac{\int (B')^2\,d\Omega}{\int B^2\,d\Omega}
+\frac{\int B^2(\phi'-\bar t)^2\,d\Omega}{\int B^2\,d\Omega}.
$$

At fixed spectral amplitude, constant [group delay](physical-optics.md#group-delay) minimizes this [root mean square](analysis.md#root-mean-square) duration. Such a pulse is a [transform-limited pulse](optics.md#transform-limited-pulse), up to a time shift and constant [phase](wave.md#phase-waves). The nonnegative second term measures temporal broadening from unequal arrival times; the first term remains even after perfect phase correction.

### Gaussian chirped pulse compression

↑ **Parent:** [Chirped pulse amplification](#chirped-pulse-amplification)

Choose an initially [transform-limited pulse](optics.md#transform-limited-pulse) with Gaussian [power](energy.md#power) and complex envelope

$$
A_0(t)=\sqrt{\frac{U}{\sqrt{2\pi}\sigma_0}}\,e^{-t^2/(4\sigma_0^2)},\qquad
\tau_0=2\sqrt{2\ln2}\,\sigma_0.
$$

Here $\sigma_0$ is the standard deviation of the power-weighted time distribution; $\tau_0$ is its [full width at half maximum](analysis.md#full-width-at-half-maximum). Neither is a field-amplitude width. The spectral amplitude is proportional to $e^{-\sigma_0^2\Omega^2}$, so the spectral power has [standard deviation](variance.md#standard-deviation) $\sigma_\Omega=1/(2\sigma_0)$. The Gaussian [time-bandwidth product](optics.md#time-bandwidth-product) in ordinary [frequency](wave.md#frequency) is $\tau_0\Delta\nu=2\ln2/\pi\simeq0.4413$, where both widths are power FWHMs.

Multiplication by $e^{i\phi_2\Omega^2/2}$ preserves spectral power and [energy](energy.md). Substituting $\phi'=\phi_2\Omega$ into the moment identity gives

$$
\sigma_t^2=\sigma_0^2+\frac{\phi_2^2}{4\sigma_0^2},\qquad
\tau(\phi_2)=\tau_0\sqrt{1+\left(\frac{4\ln2\,\phi_2}{\tau_0^2}\right)^2}.
$$

This is an exact result for a Gaussian spectrum with quadratic [spectral phase](physical-optics.md#spectral-phase). It also follows by completing the square in its inverse [Fourier transform](fourier-transform.md).

<a id="image-phase-cancellation-recovers-a-gaussian-pulse-while-residual-phase-and-narrowed-bandwidth-limit-it"></a>
![](gaussian-chirped-pulse-spectral-phase-compression.png)

**[Figure 8](#image-phase-cancellation-recovers-a-gaussian-pulse-while-residual-phase-and-narrowed-bandwidth-limit-it). Phase cancellation recovers a Gaussian pulse, while residual phase and narrowed bandwidth limit it**. Original complex-envelope [Fast Fourier transform](discrete-fourier-transform.md#fast-fourier-transform) calculations for a chosen $30\,\mathrm{fs}$ power FWHM, $1\,\mathrm{nJ}$ pulse. The stretcher adds $3000\,\mathrm{fs^2}$ of [group delay dispersion](physical-optics.md#group-delay-dispersion). Separate output cases show exact cancellation, $300\,\mathrm{fs^2}$ residual GDD, $20000\,\mathrm{fs^3}$ residual [third-order dispersion](physical-optics.md#third-order-dispersion), and a Gaussian [optical gain](#optical-gain) profile. The finite-gain curve divides out the central-frequency gain $G_0$ and retains the resulting energy change. All curves are calculations, not measured pulse traces.

For these chosen inputs, $\sigma_0=12.7398\,\mathrm{fs}$. The stretched pulse has $\tau=278.88\,\mathrm{fs}$ and [root mean square](analysis.md#root-mean-square) width $118.4282\,\mathrm{fs}$. Adding $-3000\,\mathrm{fs^2}$ recovers $30\,\mathrm{fs}$; leaving $300\,\mathrm{fs^2}$ gives $40.85\,\mathrm{fs}$. All phase-only cases retain $1\,\mathrm{nJ}$.

If GDD is cancelled but $\phi_3=20000\,\mathrm{fs^3}$ remains, the pulse is asymmetric. Gaussian spectral moments give

$$
\bar t=\frac{\phi_3\sigma_\Omega^2}{2},\qquad
\sigma_t^2=\sigma_0^2+\frac{\phi_3^2\sigma_\Omega^4}{2}.
$$

Thus the centroid is $15.4033\,\mathrm{fs}$ and the [root mean square](analysis.md#root-mean-square) duration is $25.2354\,\mathrm{fs}$. Converting this last value to a FWHM with the Gaussian factor would be wrong: the power envelope is no longer Gaussian. The calculation's integrated [energy](energy.md) agrees in time and [frequency](wave.md#frequency) through [Parseval's identity](fourier-analysis.md#parseval-identity), while its centroid and [variance](variance.md) agree with these independent moment formulas.

A real amplifier also changes spectral amplitude. For a simple small-signal example, stipulate an intensity gain profile

$$
G(\Omega)=G_0 e^{-\Omega^2/(2\sigma_g^2)},\qquad
\widetilde A_{\rm amplified}=\sqrt{G(\Omega)}\,\widetilde A_{\rm input}.
$$

This specifies finite [gain bandwidth](#gain-bandwidth), with no saturation or extra amplifier [phase](wave.md#phase-waves). Multiplying two Gaussian spectra gives

$$
\frac{1}{\sigma_{\Omega,\rm out}^2}=\frac{1}{\sigma_\Omega^2}+\frac{1}{\sigma_g^2}.
$$

For chosen $\sigma_g=\sigma_\Omega$, the amplified spectrum is narrower by $\sqrt2$, the shortest Gaussian power FWHM becomes $30\sqrt2=42.43\,\mathrm{fs}$, and the total [energy](energy.md) is $G_0U/\sqrt2$. Perfect [spectral phase](physical-optics.md#spectral-phase) correction cannot recreate the suppressed spectral amplitude. Real [gain narrowing](#gain-narrowing) and saturation require a material-dependent amplifier model; a constant multiplier is only a limited idealization. [Gérard Mourou](physicist.md#gerard-mourou)'s 2018 lecture discusses [gain narrowing](#gain-narrowing) as a limit on the shortest amplified pulses.[Extreme Light Physics and Application, p.105, §II.E: finite gain bandwidth and gain narrowing](physics-bibliography.md#extreme-light-physics-and-application-by-gerard-mourou)

### Strickland-Mourou chirped pulse amplification experiment

↑ **Parent:** [Chirped pulse amplification](#chirped-pulse-amplification)

The 1985 experiment launched $150\,\mathrm{ps}$ pulses from a [mode-locked laser](#mode-locked-laser) into $1.4\,\mathrm{km}$ of [optical fiber](optical-instrument.md#optical-fiber). Dispersion and [self-phase modulation](optics.md#self-phase-modulation) produced a broader spectrum and approximately $300\,\mathrm{ps}$ pulses. A Pockels cell selected a pulse for repeated amplification in neodymium glass, giving approximately $2\,\mathrm{mJ}$ before the double-pass [diffraction grating](physical-optics.md#diffraction-grating) compressor. Its transmission was 50 percent. The amplified output was reported as $1\,\mathrm{mJ}$ with a $2\,\mathrm{ps}$ width limited by the streak camera response. The compressor was adjusted on fiber-output pulses using [intensity autocorrelation](optics.md#intensity-autocorrelation); that measurement gave $1.5\,\mathrm{ps}$. [Steve Williamson](physicist.md#steve-williamson) was acknowledged for help developing the concept, and [Philippe Bado](physicist.md#philippe-bado) and [Marcel Bouvier](electrical-engineering.md#marcel-bouvier) for technical support.[pp.219–221, Figs.1–4 and acknowledgments: preparation, compressor adjustment, amplified readout and response limit](physics-bibliography.md#compression-of-amplified-chirped-optical-pulses-by-donna-strickland-and-gerard-mourou)

The crucial comparison is compression before and after amplification. It asks whether enough usable [spectral phase](physical-optics.md#spectral-phase) structure survives the amplifier, rather than merely whether its output is bright. A response-limited trace cannot establish the true width below the detector's resolution or prove that every higher-order phase coefficient vanished. An [intensity autocorrelation](optics.md#intensity-autocorrelation) is also not a direct unique measurement of the complex [electric field](electric-field.md). These are limits on the inference, not extra controls attributed to the experiment.

[Donna Strickland](physicist.md#donna-strickland)'s 2018 lecture describes setting the compressor with the high-repetition oscillator pulses and making the amplified-pulse measurement with [Steve Williamson](physicist.md#steve-williamson)'s streak camera. It explicitly notes imperfect chirp matching.[Generating High-Intensity Ultrashort Optical Pulses, p.168: separate autocorrelation and streak-camera measurements](physics-bibliography.md#generating-high-intensity-ultrashort-optical-pulses-by-donna-strickland) The first apparatus therefore illustrates the strategy without establishing a universal lossless or exactly phase-matched amplifier.

[Donna Strickland](physicist.md#donna-strickland) leads an ultrafast [laser](laser.md) group at Waterloo investigating intense [laser](laser.md) interactions and [nonlinear optics](optics.md#nonlinear-optics).[Biography and research interests: professional appointment and experimental research](physics-bibliography.md#donna-strickland-by-university-of-waterloo) [Gérard Mourou](physicist.md#gerard-mourou)'s later work includes coherent combination of [laser](laser.md) beams in the XCAN project at École polytechnique.[Professor emeritus and XCAN prototype: coherent combination of 61 beams](physics-bibliography.md#the-first-laser-pixels-by-ecole-polytechnique) Their complementary research settings connect the original short-pulse experiment with the continuing problems of producing useful [energy](energy.md), [peak power](energy.md#peak-power) and average [power](energy.md#power) together.

## Attosecond physics

↑ **Parent:** [Laser](laser.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Attosecond_physics)

[Attosecond physics](#attosecond-physics) resolves changes on the scale of $10^{-18}$ [seconds](physics.md#second), especially [electron](physics.md#electron) dynamics. Its central trick is to convert a short optical event into an experimentally accessible [energy](energy.md) or [phase](wave.md#phase-waves) change. A broad [optical spectrum](optics.md#optical-spectrum) provides the ingredients for a short [optical pulse](optics.md#optical-pulse); their [spectral phases](physical-optics.md#spectral-phase) determine when those ingredients add constructively. [High harmonic generation](#high-harmonic-generation) supplies the [optical spectrum](optics.md#optical-spectrum), while [RABBITT](#reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions) and [attosecond streaking](#attosecond-streaking) supply complementary timing measurements. XUV denotes [extreme ultraviolet](optics.md#extreme-ultraviolet) radiation.

There are two separate timing problems: characterize the incident [optical pulse](optics.md#optical-pulse), then infer the response of the target. A [photoelectron](atomic-physics.md#photoelectron) measurement mixes the incident [spectral phase](physical-optics.md#spectral-phase), the target's transition response and the probing [electric field](electric-field.md). Recovering one requires constraints on the others. These methods measure distributions of [photoelectron](atomic-physics.md#photoelectron) [energies](energy.md) over repeated shots, rather than photographing a moving [atomic orbital](chemistry.md#atomic-orbital).

<a id="image-attosecond-generation-and-electron-timing-use-separate-gas-interactions"></a>
![](attosecond-generation-and-electron-readout.png)

**[Figure 9](#image-attosecond-generation-and-electron-timing-use-separate-gas-interactions). Attosecond generation and electron timing use separate gas interactions**. Original functional schematic, not a reproduction of a historical apparatus. The upper path generates and selects short-wavelength radiation; the lower path supplies a delayed reference [electric field](electric-field.md). The analyser converts [photoionization](atomic-physics.md#photoionization) into an [electron spectrometer](optical-instrument.md#electron-spectrometer) readout. The two lower panels distinguish weak-reference two-path [wave interference](physical-optics.md#interference-wave-propagation) from a classical [momentum](momentum.md)-shift idealization.

### High harmonic generation

↑ **Parent:** [Attosecond physics](#attosecond-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/High_harmonic_generation)

[High harmonic generation](#high-harmonic-generation) converts an intense driving [electric field](electric-field.md) into radiation at high integer multiples of its [frequency](wave.md#frequency). [High harmonic generation](#high-harmonic-generation) in a [gas](thermodynamics.md#gas) is a process in [nonlinear optics](optics.md#nonlinear-optics): an [electron](physics.md#electron) can leave a neutral target by [tunnel ionization](atomic-physics.md#tunnel-ionization), gain [kinetic energy](energy.md#kinetic-energy) in the driving [electric field](electric-field.md), and return to radiate upon recombination. This three-step picture is an approximate account of a [probability amplitude](wave-function.md#probability-amplitude) for emission in [quantum mechanics](quantum-mechanics.md), not a measured path of one [electron](physics.md#electron).[Generation and Measurement of Isolated Attosecond Light Pulses, slide 5: tunnelling, acceleration and return](physics-bibliography.md#generation-and-measurement-of-isolated-attosecond-light-pulses-by-michael-hentschel)

Why odd multiples? In an ideal centrosymmetric [gas](thermodynamics.md#gas) driven by a single [frequency](wave.md#frequency), assume the radiating [electric dipole moment](electrostatics.md#electric-dipole-moment) satisfies $d(t+T/2)=-d(t)$, where $T$ is the driving period. Its [Fourier series](fourier-series.md) coefficient obeys $d_q=-(-1)^q d_q$, so every even coefficient vanishes. A finite envelope, an oriented target or an additional driving [frequency](wave.md#frequency) can invalidate that symmetry argument. Producing many odd components also does not prove that their [spectral phases](physical-optics.md#spectral-phase) form a short [optical pulse](optics.md#optical-pulse).

The 1988 report involving [Anne L'Huillier](physicist.md#anne-l’huillier) observed odd multiples of a $1064\,\mathrm{nm}$ driving [wavelength](wave-equation.md#wavelength) in rare gases, reaching order 33 in [argon](chemical-substance.md#argon). The unexpectedly slow fall of yield beyond the fifth order supplied a broad spectral plateau. A spectral observation alone did not establish the relative [spectral phases](physical-optics.md#spectral-phase) needed for an [attosecond pulse train](#attosecond-pulse-train).[Multiple-harmonic conversion of 1064 nm radiation in rare gases, abstract](physics-bibliography.md#multiple-harmonic-conversion-of-1064-nm-radiation-in-rare-gases-by-m-ferray-and-others)

#### Three-step model of high harmonic generation

↑ **Parent:** [High harmonic generation](#high-harmonic-generation)

For an original classical calculation of the return step, neglect the residual [ion](chemistry.md#ion)'s [Coulomb force](electrostatics.md#coulomb-force) after release. Take a spatially uniform driving [electric field](electric-field.md) $E(t)=E_0\cos\omega t$, an [electron](physics.md#electron) of [electric charge](electric-charge.md) $-e$ and [mass](classical-mechanics.md#mass) $m$, and zero initial position and [velocity](classical-mechanics.md#velocity) at $t_i$. With $\alpha=\omega t_i$ and $\beta=\omega t$, integrating [Newton's second law](force.md#newton-s-second-law) gives

$$
v(t)=-\frac{eE_0}{m\omega}(\sin\beta-\sin\alpha),\qquad
x(t)=\frac{eE_0}{m\omega^2}\left[\cos\beta-\cos\alpha+(\beta-\alpha)\sin\alpha\right].
$$

A return requires $\beta>\alpha$ and $x(t)=0$. Define the cycle-averaged free-electron quiver [kinetic energy](energy.md#kinetic-energy)

$$
U_p=\frac{e^2E_0^2}{4m\omega^2},\qquad
K_{\rm return}=2U_p(\sin\beta-\sin\alpha)^2.
$$

Searching the first-return solutions for release phases $0<\alpha<\pi/2$ gives a maximum near $\alpha=0.3134$ and $\beta=4.3990$, with $K_{\rm return}\simeq3.1731U_p$. For a chosen [ionization energy](mathematical-physics.md#ionization-energy) $I_p$, recombination into the initial state can therefore emit a [photon](quantum-mechanics.md#photon) with [energy](energy.md) up to approximately $I_p+3.17U_p$ in this model. This is an upper return-energy scale, not a prediction of the emitted yield. It omits release probabilities, [quantum interference](quantum-system.md#quantum-interference), propagation, [phase matching](physical-optics.md#phase-matching) and depletion of the neutral [gas](thermodynamics.md#gas).

The calculation explains why a long driving [wavelength](wave-equation.md#wavelength) can increase the available return [energy](energy.md): at fixed $E_0$, $U_p$ grows as $\omega^{-2}$. It does not say that conversion efficiency improves. The [electron](physics.md#electron) must return with a [probability amplitude](wave-function.md#probability-amplitude) for emission that survives the microscopic dynamics and adds coherently across the [gas](thermodynamics.md#gas).

### Attosecond pulse train

↑ **Parent:** [Attosecond physics](#attosecond-physics)

An [attosecond pulse train](#attosecond-pulse-train) contains repeated short [optical pulses](optics.md#optical-pulse). For a group of odd multiples of a common driving [frequency](wave.md#frequency), the separation is half the driving period when the relative [spectral phases](physical-optics.md#spectral-phase) recur. The construction resembles [mode locking](#mode-locking), but the participating components come from [high harmonic generation](#high-harmonic-generation), rather than separate resonant modes of a [laser](laser.md) oscillator.

#### Coherent harmonic pulse-train model

↑ **Parent:** [Attosecond pulse train](#attosecond-pulse-train)

Choose $N$ equal-amplitude, monochromatic odd components with orders $q_j=q_0+2j$, $j=0,\ldots,N-1$, and odd $q_0$. Fix the complex-field convention

$$
\mathcal E(t)=a\sum_{j=0}^{N-1}e^{i\phi_j-iq_j\omega t},\qquad I(t)\propto|\mathcal E(t)|^2.
$$

Here $I$ is a normalized [light intensity](wave.md#light-intensity) after averaging the fast carrier oscillations. Setting every $\phi_j=0$ and summing a [geometric series](sequence-and-series.md#geometric-series) gives

$$
\frac{I(t)}{N^2|a|^2}=\left[\frac{\sin(N\omega t)}{N\sin(\omega t)}\right]^2.
$$

At the removable singularities take the continuous limit. Maxima repeat every $T/2=\pi/\omega$; the first zeros on either side of a maximum lie at $t=\pm T/(2N)$. The zero-to-zero width is $T/N$, which is not the [full width at half maximum](analysis.md#full-width-at-half-maximum).

Choose orders $13,15,17,19,21$ and driving [wavelength](wave-equation.md#wavelength) $\lambda=800\,\mathrm{nm}$. Using $T=\lambda/c$ with the [speed of light](special-relativity.md#speed-of-light) $c$ gives $T=2.66851\,\mathrm{fs}$ and burst spacing $1.33426\,\mathrm{fs}$. Solving the exact half-maximum equation gives a [full width at half maximum](analysis.md#full-width-at-half-maximum) of approximately $240.6$ attoseconds. These are values of the specified five-component model, not measurements from the 2001 experiment.

A deliberately chosen [spectral phase](physical-optics.md#spectral-phase) $\phi_q=q\omega t_0$ translates the whole [attosecond pulse train](#attosecond-pulse-train) by $t_0$ without changing its shape. Adding $\kappa(q-17)^2/2$ makes neighboring phase increments unequal: the same component intensities then produce a different temporal profile. For the choice $t_0=0.20\,\mathrm{fs}$ and $\kappa=0.08$ radians per squared harmonic order, the adjacent-component delay estimates are

$$
\frac{\phi_{q+2}-\phi_q}{2\omega}
=t_0+\frac{\kappa(q+1-17)}{\omega},
$$

namely $0.0981$, $0.1660$, $0.2340$ and $0.3019\,\mathrm{fs}$ for $q=13,15,17,19$. This [finite difference](finite-difference.md) estimates the [group delay](physical-optics.md#group-delay) at the pair's midpoint. It is not a single common arrival time.

<a id="image-identical-harmonic-intensities-can-encode-different-pulse-shapes-and-delays"></a>
![](coherent-harmonic-train-and-phase-delays.png)

**[Figure 10](#image-identical-harmonic-intensities-can-encode-different-pulse-shapes-and-delays). Identical harmonic intensities can encode different pulse shapes and delays**. Original idealized calculation for five monochromatic odd components. The top panels compare equal component intensities and the resulting normalized [light intensities](wave.md#light-intensity). The lower panels compare a chosen delay-dependent two-path signal and the [group delays](physical-optics.md#group-delay) recovered from neighboring [spectral phases](physical-optics.md#spectral-phase). All values are stipulated model inputs or calculated outputs; none are experimental traces.

The infinite monochromatic sum is periodic forever and has infinite total [energy](energy.md). A real [attosecond pulse train](#attosecond-pulse-train) has a finite envelope and finite component linewidths. This calculation isolates coherent addition; it cannot describe an isolated burst or establish its contrast against satellites. As a further check, averaging $I(t)$ over one half-period gives $N|a|^2$ for any constant component [spectral phases](physical-optics.md#spectral-phase), because the cross terms integrate to zero by [Fourier orthogonality](fourier-series.md#fourier-orthogonality). [Spectral phase](physical-optics.md#spectral-phase) redistributes the [light intensity](wave.md#light-intensity) in time while leaving that average fixed.

### Isolated attosecond pulse

↑ **Parent:** [Attosecond physics](#attosecond-physics)

An [isolated attosecond pulse](#isolated-attosecond-pulse) has one dominant short burst within the observation window, with any satellite emission quantified. A broad [optical spectrum](optics.md#optical-spectrum) alone cannot distinguish one burst from several. Selecting a generation interval and an appropriate spectral band can suppress neighboring bursts, but the resulting temporal contrast must still be tested.

For a simple calculation independent of any apparatus, let $\mathcal E(t)=f(t)+r e^{i\theta}f(t-\Delta)$, with two nonoverlapping copies of a short [optical pulse](optics.md#optical-pulse). Its [optical spectrum](optics.md#optical-spectrum) has intensity

$$
|\widetilde{\mathcal E}(\Omega)|^2
=|\widetilde f(\Omega)|^2\left[1+r^2+2r\cos(\Omega\Delta+\theta)\right].
$$

A satellite produces spectral fringes of angular spacing $2\pi/\Delta$ when the two bursts are coherent and resolved. For chosen field-amplitude ratio $r=0.2$, the satellite/main [energy](energy.md) ratio is $r^2=0.04$, while fringe visibility is $2r/(1+r^2)\simeq0.3846$. Weak satellite [energy](energy.md) can thus leave substantial fringes. Averaging an uncontrolled $\theta$ removes the interference term without removing the satellite: absence of fringes alone does not prove isolation.

### Reconstruction of attosecond beating by interference of two-photon transitions

↑ **Parent:** [Attosecond physics](#attosecond-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reconstruction_of_attosecond_beating_by_interference_of_two-photon_transitions)

[RABBITT](#reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions) measures adjacent harmonic [spectral phases](physical-optics.md#spectral-phase) through two-photon [photoionization](atomic-physics.md#photoionization). A weak delayed [infrared](optics.md#infrared) reference opens two interfering paths to a shared [photoelectron](atomic-physics.md#photoelectron) [energy](energy.md); the [two-path attosecond phase reconstruction](#two-path-attosecond-phase-reconstruction) spells out the inference.

#### Two-path attosecond phase reconstruction

↑ **Parent:** [Reconstruction of attosecond beating by interference of two-photon transitions](#reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions)

An original two-amplitude model makes the timing inference explicit. Use the [spectral phase](physical-optics.md#spectral-phase) convention of the [coherent harmonic pulse-train model](#coherent-harmonic-pulse-train-model), and define positive delay $\tau$ to retard the reference [electric field](electric-field.md). Let the amplitudes leading to the same final [photoelectron](atomic-physics.md#photoelectron) state be

$$
M_-(\tau)=b_-e^{i(\phi_{q-1}+\omega\tau+\eta_-)},\qquad
M_+(\tau)=b_+e^{i(\phi_{q+1}-\omega\tau+\eta_+)},
$$

with real $b_\pm\geq0$. Squaring their sum gives

$$
S_q(\tau)=b_-^2+b_+^2+2b_-b_+\cos(2\omega\tau-\Delta\phi_q+\delta_q),
\qquad \Delta\phi_q=\phi_{q+1}-\phi_{q-1},\quad\delta_q=\eta_--\eta_+.
$$

The $2\omega$ oscillation comes from opposite signs of the reference [photon](quantum-mechanics.md#photon)'s [phase](wave.md#phase-waves). For $\Delta\phi_q=2\omega t_0$ and $\delta_q=0$, the signal peaks at $\tau=t_0$ modulo $T/2$. A fitted phase contains the target contribution $\delta_q$; setting it to zero is an assumption, not an observation. In an experiment, unobserved final channels can add as probabilities, so the displayed formula is one effective-channel idealization.

For a chosen example, impose $\Delta\phi_q=0.80$ radians and $\delta_q=0.15$ radians at $800\,\mathrm{nm}$. The observed oscillation has argument $2\omega\tau-0.65$. Its peak shift is $0.1380\,\mathrm{fs}$, while the corrected finite-difference [group delay](physical-optics.md#group-delay) is $\Delta\phi_q/(2\omega)=0.1699\,\mathrm{fs}$. Ignoring the target contribution would bias the inferred delay by $-31.9$ attoseconds. These stipulated phases demonstrate a reconstruction error; they are not atomic calculations or measured delays.

Recovering all neighboring phase differences determines the component [spectral phases](physical-optics.md#spectral-phase) up to an overall [phase](wave.md#phase-waves) and the chosen timing origin, provided the oscillation phases are consistently unwrapped. Known component amplitudes then give a temporal field by a finite inverse [Fourier transform](fourier-transform.md). This is why measuring the [optical spectrum](optics.md#optical-spectrum) alone is insufficient: it omits the very information that decides when constructive [wave interference](physical-optics.md#interference-wave-propagation) occurs.

#### 2001 attosecond pulse-train experiment

↑ **Parent:** [Reconstruction of attosecond beating by interference of two-photon transitions](#reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions)

[Pierre Agostini](physicist.md#pierre-agostini)'s experiment illuminated an [argon](chemical-substance.md#argon) jet with an annular $800\,\mathrm{nm}$ beam. A pinhole removed the annulus; a tungsten-coated mirror relayed harmonics and weak central reference into another [argon](chemical-substance.md#argon) jet. A magnetic-bottle [electron spectrometer](optical-instrument.md#electron-spectrometer) used [time of flight](particle-detection.md#time-of-flight) and [microchannel plate detectors](tensor-product-of-quantum-systems.md#microchannel-plate-detector). Glass plates varied delay. Reference-on sidebands contrasted with reference-off peaks. Atomic-phase-corrected reconstruction yielded $250$-attosecond bursts.[pp.1690–1691, Figs.1–4 and Table 1](physics-bibliography.md#observation-of-a-train-of-attosecond-pulses-from-high-harmonic-generation-by-p-m-paul-and-others)

The [two-path attosecond phase reconstruction](#two-path-attosecond-phase-reconstruction) explains the control's purpose: adding the reference opens an interference channel. Its fitted oscillation tests phase relationships under the weak-field and atomic-response model. It does not independently reveal every target phase or an arbitrary nonperiodic [optical pulse](optics.md#optical-pulse).

### Attosecond streaking

↑ **Parent:** [Attosecond physics](#attosecond-physics)

[Attosecond streaking](#attosecond-streaking) uses a synchronized reference [electric field](electric-field.md) to change a [photoelectron](atomic-physics.md#photoelectron)'s outgoing [momentum](momentum.md). Scanning relative delay produces an [energy](energy.md)-versus-delay distribution. A short emission interval samples only a small part of the reference cycle; a longer interval samples a range of kicks and can broaden or reshape the distribution.

For an explicit classical limit, use the [electric dipole](electrostatics.md#electric-dipole) approximation and choose the [magnetic vector potential](electromagnetism.md#magnetic-vector-potential) $A(t)$ along the detection axis with $E(t)=-dA/dt$ and $A(\infty)=0$. Neglect the residual [ion](chemistry.md#ion)'s [Coulomb force](electrostatics.md#coulomb-force). An [electron](physics.md#electron) released at $t_i$ with mechanical [momentum](momentum.md) $p_0$ obeys

$$
p_f=p_0-eA(t_i),\qquad
K_f=\frac{[p_0-eA(t_i)]^2}{2m}.
$$

Indeed, integrating $\dot p=-eE=e\dot A$ from release to the end of the field gives the stated minus sign. The useful clock variable here is $A$, rather than the instantaneous $E$ itself. If $A$ is nearly linear across a narrow emission window with temporal [standard deviation](variance.md#standard-deviation) $\sigma_t$, and initial [momentum](momentum.md) is sharp, then

$$
\sigma_p\simeq e|E(t_i)|\sigma_t.
$$

This local mapping fails near a zero of $E$, where first-order timing sensitivity vanishes. A real inversion must include the incident bandwidth, initial [photoelectron](atomic-physics.md#photoelectron) distribution, collection angles and target–field response.

For an original dimensionless example in [atomic units](physics.md#atomic-units), choose $p_0=2$, $m=e=1$ and $A(t_i)=0.10$. Then $p_f=1.9$ and $K_f=1.805$, compared with initial [kinetic energy](energy.md#kinetic-energy) $2$. Reversing $A$ gives $K_f=2.205$: the shifts are asymmetric because of the $A^2/2$ term. A measurement that keeps only the term linear in $A$ would miss $0.005$ in both cases.

#### 2001 isolated attosecond pulse experiment

↑ **Parent:** [Attosecond streaking](#attosecond-streaking)

The experiment involving [Ferenc Krausz](physicist.md#ferenc-krausz) combined a subfemtosecond soft-[X-ray](electromagnetic-radiation.md#x-ray) pulse with a few-cycle visible [electric field](electric-field.md). Its delay-dependent [krypton](chemical-substance.md#krypton) [photoelectron](atomic-physics.md#photoelectron) spectra tested the field-controlled response. The reported pulse duration was $650\pm150$ attoseconds. Changing delay compared the emitted [electron](physics.md#electron) distributions at different reference phases; the spectral-width trace supplied a further duration-sensitive observable.[Attosecond metrology, abstract and Figs.3–5: krypton spectra, delay scan and width](physics-bibliography.md#attosecond-metrology-by-michael-hentschel-and-others)

The distinction from [RABBITT](#reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions) is the measurement regime and reconstruction, rather than merely calling one trace a clock. The [attosecond streaking](#attosecond-streaking) [momentum](momentum.md) map is a limiting model; a finite-duration [wave packet](dispersion-relation.md#wave-packet) requires a quantum transition calculation. Inferring an emission delay also requires separating the illuminating pulse's [spectral phase](physical-optics.md#spectral-phase) from the target response. The measurement supports time-dependent [photoionization](atomic-physics.md#photoionization) in a specified model, with no unique classical [electron](physics.md#electron) trajectory inside an [atomic orbital](chemistry.md#atomic-orbital) implied.

## ↑ Ancestors (4)

1. [Optics](optics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (100)

- [Ashkin radiation-pressure trapping experiment](optics.md#ashkin-radiation-pressure-trapping-experiment)
- [Atom-cloud gravity-gradient measurement](newton-s-law-of-universal-gravitation.md#atom-cloud-gravity-gradient-measurement)
- [Attosecond pulse train](#attosecond-pulse-train)
- [Circular-aperture diffraction laboratory experiment](point-spread-function.md#circular-aperture-diffraction-laboratory-experiment)
- [Coherent beam splitter recombination](optical-instrument.md#coherent-beam-splitter-recombination)
- [Cold-atom collapse and revival after a lattice quench](quantum-mechanics.md#cold-atom-collapse-and-revival-after-a-lattice-quench)
- [Comb tooth index ambiguity](#comb-tooth-index-ambiguity)
- [Conjugate pinholes in confocal microscopy](fluorescence.md#conjugate-pinholes-in-confocal-microscopy)
- [Continuous double heterostructure laser experiment](semiconductor.md#continuous-double-heterostructure-laser-experiment)
- [Cryogenic laser-power substitution experiment](radiometry.md#cryogenic-laser-power-substitution-experiment)
- [Digital optical phase conjugation](physical-optics.md#digital-optical-phase-conjugation)
- [Donna Strickland](physicist.md#donna-strickland)
- [Doppler cooling](atomic-physics.md#doppler-cooling)
- [Doppler-Free Two-Photon Spectroscopy of Hydrogen by Theodor W. Hänsch and others](physics-bibliography.md#doppler-free-two-photon-spectroscopy-of-hydrogen-by-theodor-w-hansch-and-others)
- [Dragged-bead fluctuation theorem experiment](stochastic-thermodynamics.md#dragged-bead-fluctuation-theorem-experiment)
- [Dye laser](#dye-laser)
- [Electric dipole](electrostatics.md#electric-dipole)
- [Equipartition theorem](canonical-ensemble.md#equipartition-theorem)
- [Exciton absorption experiment in copper(I) oxide](quantum-mechanics.md#exciton-absorption-experiment-in-copper-i-oxide)
- [Experimental inputs to electronegativity scales](electronegativity.md#experimental-inputs-to-electronegativity-scales)
- [Fermionic atom antibunching](tensor-product-of-quantum-systems.md#fermionic-atom-antibunching)
- [Finite-well confinement in a semiconductor heterostructure](semiconductor.md#finite-well-confinement-in-a-semiconductor-heterostructure)
- [Flow cytometry](biology.md#flow-cytometry)
- [Fluorescence lifetime measurement with pulsed excitation](fluorescence.md#fluorescence-lifetime-measurement-with-pulsed-excitation)
- [Fluorescent bead experiment for confocal microscopy](fluorescence.md#fluorescent-bead-experiment-for-confocal-microscopy)
- [FRET proximity readout experiment](biology.md#fret-proximity-readout-experiment)
- [Gaussian beam](physical-optics.md#gaussian-beam)
- [Gérard Mourou](physicist.md#gerard-mourou)
- [Gérard Roger](engineering.md#gerard-roger)
- [Helium-neon laser](#helium-neon-laser)
- [Kinetochore ablation experiment](cell-cycle.md#kinetochore-ablation-experiment)
- [Laser](laser.md)
- [Laser cooling](atomic-physics.md#laser-cooling)
- [Laser detuning](#laser-detuning)
- [Laser-diffraction measurement of capillary waves](surface-tension.md#laser-diffraction-measurement-of-capillary-waves)
- [Laser flash analysis](heat.md#laser-flash-analysis)
- [Laser spectroscopy](atomic-physics.md#laser-spectroscopy)
- [LIGO differential strain measurement](gravitational-wave.md#ligo-differential-strain-measurement)
- [LIGO displacement readout and control](gravitational-wave.md#ligo-displacement-readout-and-control)
- [Lower-level depopulation in a four-level laser](#lower-level-depopulation-in-a-four-level-laser)
- [Lunar laser ranging](energy.md#lunar-laser-ranging)
- [Michelson interferometer](physical-optics.md#michelson-interferometer)
- [Mode-locked laser](#mode-locked-laser)
- [Mode locking](#mode-locking)
- [Mollow triplet](quantum-system.md#mollow-triplet)
- [Motional sideband](atomic-physics.md#motional-sideband)
- [Near-field diffraction laboratory experiment](physical-optics.md#near-field-diffraction-laboratory-experiment)
- [Nitrogen dissociation threshold from fragment images](chemical-bond.md#nitrogen-dissociation-threshold-from-fragment-images)
- [Nobel Prize in Physics in 1964](nobel-prize-in-physics.md#nobel-prize-in-physics-in-1964)
- [Nobel Prize in Physics in 1997](nobel-prize-in-physics.md#nobel-prize-in-physics-in-1997)
- [Nonlinear optics](optics.md#nonlinear-optics)
- [Off-axis holography](physical-optics.md#off-axis-holography)
- [Optical dipole trap](atomic-physics.md#optical-dipole-trap)
- [Optical fiber coupling and bend experiment](optical-instrument.md#optical-fiber-coupling-and-bend-experiment)
- [Optical fiber purity and low-loss transmission](optical-instrument.md#optical-fiber-purity-and-low-loss-transmission)
- [Optical frequency comb](#optical-frequency-comb)
- [Optical frequency measurement with a comb](#optical-frequency-measurement-with-a-comb)
- [Optical molasses](atomic-physics.md#optical-molasses)
- [Optical molasses experiment of 1985](atomic-physics.md#optical-molasses-experiment-of-1985)
- [Optical path length](physical-optics.md#optical-path-length)
- [Optical pumping](atomic-physics.md#optical-pumping)
- [Optical tweezers](optics.md#optical-tweezers)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2014/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-genetics-course-of-the-university-of-cambridge/2024/paper-2.md#5/solution)
- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2015/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2017.md#1/b/solution)
- [Solution](past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2013/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-2.md#section-b/b8/solution)
- [Solution](past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2012/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-2.md#6/i/solution)
- [Photodetachment threshold](electronegativity.md#photodetachment-threshold)
- [Photodiode responsivity measurement](optical-instrument.md#photodiode-responsivity-measurement)
- [Pierre Agostini](physicist.md#pierre-agostini)
- [Point spread function](point-spread-function.md)
- [Polarization preparation and dephasing experiment](quantum-system.md#polarization-preparation-and-dephasing-experiment)
- [Population inversion](#population-inversion)
- [Radiation-pressure laser power measurement](pressure.md#radiation-pressure-laser-power-measurement)
- [Raman effective Rabi frequency](atomic-physics.md#raman-effective-rabi-frequency)
- [Raman spectroscopy](optics.md#raman-spectroscopy)
- [Rayleigh criterion](point-spread-function.md#rayleigh-criterion)
- [Saturation spectroscopy preparation and detector readout](atomic-physics.md#saturation-spectroscopy-preparation-and-detector-readout)
- [Scanning Fabry–Pérot measurement](optical-instrument.md#scanning-fabry-perot-measurement)
- [Single-beam gradient trapping experiment](optics.md#single-beam-gradient-trapping-experiment)
- [Single-mode optical fiber](optical-instrument.md#single-mode-optical-fiber)
- [Single-molecule absorption in a molecular crystal](molecule.md#single-molecule-absorption-in-a-molecular-crystal)
- [Stimulated emission](#stimulated-emission)
- [Stirling engine](thermodynamics.md#stirling-engine)
- [Strickland-Mourou chirped pulse amplification experiment](#strickland-mourou-chirped-pulse-amplification-experiment)
- [Thermal calibration of an optical trap](optics.md#thermal-calibration-of-an-optical-trap)
- [Total internal reflection](electromagnetic-wave.md#total-internal-reflection)
- [Trapped-ion quantum control](atomic-physics.md#trapped-ion-quantum-control)
- [Willard Sterling Boyle](physicist.md#willard-sterling-boyle)
- [Zeeman slower](atomic-physics.md#zeeman-slower)
- [Zeeman splitting](atomic-physics.md#zeeman-splitting)
