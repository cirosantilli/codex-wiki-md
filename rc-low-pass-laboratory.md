# RC low-pass laboratory

↑ **Parent:** [RC low-pass filter](rc-low-pass-filter.md)

The University of Colorado Boulder's Lab 3: Filters, §§7.1–7.4, specifies measuring the [resistor](resistor.md) and [capacitor](capacitor.md), then driving the assembled [RC low-pass filter](rc-low-pass-filter.md) with a [function generator](function-generator.md). A two-channel [oscilloscope](oscilloscope.md) reads actual [input](input-computer-science.md) and [output](output-computing.md) using high [electrical impedance](electrical-impedance.md). Sweep the [frequency](frequency.md), record the voltage [amplitude](wave-amplitude.md) ratio, and locate $1/\sqrt2$. A control compares a cable with a $10\times$ [oscilloscope probe](oscilloscope-probe.md) on a resistive [voltage divider](voltage-divider.md), isolating measurement [capacitance](capacitance.md) before using the probe for the filter. A slow [square wave](square-wave.md) then lets discharge timing estimate the [time constant](time-constant.md) independently. Agreement supports the [RC low-pass frequency response](rc-low-pass-frequency-response.md); source [output impedance](output-impedance.md), probe loading, and instrument [signal bandwidth](signal-bandwidth.md) limit it. These are prescribed measurements, with no measured dataset supplied here.[Lab 3: Filters, §§7.1.1–7.1.3, Fig. 9 and §7.2.1, §§7.2.3, 7.3 and 7.4: component preparation, two-channel setup, probe control, frequency sweep and discharge timing](lab-3-filters-by-university-of-colorado-boulder-physics-undergraduate-labs.md)

The two-channel setup can also test the predicted [phase difference](phase-difference.md) directly: for positive [frequency](frequency.md) $f$, measure the output's time lag $\Delta t$ between corresponding features of the two [sinusoids](sinusoid.md). For this single-stage model the phase lies between $-\pi/2$ and $0$, so choose the lag within a quarter cycle and calculate $\phi=-2\pi f\Delta t$. At the [cutoff frequency](cutoff-frequency.md) the predicted lag is one eighth of a cycle. This tests the timing part of the [frequency response](frequency-response.md) as well as the voltage ratio.

## ↑ Ancestors (6)

1. [RC low-pass filter](rc-low-pass-filter.md)
2. [Low-pass filter](low-pass-filter.md)
3. [Linear filter](linear-filter.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)
