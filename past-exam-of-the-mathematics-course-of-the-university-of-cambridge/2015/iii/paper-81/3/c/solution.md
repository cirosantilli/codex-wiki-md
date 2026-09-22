<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Analytically continuing the [free-particle propagator](../../../../../../free-particle-propagator.md) to imaginary time gives the [Gaussian heat kernel](../../../../../../gaussian-heat-kernel.md)

$$
K_0(x;\beta)=\left(\frac m{2\pi\hbar^2\beta}\right)^{1/2}\exp\left(-\frac{mx^2}{2\hbar^2\beta}\right).
$$

The two image endpoints have displacements $2rL$ and $2rL-2q$ from the starting point. Inserting their kernels into the [thermal trace of an interval image kernel](../../../../../../thermal-trace-of-an-interval-image-kernel.md) gives

$$
\boxed{Z=\left(\frac m{2\pi\hbar^2\beta}\right)^{1/2}\int_0^L dq\sum_{r\in\mathbb Z}\left[e^{-2m(rL)^2/(\hbar^2\beta)}-e^{-2m(rL-q)^2/(\hbar^2\beta)}\right]}.
$$

The prefactor comes from the normalization of the [free-particle propagator](../../../../../../free-particle-propagator.md); it cannot be dropped from a thermal trace.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
