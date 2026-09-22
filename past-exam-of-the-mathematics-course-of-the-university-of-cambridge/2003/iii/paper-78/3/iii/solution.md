<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With vertical [shear modulus](../../../../../../shear-modulus.md) $\rho'\beta_z'^2$ and horizontal [shear modulus](../../../../../../shear-modulus.md) $\rho'\beta_x'^2$, force balance therefore gives the anisotropic [shear-horizontal wave](../../../../../../shear-horizontal-wave.md) equation

$$
\rho'u_{y,tt}=\partial_z\sigma_{yz}+\partial_x\sigma_{xy}
=\rho'\beta_z'^2u_{y,zz}+\rho'\beta_x'^2u_{y,xx}.
$$

For $u_y=Y(z)e^{i(kx-\omega t)}$, the layer vertical [wavenumber](../../../../../../wavenumber.md) and substrate decay exponent are

$$
q^2=\frac{\omega^2-\beta_x'^2k^2}{\beta_z'^2},\qquad
\kappa^2=k^2-\frac{\omega^2}{\beta^2}.
$$

The free top still gives $Y=A\cos(qz)$; the substrate still has $Y=B e^{-\kappa(z-h)}$. Welded displacement continuity and the now anisotropic [traction](../../../../../../traction.md) continuity give

$$
B=A\cos(qh),\qquad \rho'\beta_z'^2qA\sin(qh)=\mu\kappa B.
$$

Hence the [anisotropic Love-wave dispersion](../../../../../../anisotropic-love-wave-dispersion.md) relation is

$$
\boxed{\tan(qh)=\frac{\mu\kappa}{\rho'\beta_z'^2q}}.
$$

Equivalently, writing $c=\omega/k$,

$$
\tan\left[\frac{\omega h}{\beta'_z}\sqrt{1-\frac{\beta_x'^2}{c^2}}\right]
=\frac{\rho\beta^2}{\rho'\beta'_z}
\frac{\sqrt{c^{-2}-\beta^{-2}}}{\sqrt{1-\beta_x'^2/c^2}},\qquad \beta'_x<c<\beta.
$$

This replaces the isotropic speed in the layer equation by separate horizontal and vertical speeds and replaces the layer [traction](../../../../../../traction.md) modulus by $\rho'\beta_z'^2$. No additional SH/P-SV coupling arises for the aligned symmetry axes and constitutive law here.

A rigid base still imposes $q_n=\chi_n/h$, but now

$$
\omega^2=\beta_x'^2k^2+\omega_{n,z}^2,\qquad\omega_{n,z}=\frac{\beta'_z\chi_n}{h}.
$$

Thus

$$
\boxed{c_n=\frac{\beta'_x}{\sqrt{1-\omega_{n,z}^2/\omega^2}},\qquad
U_n=\beta'_x\sqrt{1-\omega_{n,z}^2/\omega^2}}.
$$

The vertical speed sets the resonance [frequencies](../../../../../../frequency.md), while the horizontal speed sets the high-[frequency](../../../../../../frequency.md) limits and $c_nU_n=\beta_x'^2$.

For the elastic substrate, put $\epsilon_x=\beta'_x/\beta$, $\zeta=\rho'\beta'_x\beta'_z/(\rho\beta^2)$, $W=\omega h/\beta'_z$ and $K=kh\beta'_x/\beta'_z$. The exact parameterization is

$$
W(y)=\frac{y\sqrt{1+\zeta^2\tan^2y}}{\sqrt{1-\epsilon_x^2}},\qquad
K(y)=\frac{y\sqrt{\epsilon_x^2+\zeta^2\tan^2y}}{\sqrt{1-\epsilon_x^2}},\qquad U=\beta'_x\frac{W'}{K'}.
$$

It reproduces the isotropic analysis with $\beta'$ replaced by $\beta'_z$ in the [frequency](../../../../../../frequency.md) scale, by $\beta'_x$ in the velocities, and by the two effective contrast parameters above. In particular the true cutoffs are $\omega_{c,n}=n\pi\beta'_z/[h\sqrt{1-\epsilon_x^2}]$, the group minima occur near $\omega_{n,z}$, and a sufficient rigid-limit validity range is

$$
\boxed{\frac{\omega h}{\beta'_z}-\chi_n\gg
\max\left\{\chi_n\epsilon_x^2,(\zeta^2\chi_n)^{1/3}\right\}}.
$$

For comparable horizontal and vertical layer speeds, a bounded density ratio and fixed mode index, the minimum estimate becomes $\delta_{\min}\sim(\zeta^2\chi_n/2)^{1/3}$ and $U_{\min}/\beta'_x\sim3(\zeta/\chi_n)^{1/3}/2^{2/3}$. If their ratio is extreme, that more specific minimum-depth estimate additionally needs $\zeta/\delta_{\min}\gg\epsilon_x$; the exact parameterization and load criterion remain valid without it. As in the isotropic case, neither a slow horizontal nor a slow vertical speed alone justifies the rigid boundary at cutoff or within the strong-dispersion transition.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
