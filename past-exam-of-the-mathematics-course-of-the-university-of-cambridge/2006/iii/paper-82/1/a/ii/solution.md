<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use time dependence $e^{i\omega t}$ and write the outgoing two-dimensional [Helmholtz equation](../../../../../../../helmholtz-equation.md) kernel as $G_2\sim C e^{-ik_0r}/\sqrt{k_0r}$, where $C$ is independent of the [Mach number](../../../../../../../mach-number.md). The harmonic [Lighthill acoustic analogy](../../../../../../../lighthill-acoustic-analogy.md) gives

$$
\widehat\rho'=\frac1{c_0^2}\partial_i\partial_j\int G_2(\mathbf x-\mathbf y)\widehat T_{ij}(\mathbf y)\,d^2y.
$$

For a compact [acoustic quadrupole](../../../../../../../acoustic-quadrupole.md), the source integral is $O(\rho_0U^2\ell^2)$. In the radiation region each derivative of the outgoing exponential supplies a factor of $k_0$, so

$$
\frac{|\widehat\rho'|}{\rho_0}=O\!\left[m^2(k_0\ell)^2(k_0r)^{-1/2}\right].
$$

Keeping the same advective source-frequency scaling as in (i), $\omega=O(U/\ell)$ and hence $k_0\ell=O(m)$. Therefore the [two-dimensional compact quadrupole scaling](../../../../../../../two-dimensional-compact-quadrupole-scaling.md) is

$$
\boxed{\frac{|\widehat\rho'|}{\rho_0}=O\!\left(m^{7/2}\sqrt{\frac\ell r}\right).}
$$

The changed exponent comes from cylindrical spreading $(k_0r)^{-1/2}$. Compactness $k_0\ell\ll1$ and the far-field condition $k_0r\gg1$ are separate assumptions. At fixed imposed $\omega$ and fixed $\ell$, with only $U$ varied, the stress instead gives an $O(m^2)$ dependence; monochromaticity alone does not supply the additional source-frequency assumption.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
