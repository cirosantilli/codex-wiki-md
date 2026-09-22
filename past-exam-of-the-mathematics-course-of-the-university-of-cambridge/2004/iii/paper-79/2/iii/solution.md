<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use local coordinates with the interface $z=0$, solid below and fluid above, and choose the [P-SV displacement potentials](../../../../../../p-sv-displacement-potentials.md) convention $u_x=\phi_x-\psi_z$, $u_z=\phi_z+\psi_x$. Let the reflected P and SV potential [wave amplitudes](../../../../../../wave-amplitude.md) be $A,B$, while the transmitted P [wave amplitude](../../../../../../wave-amplitude.md) is $T_P$. All four waves have the same tangential slowness

$$
p=\frac{\sin\theta_P}{\alpha}=\frac{\sin\theta_S}{\beta}=\frac{\sin\theta_f}{\alpha_f},\qquad
q_P=\frac{\cos\theta_P}{\alpha},\quad q_S=\frac{\cos\theta_S}{\beta},\quad q_f=\frac{\cos\theta_f}{\alpha_f}.
$$

The incident and transmitted retarded times have negative $q_Pz,q_fz$, while [elastic waves](../../../../../../elastic-wave.md) have positive $q_Pz,q_Sz$. At the interface all waveform [derivatives](../../../../../../derivative.md) therefore have the same argument. [displacement field](../../../../../../displacement-field-mechanics.md) continuity gives

$$
q_P(1-A)+pB=q_fT_P. \qquad(1)
$$

With [Lamé parameters](../../../../../../lame-parameter.md) $\mu=\rho\beta^2$ and $\lambda=\rho(\alpha^2-2\beta^2)$, the shear and normal [stresses](../../../../../../stress.md) follow directly from differentiation:

$$
\sigma_{xz}=\mu(2\phi_{xz}+\psi_{xx}-\psi_{zz}),\qquad
\sigma_{zz}=\lambda\Delta\phi+2\mu(\phi_{zz}+\psi_{xz}).
$$

The fluid has no shear [traction](../../../../../../traction.md), so the coefficient of $f''$ in $\sigma_{xz}$ must vanish:

$$
\frac{\sin2\theta_P}{\alpha^2}(1-A)-\frac{\cos2\theta_S}{\beta^2}B=0. \qquad(2)
$$

The coefficient of $f''$ in the solid [stress](../../../../../../stress.md) is $\rho[\cos2\theta_S(1+A)-\sin2\theta_SB]$; in the fluid it is $\rho_fT_P$. Thus

$$
\rho[\cos2\theta_S(1+A)-\sin2\theta_SB]=\rho_fT_P. \qquad(3)
$$

These are the three required matching conditions; tangential [displacement field](../../../../../../displacement-field-mechanics.md) need not be continuous at a solid–inviscid-fluid boundary.

Put $C=\cos2\theta_S$ and $X=1-A$. From (2), $B=(\beta^2/\alpha^2)(\sin2\theta_P/C)X$. In (1), the coefficient of $X$ simplifies because $C+2(\beta^2/\alpha^2)\sin^2\theta_P=1$. Hence $X=(\alpha C\cos\theta_f)/(\alpha_f\cos\theta_P)T_P$. Substitute this into (3) to obtain

$$
2\rho C=\left[\rho_f+\frac{\rho\alpha\cos\theta_f}{\alpha_f\cos\theta_P}
\left(C^2+\frac{\beta^2}{\alpha^2}\sin2\theta_P\sin2\theta_S\right)\right]T_P.
$$

Therefore the [solid-fluid P-wave transmission coefficient](../../../../../../solid-fluid-p-wave-transmission-coefficient.md) is

$$
\boxed{T_P=\frac{2\rho\alpha_f\cos2\theta_S\cos\theta_P}
{\rho_f\alpha_f\cos\theta_P+\rho\alpha\left[\cos^22\theta_S+(\beta^2/\alpha^2)\sin2\theta_P\sin2\theta_S\right]\cos\theta_f}.}
$$

Division by $C$ was only an elimination device; the final expression extends continuously to $C=0$. The normal-incidence value is $2\rho\alpha_f/(\rho\alpha+\rho_f\alpha_f)$. This is a potential coefficient; longitudinal [displacement field](../../../../../../displacement-field-mechanics.md) transmission additionally multiplies it by $\alpha/\alpha_f$. The original PDF's bracket lies in the denominator and contains $\beta^2/\alpha^2$ and $\cos\theta_f$. The converted TeX misplaces the bracket, substitutes $\theta^2$ for $\beta^2$, and loses the final cosine.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
