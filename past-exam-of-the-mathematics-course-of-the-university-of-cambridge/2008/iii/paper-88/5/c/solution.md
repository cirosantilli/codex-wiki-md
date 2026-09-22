<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $p^2+q^2>1$, $m=i\sqrt{p^2+q^2-1}$ and the [Weyl plane-wave representation](../../../../../../weyl-plane-wave-representation.md) contains [evanescent waves](../../../../../../evanescent-wave.md). Their amplitudes decay exponentially with the distance from the scattering region. Excluding them removes high transverse spatial frequencies, including subwavelength information. Near-field measurements can in principle detect them, but back-propagating their decay exponentially amplifies measurement errors.

For propagating data, the Fourier transfer satisfies $|\mathbf k_s-\mathbf k_i|\leq2k$. One illumination still samples only the [Ewald sphere](../../../../../../ewald-sphere.md), so this frequency bound does not imply access to every mode inside that ball. The lack of a volumetric spectrum is the separate nonuniqueness described in the previous part.

The [Born approximation](../../../../../../born-approximation.md) requires the incident field to remain a good approximation inside the scatterer. A useful sufficient smallness estimate for a weak, extended inclusion is small accumulated phase $kD|n-1|\ll1$, alongside weak reflection and multiple scattering. Small pointwise contrast alone can fail for a thick inclusion or a resonance. The scalar Helmholtz and background-medium assumptions, and the extra linearization of $n^2-1$, also belong to the model's validity conditions.

Numerically, a finite [aperture](../../../../../../aperture.md) windows the measured fields and limits angular and Fourier resolution. Discrete sampling must satisfy the [Nyquist–Shannon sampling theorem](../../../../../../nyquist-shannon-sampling-theorem.md) for the retained transverse bandwidth; spacings $\Delta x,\Delta y\lesssim\pi/K_{\max}$ avoid its simplest aliasing. Finite [discrete Fourier transforms](../../../../../../discrete-fourier-transform.md) also introduce periodic continuation, truncation, interpolation and window errors. Noise, unresolved evanescent modes and near-grazing modes with $m\simeq0$ limit reliable recovery. Refining the grid cannot by itself fill the missing three-dimensional Fourier data.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
