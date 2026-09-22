<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Split the Fourier integral at zero and use the two stationary covariance branches:

$$
s(\omega)=\int_0^\infty e^{-(A+i\omega I)\tau}\sigma\,d\tau
+\int_0^\infty e^{-(A-i\omega I)\tau}\!{}^T\sigma\,d\tau.
$$

Equivalently, Fourier transforming the [Multivariate Ornstein-Uhlenbeck process](../../../../../../../multivariate-ornstein-uhlenbeck-process.md) equation gives

$$
(A+i\omega I)x(\omega)=b\Lambda(\omega).
$$

Unit white-noise covariance then yields the [Ornstein-Uhlenbeck power spectrum](../../../../../../../ornstein-uhlenbeck-power-spectrum.md)

$$
s(\omega)=(A+i\omega I)^{-1}bb^T(A^T-i\omega I)^{-1},
$$

so

$$
\boxed{(A+i\omega I)s(\omega)(A^T-i\omega I)=bb^T}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 353](../../../../paper-353-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
