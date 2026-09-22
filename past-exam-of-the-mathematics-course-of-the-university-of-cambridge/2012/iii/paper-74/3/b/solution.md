<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [linear stability analysis](../../../../../../linear-stability.md) of a general stable two-species [reaction–diffusion system](../../../../../../reaction-diffusion-system.md), take [Fourier modes](../../../../../../fourier-mode.md) proportional to $e^{\lambda t+ikx}$. Their matrix is $J_k=J-k^2\operatorname{diag}(D_u,D_v)$. Put $s=k^2$, $\tau=\operatorname{tr}J$, $\Delta=\det J$ and $B=D_va_{11}+D_ua_{22}$. Then

$$
\tau_k=\tau-(D_u+D_v)s,\qquad
\Delta_k=\Delta-Bs+D_uD_vs^2.
$$

The full system is stable precisely when $\tau_k<0$ and $\Delta_k>0$ for every allowed mode. If the homogeneous state is stable, the trace already decreases with $s$; only the determinant can change sign. If $B\leq0$, its minimum for $s\geq0$ is at zero. If $B>0$, it is at $s_*=B/(2D_uD_v)$. Thus the [two-species Turing criterion](../../../../../../two-species-diffusion-driven-instability-criterion.md) for instability on a continuum of wavenumbers is

$$
\boxed{\tau<0,\quad\Delta>0,\quad B>0,\quad
B^2>4D_uD_v\Delta.}
$$

Strict stability has $B<2\sqrt{D_uD_v\Delta}$ together with the homogeneous conditions. Equality at positive $B$ marks a stationary neutral mode. At that first onset,

$$
\boxed{k_c^2=\frac{B}{2D_uD_v}=\sqrt{\frac{\Delta}{D_uD_v}},\qquad
k_c=\left(\frac{\Delta}{D_uD_v}\right)^{1/4}.}
$$

Beyond threshold, the growing band lies between the positive roots $s_\pm=[B\pm\sqrt{B^2-4D_uD_v\Delta}]/(2D_uD_v)$, as long as the homogeneous trace stays negative.

For the [Brusselator](../../../../../../brusselator.md), $B=D_v(b-1)-D_ua^2$. Write $r=D_u/D_v$. The stationary determinant threshold gives the [Turing threshold of the Brusselator](../../../../../../turing-threshold-of-the-brusselator.md) in dimensional diffusivities:

$$
\boxed{b_T=(1+a\sqrt r)^2,\qquad
k_c^2=\frac{a}{\sqrt{D_uD_v}},\qquad
k_c=\frac{\sqrt a}{(D_uD_v)^{1/4}}.}
$$

For this to be a genuine diffusion-driven loss of stability, it must occur before the homogeneous [Hopf bifurcation](../../../../../../hopf-bifurcation.md) threshold. The [Brusselator Turing-before-Hopf diffusivity condition](../../../../../../brusselator-turing-before-hopf-diffusivity-condition.md) is

$$
\boxed{b_T<1+a^2
\quad\Longleftrightarrow\quad
\frac{D_v}{D_u}>\left(\frac{\sqrt{1+a^2}+1}{a}\right)^2.}
$$

Indeed $a^2r+2a\sqrt r<a^2$ is equivalent to $\sqrt r<(\sqrt{1+a^2}-1)/a$. With this strict inequality, $b_T<b<b_H$ contains a spatially unstable but homogeneously stable interval. If the ratio condition fails, the first linear instability as $b$ increases is homogeneous at $b_H$, rather than a [Turing instability](../../../../../../turing-instability.md); equality gives simultaneous neutral homogeneous and finite-wavenumber modes. Equal diffusivities cannot produce a [Turing instability](../../../../../../turing-instability.md).

These continuum formulas assume the onset wavenumber is available. On a finite domain with a specified discrete mode set, the [discrete-mode Turing threshold for the Brusselator](../../../../../../discrete-mode-turing-threshold-for-the-brusselator.md) is

$$
\boxed{b_T^{\rm discrete}=\min_{k\ne0\ \rm allowed}
\left[1+a^2\frac{D_u}{D_v}+D_uk^2+\frac{a^2}{D_vk^2}\right],}
$$

provided this minimum is below $b_H$. The question supplies no boundary geometry, so the continuous-mode onset above is the usual answer; this last expression states how a finite-size restriction changes it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
