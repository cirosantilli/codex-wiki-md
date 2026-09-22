<h1 id="section-d/d9/solution">Solution</h1>

↑ **Parent:** [D9](../d9.md)

The [photoelectric effect](../../../../../photoelectric-effect.md), [black-body radiation](../../../../../black-body-radiation.md) and the [Davisson–Germer experiment](../../../../../davisson-germer-experiment.md) challenge different parts of a fully classical picture. Classical [electromagnetic waves](../../../../../electromagnetic-wave-split.md) successfully describe propagation, [interference](../../../../../interference-wave-propagation.md) and [diffraction](../../../../../diffraction.md), while classical particles follow trajectories determined by forces. The difficulty is combining that picture with the observed exchange of energy between radiation and matter, the equilibrium distribution of radiation, and electron scattering. The three experiments expose the roles of discrete energy exchange and coherent [matter waves](../../../../../matter-wave.md).

In a [photoelectric effect](../../../../../photoelectric-effect.md) experiment, monochromatic light illuminates a metal cathode in vacuum and a second electrode collects emitted [electrons](../../../../../electron.md). Varying the collecting voltage measures a [photocurrent](../../../../../photocurrent.md); reversing it until collection ceases determines the [stopping potential](../../../../../stopping-potential.md). The observations distinguish two controls: at fixed frequency above threshold, increasing [light intensity](../../../../../light-intensity.md) increases the emission rate, whereas the largest emitted [kinetic energy](../../../../../kinetic-energy.md) is determined mainly by frequency. There is a material-dependent [photoelectric threshold frequency](../../../../../photoelectric-threshold-frequency.md), and emission above threshold does not require the long charging-up delay predicted by a simple picture of gradual classical energy accumulation at low intensity.

A classical wave carries continuously distributed energy, with intensity proportional to squared field amplitude. On a fully classical absorption picture, increasing intensity would be expected to increase the energy delivered to an electron, and sufficiently long exposure could accumulate the escape energy even below the observed threshold. It does not naturally produce the measured universal straight-line relation between stopping potential and light frequency. In 1905, [Albert Einstein](../../../../../albert-einstein.md) instead treated light-energy transfer as localized quanta. His argument distinguished the fastest escaping [electrons](../../../../../electron.md) from electrons losing energy before escape.[§8, printed pp. 193–196, energy balance and frequency versus intensity predictions](../../../../../einstein-s-miraculous-year/on-a-heuristic-point-of-view-concerning-the-production-and-transformation-of-light-by-albert-einstein.md)

In the single-[photon](../../../../../photon.md) regime, [conservation of energy](../../../../../conservation-of-energy.md) gives the [Einstein photoelectric equation](../../../../../einstein-photoelectric-equation.md)

$$
\boxed{K_{\max}=h\nu-\Phi=eV_s,\qquad\nu_0=\frac\Phi h,}
$$

where $\Phi$ is the surface [work function](../../../../../work-function.md). The photon supplies energy $h\nu$; the escape cost is paid first, and the remainder sets the upper electron-energy edge. Increasing intensity at fixed frequency increases the number of available [photons](../../../../../photon.md), so it raises current without raising this edge. Below $\nu_0$, one photon cannot pay the escape cost. In an actual measurement, stable surface preparation, suppression of unwanted higher-frequency light, and the [photoelectric contact-potential correction](../../../../../photoelectric-contact-potential-correction.md) are needed to test the slope $h/e$ reliably. [Robert Andrews Millikan](../../../../../robert-andrews-millikan.md)'s experiment used selected mercury spectral lines, freshly exposed metal surfaces and an electrometer to make such a quantitative test.[§§2–4, printed pp. 361–375, apparatus and stopping-potential measurements](../../../../../a-direct-photoelectric-determination-of-planck-s-h-by-robert-andrews-millikan.md) The interpretation is for weak single-photon illumination; [multiphoton photoemission](../../../../../multiphoton-photoemission.md) at sufficiently intense fields is a different regime.

[Black-body radiation](../../../../../black-body-radiation.md) tests equilibrium physics rather than the escape of individual electrons. A small aperture in an isothermal absorbing cavity approximates an ideal [blackbody](../../../../../blackbody.md): radiation entering the hole undergoes repeated interactions with the walls, and the equilibrium spectrum depends on [temperature](../../../../../temperature-split.md) rather than wall material. A spectrally resolving detector outside the aperture measures how emitted power varies with frequency or wavelength. Experimentally the spectrum has a finite peak, is strongly suppressed at short wavelengths, shifts toward shorter wavelengths when the cavity is heated, and has integrated emission proportional to $T^4$.

