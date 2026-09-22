<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

Write $\zeta=(\nabla\times\mathbf u)\cdot\mathbf e_z$ and $q=\zeta-f\eta/h_0$, so the PDF's vector [potential vorticity](../../../../../potential-vorticity.md) is $\mathbf Q=q\mathbf e_z$. The local TeX loses some of this boldface. Taking the vertical [curl](../../../../../curl.md) of the momentum equation gives $\zeta_t=-f\nabla\cdot\mathbf u$, while [mass conservation](../../../../../mass-conservation.md) gives $\eta_t=-h_0\nabla\cdot\mathbf u$. Thus

$$
\boxed{q_t=\zeta_t-\frac f{h_0}\eta_t=0,\qquad \mathbf Q_t=0}.
$$

This is the linear perturbation of [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md), scaled by $h_0$; it should not be confused with the full nonlinear conserved ratio $(f+\zeta)/h$.

Since $\nabla\cdot(\mathbf e_z\times\mathbf u)=-\zeta$, taking the [divergence](../../../../../divergence.md) of momentum gives $(\nabla\cdot\mathbf u)_t=f\zeta-g\nabla^2\eta$. Differentiate [mass conservation](../../../../../mass-conservation.md) and use $\zeta=q+f\eta/h_0$ to obtain

$$
\boxed{\eta_{tt}-gh_0\nabla^2\eta+f^2\eta=-h_0 f q=-h_0\mathbf f\cdot\mathbf Q}.
$$

For $\mathbf Q=0$, substitution of the stated [plane wave](../../../../../plane-wave.md) gives the [linear rotating shallow-water dispersion relation](../../../../../linear-rotating-shallow-water-dispersion-relation.md), with $c=\sqrt{gh_0}$:

$$
\boxed{\omega^2=f^2+c^2k^2,\qquad\omega_\pm(k)=\pm\sqrt{f^2+c^2k^2}}.
$$

The two even branches approach $\pm c|k|$ at large $|k|$ and have values $\pm|f|$ at $k=0$. The original [dispersion diagram](../../../../../dispersion-diagram.md) below also compares the speed magnitudes.

<a id="18d/image-a-dispersion-relation-and-its-velocity-branches"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4-dispersion.png)

**[Figure 1](#18d/image-a-dispersion-relation-and-its-velocity-branches). A dispersion relation and its velocity branches**. Rotating shallow-water frequency branches and magnitudes of [phase velocities](../../../../../phase-velocity.md) and [group velocities](../../../../../group-velocity.md), with dimensionless [wavenumber](../../../../../wavenumber.md).

For $k\ne0$, the [phase velocity](../../../../../phase-velocity.md) and [group velocity](../../../../../group-velocity.md) magnitudes are

$$
\boxed{|c_p|=\frac{|\omega|}{|k|}=\sqrt{c^2+\frac{f^2}{k^2}},\qquad
|c_g|=\left|\frac{d\omega}{dk}\right|=\frac{c^2|k|}{\sqrt{f^2+c^2k^2}},\qquad |c_p||c_g|=c^2}.
$$

The printed convention $e^{i(kx+\omega t)}$ means the signed [phase velocity](../../../../../phase-velocity.md) is $-\omega/k$ and the signed [group velocity](../../../../../group-velocity.md) is $-d\omega/dk$. The speed magnitudes above are independent of that sign convention.

For $f\ne0$, longer [wavelengths](../../../../../wavelength.md) have greater [phase velocity](../../../../../phase-velocity.md) but smaller [group velocity](../../../../../group-velocity.md): individual crests and [wave packets](../../../../../wave-packet.md) therefore answer “faster or slower” differently. At long [wavelength](../../../../../wavelength.md), $|k|\ll|f|/c$, the [frequency](../../../../../frequency.md) is nearly the inertial [frequency](../../../../../frequency.md) $|f|$, $|c_p|\sim|f|/|k|$, and $|c_g|\sim c^2|k|/|f|$. Rotation has its largest relative effect here, and the waves are strongly [dispersive](../../../../../wave-dispersion.md). At short [wavelength](../../../../../wavelength.md), $|k|\gg|f|/c$, both speeds tend to $c$ and rotation gives only a small, weakly [dispersive](../../../../../wave-dispersion.md) correction. If $f=0$, the gravity waves are [nondispersive](../../../../../nondispersive-wave.md), with speed $c$; at $k=0$ the [phase velocity](../../../../../phase-velocity.md) formula is undefined.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
