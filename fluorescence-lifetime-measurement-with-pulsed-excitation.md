# Fluorescence lifetime measurement with pulsed excitation

↑ **Parent:** [Time-correlated single-photon counting](time-correlated-single-photon-counting.md)

The inspected apparatus sends picosecond diode-[laser](laser.md) pulses into a sample cuvette. A neutral attenuation filter keeps detected events rare; an emission cut-off filter rejects scattered excitation. Collection optics deliver [fluorescence](fluorescence.md) to a [photodetector](photodetector.md); detector pulses and the laser-driver synchronization signal feed the timing electronics. The illustrated arrangement uses a PDL 800-B driver and TimeHarp 200 electronics. The note's recorded comparison uses two dye solutions and a prompt instrument-response trace; the dye tails have distinct slopes on a logarithmic display. Its Figure 9 measurement specifies an 80 MHz source, separately from the Figure 8 driver-setting example.[Michael Wahl, Time-Correlated Single Photon Counting, v. 2.1, pp. 7–9, Figures 8–9: cuvette/filter/detector setup; Toluidine Blue and Oxazin 4 curves; explicit 80 MHz measurement setting](time-correlated-single-photon-counting-technical-note-v-2-1-by-michael-wahl.md)

For a defensible new measurement, separately acquire detector background with excitation blocked, a solvent/container blank under excitation, and a prompt response appropriate to the timing channel. Compare successively attenuated acquisitions to expose pile-up; compare early and late acquisition intervals to expose [photobleaching](photobleaching.md). Choose a repetition period long enough for the relevant decay or include residual population from earlier pulses in the model. These are proposed checks, not additional controls claimed for the published curves. [Photon shot noise](photon-shot-noise.md), background mismatch, and uncertainty in the [fluorescence instrument response](fluorescence-instrument-response.md) limit how uniquely multiple decay components can be inferred.

## ↑ Ancestors (8)

1. [Time-correlated single-photon counting](time-correlated-single-photon-counting.md)
2. [Fluorescence lifetime](fluorescence-lifetime.md)
3. [Fluorescence](fluorescence.md)
4. [Physical optics](physical-optics.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
