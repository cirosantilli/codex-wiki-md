<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use complex amplitudes with time dependence $e^{i\omega t}$, so the outgoing two-dimensional [Helmholtz equation](../../../../../../../helmholtz-equation.md) kernel has phase $e^{-ik_0r}$. Dividing the harmonic form of [Lighthill acoustic analogy](../../../../../../../lighthill-acoustic-analogy.md) by $c_0^2$ and integrating the two source derivatives by parts gives an amplitude proportional to

$$
\widetilde\rho'\sim\frac{k_0^2}{c_0^2}\frac{e^{-ik_0r}}{\sqrt{k_0r}}\,n_in_j\int\widetilde T_{ij}(\mathbf y)\,d^2y.
$$

Only the magnitude is needed here; the specified kernel omits its constant phase and normalization. In the [acoustic compact-source approximation](../../../../../../../acoustic-compact-source-approximation.md), $\int\widetilde T_{ij}d^2y=O(\rho_0U^2\ell^2)$. With $\omega=O(U/\ell)$, hence $k_0\ell=O(m)$, the [two-dimensional compact quadrupole scaling](../../../../../../../two-dimensional-compact-quadrupole-scaling.md) is

$$
\frac{|\widetilde\rho'|}{\rho_0}=O\left[\frac{U^2}{c_0^2}(k_0\ell)^2(k_0r)^{-1/2}\right]=\boxed{O\left(m^{7/2}\sqrt{\ell/r}\right).}
$$

The half-power difference from three dimensions comes from cylindrical spreading, including its $k_0^{-1/2}$ factor. As in part (i), the [Mach number](../../../../../../../mach-number.md) power is stated with the geometrical range factor separated; $k_0r\gg1$ is still required.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 77](../../../../paper-77-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
