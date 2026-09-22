# Vibroseis correlation

↑ **Parent:** [Vibroseis](vibroseis.md)

Let a linear Earth response $h$ be recorded using a known source sweep $s$, giving $d=s*h+n$. Cross-correlating the record with the sweep yields

$$
c(\tau)=\int d(t)s(t-\tau)\,dt=(h*R_{ss})(\tau)+R_{ns}(\tau).
$$

Thus a compact sweep [autocorrelation](autocorrelation.md) $R_{ss}$ produces pulse-compressed arrival wavelets, while unrelated noise has a smaller coherent response. The [Fourier transform](fourier-transform-split.md) of the result is $H(\omega)|S(\omega)|^2+N(\omega)\overline{S(\omega)}$. Correlation is a matched-filter operation, not an exact inversion of missing source [frequencies](frequency.md). Spectral shaping or stabilized deconvolution can further adjust the wavelet within the measured bandwidth.[Vibratory-source explanation: correlating the known sweep with geophone measurements](geophysical-survey-summary-report-section-3-geophysical-testing-methodology.md)

## ↑ Ancestors (7)

1. [Vibroseis](vibroseis.md)
2. [Seismic source](seismic-source.md)
3. [Seismology](seismology.md)
4. [Geophysics](geophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford/2022/paper-1/6/e/ii/solution.md)
- [Solution](past-exam-of-the-year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford/2022/paper-1/6/g/iii/solution.md)
- [Vibroseis](vibroseis.md)
