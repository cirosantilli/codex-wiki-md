<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [Feynman gauge](../../../../../../feynman-gauge.md), use the mode expansion

$$
\widehat A^\mu(x)=
\int\frac{d^3\mathbf k}{(2\pi)^3\,2|\mathbf k|}
\sum_{\lambda=0}^3
\left[
\epsilon^\mu_\lambda(\mathbf k)a_\lambda(\mathbf k)e^{-ikx}
+\epsilon^{\mu*}_\lambda(\mathbf k)a_\lambda^\dagger(\mathbf k)e^{ikx}
\right],
$$

with $k^0=|\mathbf k|$ and the covariant polarization completeness relation. For $x^0>y^0$, time ordering retains the annihilation-creation contraction and gives the positive-frequency term; for $x^0<y^0$, it gives the negative-frequency term. Combining them by a $k^0$ contour integral gives

$$
\boxed{
\langle0|\mathcal T\widehat A^\mu(x)\widehat A^\nu(y)|0\rangle
=\int_{C_F}\frac{d^4k}{(2\pi)^4}
\frac{-i\eta^{\mu\nu}}{k^2}
e^{-ik\cdot(x-y)}}.
$$

The [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) places the positive-energy pole $k^0=|\mathbf k|-i\epsilon$ below the real axis and the negative-energy pole $k^0=-|\mathbf k|+i\epsilon$ above it. Equivalently the denominator is $k^2+i\epsilon$ with the contour along the real axis.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
