<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The line references below use the original listing's line numbers.

- Lines 1–7 set the grid dimensions, domain lengths, [thermal diffusivity](../../../../../thermal-diffusivity.md) and time interval. The elapsed time is $n_t\Delta t=10\,\mathrm s$.
- Lines 9–10 supply coordinates, subject to the periodic-grid correction above. Lines 16–17 sample the initial [Gaussian function](../../../../../gaussian-function.md).
- Lines 11–14 construct the [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md) frequency order and $K^2=K_X^2+K_Y^2$. Negative frequencies occupy the second half of each array. This is the discrete version of replacing each spatial derivative by multiplication by $ik$.
- Line 20 computes the two-dimensional [Fast Fourier transform](../../../../../fast-fourier-transform.md). Lines 22–24 multiply every mode by $\exp(-\alpha K^2\Delta t)$ at every step, implementing the modal solution derived above.
- Line 26 performs the inverse [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md). Taking the real part removes tiny imaginary [roundoff errors](../../../../../round-off-error.md); conjugate symmetry of the exact transformed real data already guarantees a real result.
- Lines 28–42 display the initial and final arrays. A common colour scale is needed to compare their peak [temperatures](../../../../../temperature-split.md); independent automatic colour scales can hide the decrease in amplitude.

For this linear homogeneous problem, the exponential update is exact for the retained modes, apart from [roundoff error](../../../../../round-off-error.md). It is not a forward [Euler method](../../../../../euler-method.md) step and does not require the explicit finite-difference diffusion stability restriction. Sampling, periodic modelling and spatial resolution still matter.

## ↑ Ancestors (12)

1. [E](../e.md)
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
