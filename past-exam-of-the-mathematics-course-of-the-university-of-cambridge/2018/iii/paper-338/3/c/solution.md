<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [H2RG detector](../../../../../../h2rg-detector.md) is a [hybrid infrared detector](../../../../../../hybrid-infrared-detector.md): a photosensitive array is bonded, pixel by pixel through indium contacts, to a separate silicon readout circuit. In infrared use the absorber is normally [mercury cadmium telluride](../../../../../../mercury-cadmium-telluride.md), whose composition sets the absorption cutoff. The H2RG readout architecture can also be used with other absorbing materials, so the readout name does not fix the detector’s wavelength response. The [manufacturer’s H2RG specification](https://www.teledyne-si.com/en-us/Products-and-Services_/Documents/Infrared%20and%20Visible%20FPAs/TSI-0855%20H2RG%20Brochure-25Feb2022.pdf) gives a $2048\times2048$ grid and $18\,\mu\mathrm m$ pixel pitch, together with reference-pixel and guide-window capabilities.

Each illuminated pixel contains a [photodiode](../../../../../../photodiode.md) connected to its own readout node. Absorbed photons generate carriers; their accumulated charge changes the node voltage, with $|\Delta V|=|\Delta Q|/C$ for node [capacitance](../../../../../../capacitance.md) $C$. A reset establishes the baseline; row and column addressing and multiplexed output amplifiers sample the pixel voltage. This is not the serial transfer of charge packets through adjacent pixels used by a [charge-coupled device](../../../../../../charge-coupled-device.md).

[Nondestructive detector readout](../../../../../../nondestructive-detector-readout.md) allows repeated measurements during an integration. [Correlated double sampling](../../../../../../correlated-double-sampling.md) removes the reset baseline, [Fowler sampling](../../../../../../fowler-sampling.md) differences groups of reads at the beginning and end, and [up-the-ramp sampling](../../../../../../up-the-ramp-sampling.md) estimates the signal from its slope and can flag cosmic-ray steps or saturation. The “R” denotes [detector reference pixels](../../../../../../detector-reference-pixel.md), which monitor electronic offsets; “G” denotes a programmable guide window that can be read rapidly between full-array operations. Reference pixels do not measure sky background. Cooling suppresses [dark current](../../../../../../dark-current-physics.md) and thermal background. [Read noise](../../../../../../read-noise.md), nonlinearity, persistence and interpixel coupling still require calibration.

**An independently addressed hybrid photodiode array integrates charge and permits nondestructive voltage reads, reference correction and rapid guide-window sampling.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 338](../../../paper-338-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
