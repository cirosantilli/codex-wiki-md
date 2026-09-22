<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a zonal basic [geostrophic flow](../../../../../../geostrophic-flow.md) $U(y)$, take $\psi_0'(y)=-U(y)$ and write $\psi=\psi_0+\phi$. The flat-bottom [shallow-water quasi-geostrophic potential vorticity](../../../../../../shallow-water-quasi-geostrophic-potential-vorticity.md) gradient of the basic state is

$$
Q_0'=\beta-U''+R_D^{-2}U.
$$

Linearizing its material conservation gives the [Rossby-wave equation for a sheared zonal current](../../../../../../rossby-wave-equation-for-a-sheared-zonal-current.md),

$$
(\partial_t+U\partial_x)(\nabla_h^2\phi-R_D^{-2}\phi)+(\beta-U''+R_D^{-2}U)\phi_x=0.
$$

For a general nonuniform jet, a global two-dimensional [plane wave](../../../../../../plane-wave.md) is not an exact [normal mode](../../../../../../normal-mode.md): the coefficients depend on $y$. The exact zonal [normal mode](../../../../../../normal-mode.md) problem, $\phi=\widehat\phi(y)e^{i(kx-\omega t)}$, is

$$
\boxed{(U-\omega/k)[\widehat\phi''-(k^2+R_D^{-2})\widehat\phi]+Q_0'\widehat\phi=0,\qquad k\ne0,}
$$

with appropriate transverse boundary or radiation conditions. If the jet varies slowly compared with a wavelength, a local [plane wave](../../../../../../plane-wave.md) freezes these coefficients at $y_0$. Its local [dispersion relation](../../../../../../dispersion-relation.md) is

$$
\boxed{\omega=kU-\frac{k(\beta-U''+R_D^{-2}U)}{k^2+l^2+R_D^{-2}}.}
$$

In the nondivergent [Barotropic Rossby wave](../../../../../../barotropic-rossby-wave.md) model under a [rigid-lid approximation](../../../../../../rigid-lid-approximation.md), this becomes $\omega=kU-k(\beta-U'')/(k^2+l^2)$. It is exact for uniform $U$ and otherwise a local relation. Retaining the free-surface term also requires retaining the basic surface slope in $Q_0'$; simply adding $R_D^{-2}$ to the denominator while dropping $R_D^{-2}U$ from the numerator would describe a different prescribed-background model.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