For a large cavity, the [electromagnetic mode density in a box](../../../../../electromagnetic-mode-density-in-a-box.md), including two independent transverse polarizations, is $g(\nu)=8\pi\nu^2/c^3$ per volume per unit frequency. The classical [equipartition theorem](../../../../../equipartition-theorem.md) assigns mean energy $k_BT$ to each mode, leading to the [Rayleigh-Jeans law](../../../../../rayleigh-jeans-law.md)

$$
u_\nu^{\mathrm{classical}}=\frac{8\pi k_BT\nu^2}{c^3}.
$$

This agrees at low frequencies but diverges as frequency increases; integrating it over all frequencies gives infinite energy density at any nonzero temperature. This is the [ultraviolet catastrophe](../../../../../ultraviolet-catastrophe.md), a failure of classical equipartition applied to the electromagnetic modes.

[Max Planck](../../../../../max-planck.md)'s essential modification was that energy at a frequency is exchanged in units $h\nu$. In a modern oscillator description, the thermal excitation levels are $nh\nu$, $n=0,1,\ldots$. Using the [Boltzmann distribution](../../../../../boltzmann-distribution.md) and summing a [geometric series](../../../../../geometric-series.md) gives

$$
Z=\sum_{n=0}^\infty e^{-nh\nu/(k_BT)}=\frac1{1-e^{-h\nu/(k_BT)}},\qquad
\langle E\rangle=\frac{h\nu}{e^{h\nu/(k_BT)}-1}.
$$

Multiplying by the mode density yields [Planck's law](../../../../../planck-s-law.md) for the spectral energy density,

$$
\boxed{u_\nu(T)=\frac{8\pi h\nu^3}{c^3}\frac1{e^{h\nu/(k_BT)}-1}.}
$$

When $h\nu\ll k_BT$, expansion of the denominator recovers the classical law. When $h\nu\gg k_BT$, the large excitation cost suppresses occupancy exponentially, removing the divergence. Its integral gives the [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md), while its peak gives [Wien's displacement law](../../../../../wien-s-displacement-law.md). Thus quantization repairs the spectral shape, total emission and temperature dependence together. The displayed thermal energy excludes the oscillator's temperature-independent [zero-point energy](../../../../../zero-point-energy.md).

The [Davisson–Germer experiment](../../../../../davisson-germer-experiment.md) supplies the complementary evidence that matter cannot always be treated as classical particles with definite scattering trajectories. In 1927, [Clinton J. Davisson](../../../../../clinton-davisson.md) and [Lester Halbert Germer](../../../../../lester-halbert-germer.md) sent a narrow, accelerated electron beam normally onto a single [nickel](../../../../../nickel.md) crystal in vacuum. A movable collector measured the current of scattered [electrons](../../../../../electron.md) as direction and accelerating voltage were varied; a retarding potential selected electrons retaining approximately the incident energy. Sharp angular beams depended on crystal orientation and beam energy, with a prominent feature near $54\,\mathrm V$ and detector colatitude $50^\circ$. These are scattering directions and currents, not photographs of electron paths.[Printed pp. 707–710, apparatus; pp. 715–719, voltage and angular scans](../../../../../diffraction-of-electrons-by-a-crystal-of-nickel-by-c-davisson-and-l-h-germer.md)

The [de Broglie wavelength](../../../../../de-broglie-wavelength.md) predicts

$$
\boxed{\lambda=\frac hp=\frac{h}{\sqrt{2m_e eU}}.}
$$

At $U=54\,\mathrm V$, this gives $\lambda\simeq0.167\,\mathrm{nm}$, comparable to atomic spacings. A crystalline arrangement supplies regularly spaced scattering sites, so scattered [probability amplitudes](../../../../../probability-amplitude.md) can add constructively in selected directions. For a suitable family of crystal planes, [Bragg's law](../../../../../bragg-s-law.md) expresses the condition as $2d\sin\theta_B=n\lambda$, with $\theta_B$ measured relative to those planes. The detector colatitude is not automatically this angle. The measured angular structure and its variation with electron momentum are described by [electron diffraction](../../../../../electron-diffraction.md) with the de Broglie wavelength. A classical point-particle deflection model has no phase wavelength $h/p$ and does not supply that interference condition.

The common quantum account preserves the successes of wave propagation and particle detection while changing what is quantized. [Photons](../../../../../photon.md) exchange energy in frequency-dependent units; a thermal distribution of those excitations gives the blackbody spectrum. [Electrons](../../../../../electron.md) have a [wavefunction](../../../../../wave-function-split.md) whose amplitudes interfere on scattering from a crystal, while detection transfers localized charge. The [Born rule](../../../../../born-rule.md) turns squared amplitudes into event probabilities. These results invalidate a fully classical description of matter and radiation; the photoelectric energy law alone does not establish every property of a quantized electromagnetic field, but the three phenomena together provide complementary evidence for the quantum description.

## ↑ Ancestors (14)

1. [D9](../d9.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
