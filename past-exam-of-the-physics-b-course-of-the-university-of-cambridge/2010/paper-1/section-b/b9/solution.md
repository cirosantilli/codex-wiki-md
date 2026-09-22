<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

[stress](../../../../../stress.md) describes internal [force](../../../../../force-split.md) per [area](../../../../../surface-area.md). A cut with unit normal $\hat{\mathbf n}$ has [traction](../../../../../traction.md) $\mathbf t=\boldsymbol\sigma\hat{\mathbf n}$; its normal component is $\hat{\mathbf n}\cdot\boldsymbol\sigma\hat{\mathbf n}$ and its remainder is shear [traction](../../../../../traction.md). [force balance](../../../../../force-balance.md) constrains the [stress](../../../../../stress.md) [divergence](../../../../../divergence.md), while ordinary local angular-momentum balance makes the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) symmetric in a medium without body couples.

[strain](../../../../../strain.md) describes deformation rather than [force](../../../../../force-split.md). For small [displacement](../../../../../displacement.md) [gradients](../../../../../gradient.md),

$$
\epsilon_{ij}=\frac12(\partial_i u_j+\partial_j u_i),\qquad
\frac{\Delta V}{V}=\epsilon_{kk}.
$$

The antisymmetric displacement-gradient part is a rigid rotation to first order and contributes no infinitesimal [strain](../../../../../strain.md). Engineering [shear strain](../../../../../shear-strain.md) is $\gamma_{xy}=2\epsilon_{xy}$, so it must not be confused with the tensor component. [stress](../../../../../stress.md) has units of [pressure](../../../../../pressure-split.md); [strain](../../../../../strain.md) is dimensionless.

An isotropic linear elastic solid obeys

$$
\sigma_{ij}=\lambda\epsilon_{kk}\delta_{ij}+2G\epsilon_{ij},\qquad
w=\tfrac12\lambda(\epsilon_{kk})^2+G\epsilon_{ij}\epsilon_{ij}.
$$

Two independent moduli are required. The [shear modulus](../../../../../shear-modulus.md) $G$ and [bulk modulus](../../../../../bulk-modulus.md) $K=\lambda+2G/3$ must be positive for stability. [Young's modulus](../../../../../young-s-modulus.md) and Poisson ratio satisfy

$$
E=2G(1+\nu)=\frac{9KG}{3K+G},\qquad
K=\frac{E}{3(1-2\nu)},\qquad -1<\nu<\tfrac12.
$$

For a tensile specimen with free side faces, $\sigma_{xx}=F/A$ gives $\epsilon_{xx}=\sigma_{xx}/E$ and $\epsilon_{yy}=\epsilon_{zz}=-\nu\sigma_{xx}/E$. Pure shear gives $\tau=G\gamma$; hydrostatic loading gives $\Delta V/V=-p/K$. The incompressible limit has $\nu\to1/2$ at finite shear stiffness, not vanishing shear resistance. Crystals can be anisotropic and need a fourth-rank elastic stiffness tensor instead of the isotropic two-constant law.

[elastic deformation](../../../../../elastic-deformation.md) is recoverable on unloading; it need not remain linear at large [strain](../../../../../strain.md). Beyond yield, irreversible rearrangements such as [dislocation](../../../../../dislocation.md) motion cause plastic [strain](../../../../../strain.md), often followed by hardening. Ductile samples can neck before fracture; brittle failure has much less plastic deformation. Engineering [stress](../../../../../stress.md) uses initial [area](../../../../../surface-area.md), while true [stress](../../../../../stress.md) uses the changing instantaneous [area](../../../../../surface-area.md). A decreasing engineering [stress](../../../../../stress.md) during [necking](../../../../../necking-engineering.md) therefore need not mean that local true [stress](../../../../../stress.md) decreases. [stress](../../../../../stress.md) concentrations, flaws and loading geometry can determine failure before a uniform-material strength is reached. Viscoelastic materials also show rate dependence, creep and [stress relaxation](../../../../../stress-relaxation.md); their losses cannot be described by a static Hooke law alone.

A tensile test should measure [force](../../../../../force-split.md) and gauge-length extension independently, correct machine compliance, align the grips, and control [strain](../../../../../strain.md) rate and [temperature](../../../../../temperature-split.md). Unloading distinguishes recoverable [strain](../../../../../strain.md) from a residual plastic extension. Separate shear or hydrostatic tests determine moduli that one axial measurement does not fix. Compression specimens need [friction](../../../../../friction.md) and buckling checks. Work per [volume](../../../../../volume.md) is $\int\sigma_{ij}d\epsilon_{ij}$; the recoverable part is [elastic energy](../../../../../elastic-energy.md), while a dissipative cycle produces a loss rather than creating [energy](../../../../../energy-split.md). The original loading/unloading curve below is a chosen constitutive sketch, not measured material data.

<a id="section-b/b9/image-stress-and-strain"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1-stress-strain.png)

**[Figure 3](#section-b/b9/image-stress-and-strain). Stress and strain**. Small-strain geometry and illustrative unloading.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
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
