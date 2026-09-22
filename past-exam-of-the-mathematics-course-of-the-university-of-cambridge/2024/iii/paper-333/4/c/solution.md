<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $l=\pi/L$. For the specified [quasi-geostrophic streamfunction](../../../../../../quasi-geostrophic-streamfunction.md), the complex amplitudes of the disturbance fields are

$$
\widehat u=-l\widehat\psi\cos(ly),
\qquad
\widehat v=ik\widehat\psi\sin(ly).
$$

The product of these two amplitudes is purely imaginary after one is conjugated, so its zonal mean vanishes:

$$
\overline{u'v'}
=\frac12\operatorname{Re}(\widehat u\widehat v^*)=0.
$$

Consequently

$$
\boxed{\overline F^{(y)}=0}.
$$

[Geostrophic balance](../../../../../../geostrophic-balance.md) and [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) give

$$
\widehat\rho
=-\frac{\rho_0f_0}{g}
\widehat\psi_z\sin(ly).
$$

Therefore

$$
\overline{\rho'v'}
=-\frac{\rho_0f_0k}{2g}
\operatorname{Im}
(\widehat\psi_z\widehat\psi^*)
\sin^2(ly).
$$

Since $d\rho_s/dz=-\rho_0N^2/g$, the vertical [Eliassen–Palm flux](../../../../../../eliassen-palm-flux.md) is

$$
\boxed{
\overline F^{(z)}
=\frac{f_0^2}{N^2}
\frac k2
\operatorname{Im}
(\widehat\psi_z\widehat\psi^*)
\sin^2\frac{\pi y}{L}}.
$$

Thus it has the stated form

$$
\boxed{
\overline F^{(z)}=F_0\Theta(z)
\sin^2\frac{\pi y}{L}},
\qquad
F_0=\frac{f_0^2}{N^2},
$$

with

$$
\boxed{
\Theta(z)=\frac k2
\operatorname{Im}
(\widehat\psi_z\widehat\psi^*)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
