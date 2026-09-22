<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

The displacement is along $x$, transverse to propagation in the membrane's $yz$ plane. Write $A=|A|e^{i\phi}$; then $d=|A|\cos(\omega t-k_yy-k_zz+\phi)$. Here $|A|$ is the displacement [amplitude](../../../../../wave-amplitude.md), $\phi$ the initial phase, $\omega$ the [angular frequency](../../../../../angular-frequency.md) and $\mathbf k$ the [wavevector](../../../../../wavevector.md) normal to constant-phase lines. Its magnitude is $2\pi/\lambda$, and its direction specifies phase propagation for the chosen sign convention.

For [equal-phase two-wave membrane modes](../../../../../equal-phase-two-wave-membrane-modes.md), two equal [complex amplitudes](../../../../../complex-amplitude.md) with opposite $k_y$ sum to

$$
d=2\operatorname{Re}\{A\cos(k_yy)e^{i(\omega t-k_zz)}\}.
$$

The edge condition gives $\cos(k_ya/2)=0$, hence $k_y=(2j+1)\pi/a$, $j=0,1,\ldots$, for this even-in-$y$ family. Opposite relative phase gives the [sine](../../../../../sine.md) family; together they yield all Dirichlet transverse modes $k_y=n\pi/a$, $n\ge1$. For the equal-phase family,

$$
\boxed{k_z=\sqrt{(\omega/c)^2-[(2j+1)\pi/a]^2}.}
$$

The lowest mode has $k_y=\pi/a$. Therefore

$$
\boxed{v_z=\frac\omega{k_z}=\frac c{\sqrt{1-(\lambda/2a)^2}},\qquad0<\lambda<2a.}
$$

It approaches $c$ for $\lambda\to0$ and diverges as $\lambda\to2a^-$; there is no real travelling-mode $k_z$ beyond the cutoff. This is an axial [phase velocity](../../../../../phase-velocity.md), not the [group velocity](../../../../../group-velocity.md): $v_g=c\sqrt{1-(\lambda/2a)^2}<c$. Here $c$ denotes the membrane wave [speed](../../../../../speed.md), not the [speed of light](../../../../../speed-of-light.md).

<a id="section-d/d12/image-membrane-cutoff-and-evanescent-response"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1-ia2010-membrane.png)

**[Figure 4](#section-d/d12/image-membrane-cutoff-and-evanescent-response). Membrane cutoff and evanescent response**. Original lowest-mode phase-velocity curve, with group velocity distinguished, and a schematic below-cutoff displacement envelope of exponential form. All lengths and amplitudes are dimensionless choices; no source apparatus drawing is copied.

For the [evanescent membrane response below cutoff](../../../../../evanescent-membrane-response-below-cutoff.md), below $f_c=c/(2a)$, put $k_z=-i\kappa$ for decay along positive $z$, with $\kappa=\sqrt{(\pi/a)^2-(\omega/c)^2}$. A localized central drive creates an evanescent, sinusoidally oscillating deformation decaying away in both axial directions. Far enough from the drive the leading profile is proportional to $\cos(\pi y/a)e^{-\kappa|z-z_0|}\cos(\omega t+\phi_0)$. Higher evanescent modes contribute near the point source. The pattern has no steadily advancing axial phase front or far-field propagating wave; decreasing [frequency](../../../../../frequency.md) increases its spatial localization.

## ↑ Ancestors (13)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
