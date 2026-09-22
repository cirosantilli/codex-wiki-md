<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the same $e^{-i\omega t}$ convention and an outgoing field. Define the [scattering potential](../../../../../../scattering-potential.md) with the positive-contrast sign,

$$
 Q(\mathbf r)=k^2[n(\mathbf r)^2-1],\qquad
 (\Delta+k^2)\psi=-Q\psi.
$$

The [outgoing Green function for the three-dimensional Helmholtz equation](../../../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md) is

$$
 G_k(\mathbf r,\mathbf r')=\frac{e^{ik|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|},\qquad
 (\Delta+k^2)G_k=-\delta.
$$

Thus the [Lippmann-Schwinger equation](../../../../../../lippmann-schwinger-equation.md) has a plus sign:

$$
 \psi=\psi_i+T\psi,\qquad
 (T\phi)(\mathbf r)=\int_VG_k(\mathbf r,\mathbf r')Q(\mathbf r')\phi(\mathbf r')\,d^3r'.
$$

Replacing the total field inside the integral by the incident field gives the [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md)

$$
\boxed{\psi_s^{(1)}(\mathbf r)=\frac{k^2}{4\pi}\int_V
 [n(\mathbf r')^2-1]\frac{e^{ik|\mathbf r-\mathbf r'|}}{|\mathbf r-\mathbf r'|}
 e^{ik\widehat{\mathbf r}_0\cdot\mathbf r'}\,d^3r'.}
$$

More generally, iterating the integral equation gives the [Born series](../../../../../../born-series.md) $\psi_s=\sum_{j\geq1}T^j\psi_i$; its first term is the boxed expression. A sufficient convergence condition is $\|T\|<1$ on the chosen space of fields in $V$, and accurate single-scattering truncation needs the neglected terms to be small. Weak refractive contrast is useful, but for a sufficiently large or resonant scatterer it is not by itself a guarantee of negligible [multiple scattering](../../../../../../multiple-scattering.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
