<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

- Constant [thermal diffusivity](../../../../../thermal-diffusivity.md) makes the [Fourier spectral method](../../../../../fourier-spectral-method.md) diagonal: each [Fourier mode](../../../../../fourier-mode.md) can be evolved by its exact exponential multiplier.
- The smooth initial [Gaussian function](../../../../../gaussian-function.md) has rapidly decaying [Fourier coefficients](../../../../../fourier-coefficient.md), so a moderate grid resolves it well. The [Fast Fourier transform](../../../../../fast-fourier-transform.md) provides an efficient change between the spatial grid and those coefficients.
- A [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md) describes a periodically repeated array. Opposite edges are identified by [periodic boundary conditions](../../../../../periodic-boundary-conditions.md); this is a periodically continued plate model, rather than a plate with prescribed cold or insulated edges.
- The initial hot spot is far from those edges. Over the stated short interval its width remains much smaller than the side length, so the periodic images have negligible influence near the centre. At sufficiently long times, periodic diffusion tends to the conserved spatial mean.

For consistency with the supplied wavenumbers, use an [FFT grid on a periodic interval](../../../../../fft-grid-on-a-periodic-interval.md): $x_j=jL_x/n_x$, $0\le j<n_x$, and similarly for $y$. In [MATLAB](../../../../../matlab.md), replace the endpoint-inclusive coordinate definitions by `x = (0:nx-1)*Lx/nx;` and `y = (0:ny-1)*Ly/ny;`. The supplied `linspace` arrays instead have spacing $L_x/(n_x-1)$ while the [Fourier multipliers](../../../../../fourier-multiplier.md) assume $L_x/n_x$. Including both copies of the periodic endpoint creates a grid inconsistency, separate from high-frequency [aliasing](../../../../../aliasing.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
