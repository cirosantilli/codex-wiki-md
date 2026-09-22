<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Translation invariance of the stationary surface statistics implies that a single incident tangential wavenumber retains that wavenumber in its coherent mean. Hence, away from the surface, write

$$
\boxed{\langle\psi_s(x,z)\rangle=Ar_b(\alpha,\omega)e^{i\alpha x+i\beta z},\qquad
\langle\psi_{\rm tot}\rangle=Ae^{i\alpha x}\left(e^{-i\beta z}+r_be^{i\beta z}\right).}
$$

The unknown effective [reflection coefficient](../../../../../../reflection-coefficient.md) $r_b$ is referenced to the mean plane $z=0$. It may be the rigid or [pressure](../../../../../../pressure.md)-release coefficient just derived, or a more general rough-boundary response. Lossless microscopic reflection does not require $|r_b|=1$: diffuse scattering removes power from the coherent specular field.

For the added planar upper interface, keep the same tangential wavenumber $\alpha$. Let $\beta_2=\sqrt{k_2^2-\alpha^2}$ on its outgoing sheet. The [normal acoustic impedances](../../../../../../normal-acoustic-impedance.md) in the layer and upper medium are

$$
Z_1=\frac{\rho\omega}{\beta},\qquad Z_2=\frac{\rho_2\omega}{\beta_2}.
$$

Continuity of [pressure](../../../../../../pressure.md) and normal [velocity](../../../../../../velocity.md) gives the reflection coefficient for upward incidence from the layer and transmission coefficient for downward incidence from above:

$$
r_{12}=\frac{Z_2-Z_1}{Z_2+Z_1},\qquad t_{21}=\frac{2Z_1}{Z_2+Z_1}.
$$

If a separate impedance sheet rather than an ordinary fluid interface is intended, its specified effective impedance replaces the upper termination; a sheet impedance has not otherwise been given. These formulas correspond to the stated two-fluid interface.

Let the upper incident [pressure](../../../../../../pressure.md) [amplitude](../../../../../../wave-amplitude.md) at $z=d$ be $I$. If $D$ and $U$ denote downward and upward layer amplitudes at that plane, their interface and lower-reflection relations are

$$
D=t_{21}I+r_{12}U,\qquad U=r_be^{2i\beta d}D.
$$

Solving, or summing the geometric series of repeated round trips, gives the [coherent acoustic layer above a rough reflector](../../../../../../coherent-acoustic-layer-above-a-rough-reflector.md):

$$
\boxed{\langle\psi_{\rm tot}(x,z)\rangle=
\frac{t_{21}I\,e^{i\alpha x}}{1-r_{12}r_be^{2i\beta d}}
\left[e^{-i\beta(z-d)}+r_be^{2i\beta d}e^{i\beta(z-d)}\right],\qquad h(x)\leq z\leq d.}
$$

The expression describes the field at heights where the common homogeneous layer exists; perturbative mean fields near the moving rough boundary need their physical trace evaluated separately. For an upper incident wave normalized as $e^{i\alpha x-i\beta_2z}$, set $I=e^{-i\beta_2d}$. With a matched upper medium, $r_{12}=0$ and $t_{21}=1$, the formula reduces to the single lower-reflection field. Zeros of the denominator give ideal layer resonances, interpreted with outgoing continuation or small loss.

This is a coherent specular description: a single effective $r_b$ closes the downward/upward mean amplitudes. Diffuse paths reflected back from the upper interface can modify the mean response; they must either be neglected in this approximation or included in the effective lower reflection coefficient for the actual layered environment. Without a full roughness spectrum and boundary type, a unique numerical mean field cannot be specified beyond this general coefficient form.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
