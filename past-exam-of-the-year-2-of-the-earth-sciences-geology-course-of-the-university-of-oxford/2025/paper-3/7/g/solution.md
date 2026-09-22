<h1 id="7/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

[Aliasing](../../../../../aliasing.md) occurs because a sampled grid cannot distinguish certain different continuous [Fourier modes](../../../../../fourier-mode.md). With spacing $h$, modes $k$ and $k+2\pi m/h$ agree at every sample point. Frequencies above the [Nyquist frequency](../../../../../nyquist-frequency.md) can therefore be misidentified as lower frequencies, changing the resolved spectrum and its subsequent diffusion rate.

For the corrected grid, $h=10/128\,\mathrm{cm}$ and the maximum resolved angular wavenumber is approximately $\pi/h\simeq40.2\,\mathrm{cm^{-1}}$. The initial [Gaussian function](../../../../../gaussian-function.md) has spectral envelope proportional to $e^{-a|k|^2/4}$. At that one-coordinate cutoff the factor is about $e^{-40.4}$, so the omitted high-frequency tail is tiny. Its continuation mismatch at the distant edges is also tiny. **Significant aliasing is not expected for this resolved, smooth initial condition.**

The [linear](../../../../../linearity.md) constant-coefficient [heat equation](../../../../../heat-equation.md) only damps existing modes; it does not generate higher frequencies through nonlinear products. An unresolved narrow peak, a sharp edge or a nonlinear source would require a separate resolution assessment. The duplicated-endpoint grid issue described above should not be diagnosed as high-frequency folding.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [7](../../7.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2025](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
