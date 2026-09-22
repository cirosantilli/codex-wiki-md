<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

In a homogeneous, source-free, nonmagnetic [dielectric](../../../../../dielectric.md) the electric [wave equation](../../../../../wave-equation-split.md) is

$$
\boxed{\nabla^2\mathbf E-\frac{\epsilon_r}{c^2}\partial_t^2\mathbf E=0.}
$$

Set $\theta=\omega t-kx$ and $E_y=f(z)\cos\theta$. Substitution gives $f''+(\epsilon_r\omega^2/c^2-k^2)f=0$. For the labelled field form (a), $f=E_0\cos Kz$, so $K^2=\epsilon_r\omega^2/c^2-k^2>0$. For form (b), $f=E'_0e^{sK'z}$ with $s=\pm1$, so $K'^2=k^2-\epsilon_r\omega^2/c^2>0$. These give the two stated inequalities, with equality a zero-transverse-wavenumber limiting case.

[Faraday's law](../../../../../faraday-s-law-of-induction.md) gives the associated wave [magnetic field](../../../../../magnetic-field-split.md), without an added static field,

$$
\boxed{\mathbf H=\frac1{\mu_0\omega}\left(f'(z)\sin\theta,0,kf(z)\cos\theta\right).}
$$

Thus in case (a), $H_x=-KE_0\sin(Kz)\sin\theta/(\mu_0\omega)$ and $H_z=kE_0\cos(Kz)\cos\theta/(\mu_0\omega)$. In case (b), $H_x=sK'E'_0e^{sK'z}\sin\theta/(\mu_0\omega)$ and $H_z=kE'_0e^{sK'z}\cos\theta/(\mu_0\omega)$. In both cases $H_y=0$.

For the [planar dielectric waveguide](../../../../../planar-dielectric-waveguide.md) the core is [dielectric](../../../../../dielectric.md) but the exterior is vacuum. Consequently the _exterior_ decay constant has $K'^2=k^2-\omega^2/c^2$, while the interior oscillation has $K^2=\epsilon_r\omega^2/c^2-k^2$. Adding gives the relation labelled (c):

$$
\boxed{K^2+K'^2=\frac{(\epsilon_r-1)\omega^2}{c^2}.}
$$

For an even bound mode the complete profile can be written

$$
f(z)=\begin{cases}E_0\cos(Kz),&|z|\leq d,\\E_0\cos(Kd)e^{-K'(|z|-d)},&|z|\geq d.\end{cases}
$$

[Continuity](../../../../../continuous-function.md) of tangential $E_y$ fixes the exterior amplitude; [continuity](../../../../../continuous-function.md) of tangential $H_x$ makes $f'$ continuous because both media have [magnetic permeability](../../../../../permeability-electromagnetism.md) $\mu_0$. At $z=d$,

$$
-KE_0\sin(Kd)=-K'E_0\cos(Kd),\qquad
\boxed{K\tan(Kd)=K',}
$$

which is the relation labelled (d). The same even profile also matches at $z=-d$; [continuity](../../../../../continuous-function.md) of $H_z$ follows from that of $E_y$.

In the requested $K,K'$ plot, (c) is a first-quadrant [circle](../../../../../circle.md) and (d) rises from the origin to its first pole at $Kd=\pi/2$. Equivalently put $u=Kd$, $w=K'd$, and $\mathcal V=(\omega d/c)\sqrt{\epsilon_r-1}$. At $u=0$ the [circle](../../../../../circle.md) has $w=\mathcal V>0$ whereas $u\tan u=0$. At the other end of $0<u<\min(\mathcal V,\pi/2)$, the rising tangent curve exceeds the falling [circle](../../../../../circle.md). [Monotonicity](../../../../../monotonic-function.md) therefore gives one intersection on this first branch for every $\mathcal V>0$.

**The [fundamental even mode of a symmetric dielectric slab](../../../../../fundamental-even-mode-of-a-symmetric-dielectric-slab.md) has no positive cutoff in index contrast or thickness.** Its electric profile is a nodeless [cosine](../../../../../cosine.md) maximum at the mid-plane, smoothly joined to decaying exterior tails. The qualifier $\epsilon_r>1$ is essential: for the printed limiting value $\epsilon_r=1$, the [circle](../../../../../circle.md) collapses to $K=K'=0$ and there is no transversely confined bound mode. A uniform unconstrained wave is not a guided mode. This even-mode argument does not assert that the specified [cosine](../../../../../cosine.md) describes every possible odd guide mode.

<a id="section-b/b9/image-fundamental-slab-mode"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2-slab-mode.png)

**[Figure 1](#section-b/b9/image-fundamental-slab-mode). Fundamental slab mode**.

The original diagram uses the illustrative normalized radius $\mathcal V=1.4$; it is a scaled $KK'$ plot with $u=Kd,w=K'd$, followed by the corresponding field profile.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
