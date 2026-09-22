<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $\mathbf j_n=\bar\psi_n\boldsymbol\sigma\psi_n$ and $D=\bar\psi_\uparrow\bar\psi_\downarrow\psi_\downarrow\psi_\uparrow$. The [Pauli matrix completeness identity](../../../../../../pauli-matrix-completeness-identity.md), or direct evaluation of its three components, gives $\mathbf j^2=-6D$. Consequently the quartic action is $3UD=-U\mathbf j^2/2$.

The [Hubbard–Stratonovich decoupling](../../../../../../hubbard-stratonovich-transformation.md) follows by completing a three-component square at each site and time slice:

$$
\int d^3M\,\exp\left[-\Delta\tau\left(\frac{\mathbf M^2}{2U}-\mathbf M\cdot\mathbf j\right)\right]
=C\exp\left[\frac{U\Delta\tau}{2}\mathbf j^2\right]=C e^{-3U\Delta\tau D}.
$$

The constant $C$ is absorbed into the normalized auxiliary-field measure, and $U>0$ ensures convergence of the real [Gaussian integral](../../../../../../gaussian-integral.md). Thus the [spin-vector Hubbard–Stratonovich decoupling](../../../../../../spin-vector-hubbard-stratonovich-decoupling.md) yields

$$
\boxed{\mathcal S=\int_0^\beta d\tau\sum_{\mathbf k\sigma}\bar\psi_{\mathbf k\sigma}(\partial_\tau+\epsilon_{\mathbf k}-\mu)\psi_{\mathbf k\sigma}
+\int_0^\beta d\tau\sum_n\left[\frac{\mathbf M_n^2}{2U}-\bar\psi_n\mathbf M_n\cdot\boldsymbol\sigma\psi_n\right].}
$$

Integrating out $\mathbf M$ reconstructs the normal-ordered interaction exactly. The auxiliary field is periodic in imaginary time, while the fermionic fields remain antiperiodic.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
