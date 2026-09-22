<h1 id="10/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Regular timing supplies a common interval and a well-defined [frequency](../../../../../../frequency.md) grid for a standard [discrete Fourier transform](../../../../../../discrete-fourier-transform-split.md) and [Fast Fourier transform](../../../../../../fast-fourier-transform.md). It also makes sample-index lags correspond to fixed physical delays in [cross-correlation](../../../../../../cross-correlation.md), [autocorrelation](../../../../../../autocorrelation.md) and digital filtering. These methods estimate [frequency](../../../../../../frequency.md) content and characteristic periods, separate instrument or environmental noise from signals, identify arrivals and time delays, and compare ground-motion spectra.

A uniform interval establishes a [Nyquist frequency](../../../../../../nyquist-frequency.md); [frequencies](../../../../../../frequency.md) above it alias unless filtered before acquisition. Interpolating irregular data onto a regular grid does not undo prior [aliasing](../../../../../../aliasing.md) or fill large gaps with new measurements, and it can alter spectra and create correlated errors. Methods that directly use irregular times are possible, but the ordinary FFT and fixed-lag filter formulas cannot simply treat the original irregular observations as evenly spaced.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [10](../../../10.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../split.md)
7. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Earth sciences (geology) course of the University of Oxford](../../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
