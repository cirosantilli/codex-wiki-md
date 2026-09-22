<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In ideal [computed tomography](../../../../../../computed-tomography.md), the unknown is an absorption coefficient $a(x)$. Along a straight ray the transmitted intensity satisfies $dI/d\tau=-aI$, so

$$
\log\frac{I_{\mathrm{in}}}{I_{\mathrm{out}}}=\int_{\mathbb R}a(\tau\boldsymbol d+\rho\boldsymbol n)d\tau=Ra(\rho,\theta).
$$

Thus calibrated transmission measurements supply the [Radon transform](../../../../../../radon-transform.md) of the slice. The inversion above reconstructs the coefficient by [filtered backprojection](../../../../../../filtered-backprojection.md): filter each projection in its transverse variable and then accumulate it over the rays through each image point. This turns a collection of line-integral measurements into a spatial map, which is the key usefulness of the result.

The ideal derivation assumes known ray geometry, sufficiently complete angular sampling and a straight-ray attenuation model. The ramp [Fourier multiplier](../../../../../../fourier-multiplier.md) grows at high frequency, so measurement noise is amplified. Practical reconstruction therefore uses discretization and [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md), for example a window on the ramp filter. Limited angles or missing detector positions cannot be treated as if they were complete noiseless [Radon transform](../../../../../../radon-transform.md) data.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
