# Frequency modulation laboratory

↑ **Parent:** [Frequency modulation](frequency-modulation.md)

The New Jersey Institute of Technology's _Lab 2: FM Modulation, Demodulation and Bessel Zeros_, Part I, prepares a [voltage-controlled oscillator](voltage-controlled-oscillator.md) in low-frequency mode. A [frequency counter](frequency-counter.md) reads its output while a buffered constant [electric potential difference](electric-potential-difference.md) calibrates its sensitivity. Sweeping the control voltage checks [linearity](linearity.md); the calibrated gain is then held fixed.[Part I, Figure 2 and steps T1–T7: VCO preparation, frequency-counter readout, DC sensitivity and linearity sweep](lab-2-fm-modulation-demodulation-and-bessel-zeros-njit-ece-489.md)

An audio oscillator replaces the constant control voltage. An [oscilloscope](oscilloscope.md) displays the [signal](signal.md) and its [FFT](fast-fourier-transform.md) [frequency spectrum](frequency-spectrum.md) together. Zero modulation supplies a carrier reference. Increasing message [amplitude](wave-amplitude.md) reveals sidebands, compares their heights with the carrier, and locates a carrier minimum. These readouts test the spectrum and infer [frequency deviation](frequency-deviation.md). This is a student procedure, not a report of measured results.[“The FM Spectrum”, steps T8–T13: audio-oscillator input, simultaneous waveform/FFT, unmodulated reference, relative sideband heights and carrier minimum](lab-2-fm-modulation-demodulation-and-bessel-zeros-njit-ece-489.md)

A carrier minimum is a minimum of one [Fourier coefficient](fourier-coefficient.md), not disappearance of the whole [signal](signal.md). In the ideal model the first positive zero of $J_0$ is approximately $\beta=2.4048256$, while the [wave envelope](envelope-waves.md) remains $A$. The lab's introductory special-cases paragraph agrees with this rounded value; step T12 mistakenly repeats the equal-sideband value for the carrier zero.[“Special Cases, β=1.45 and β=2.405”, compared with the inconsistent numerical annotation in T12](lab-2-fm-modulation-demodulation-and-bessel-zeros-njit-ece-489.md)

The interpretation also has practical limits. A finite recording limits [frequency](frequency.md) resolution; inadequate sampling can cause [aliasing](aliasing.md); and nonlinear VCO response can introduce extra components. Keeping the gain fixed and first checking [linearity](linearity.md) helps distinguish those effects from a change in [FM modulation index](fm-modulation-index.md). The diagrams above are independent model calculations, not laboratory measurements.

## ↑ Ancestors (3)

1. [Frequency modulation](frequency-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)
