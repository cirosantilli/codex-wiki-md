<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Partition the range into planes $x_j=x_0+j\Delta x$. At each step, evaluate the refractive-index phase screen at $x_j$ or the midpoint, multiply the current envelope by $e^{\Delta xS_j}$, transform in $z$, multiply each transverse Fourier component by the diffraction phase $e^{-ik_z^2\Delta x/(2k_0)}$, and apply the inverse [Fourier transform](../../../../../../fourier-transform.md). Repeating this [split-step Fourier method](../../../../../../split-step-fourier-method.md) $m$ times produces $E(x_m,z)$ from $E(x_0,z)$. The step size must continue to resolve both longitudinal medium variation and the [Lie-Trotter splitting](../../../../../../lie-product-formula.md) error.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
