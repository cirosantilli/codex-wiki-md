<h1 id="section-b/b2/solution">Solution</h1>

↑ **Parent:** [B2](../b2.md)

**Two stabilization mechanisms.** [Steric stabilization](../../../../steric-stabilization.md) coats each [colloid](../../../../colloid.md) with adsorbed or grafted polymer layers. Bringing two particles close overlaps or compresses those layers, increasing their [free energy](../../../../thermodynamic-free-energy.md) through loss of chain conformations and, in a suitable solvent, increased local [osmotic pressure](../../../../osmotic-pressure.md). The resulting repulsion can keep the cores apart. A well-solvated nonionic coating can remain effective when added salt would screen electrostatic forces. Coatings can fail through desorption, poor solvent conditions or bridging, so simply adding arbitrary free polymer does not guarantee stabilization.

[Charge stabilization of colloids](../../../../charge-stabilization-of-colloids.md) instead uses similarly charged surfaces and their diffuse [electric double layers](../../../../electric-double-layer.md). Their approach costs electrostatic and ionic [free energy](../../../../thermodynamic-free-energy.md). In [DLVO theory](../../../../dlvo-theory.md), that repulsion competes with attractive [Van der Waals forces](../../../../van-der-waals-force.md). It is particularly sensitive to salt concentration, counterion valence and surface ionization.

**Bjerrum length.** The standard [Bjerrum length](../../../../bjerrum-length.md) is the separation at which the Coulomb interaction energy of two elementary charges equals thermal energy:

$$
\frac{e^2}{4\pi\varepsilon_0\varepsilon_r\ell_B}=k_BT,\qquad
\boxed{\ell_B=\frac{e^2}{4\pi\varepsilon_0\varepsilon_rk_BT}}.
$$

At $T\simeq298\,\mathrm K$ and $\varepsilon_r=78$, this is

$$
\boxed{\ell_B\simeq7.2\times10^{-10}\,\mathrm m=0.72\,\mathrm{nm}}.
$$

It compares ionic electrostatic coupling with thermal agitation. For ions of signed valences $z_1,z_2$, $U/(k_BT)=z_1z_2\ell_B/r$. The standard reference length uses $e$, not the whole colloid charge: assigning a colloid charge $Ze$ does not change the solvent's tabulated $\ell_B$.

**Screening and the printed normalization.** In a symmetric $z:z$ electrolyte, $z$ is the ionic valence magnitude, $e$ the elementary [electric charge](../../../../electric-charge-split.md), $n_\infty$ the bulk [number density](../../../../number-density.md) of each ionic species, $\varepsilon_0$ the [vacuum permittivity](../../../../vacuum-permittivity.md), $\varepsilon_R$ the solvent's [relative permittivity](../../../../relative-permittivity.md), $k_B$ the [Boltzmann constant](../../../../boltzmann-constant.md) and $T$ absolute [temperature](../../../../temperature-split.md). Mobile ions rearrange around a charged surface; the [Debye–Hückel screening length](../../../../debye-huckel-screening-length.md) $\kappa^{-1}$ sets the range of the resulting weak potential.

There is an SI normalization error in the original PDF. Combining the [Boltzmann distribution](../../../../boltzmann-distribution.md) $n_\pm=n_\infty e^{\mp ze\psi/(k_BT)}$ with the SI [Poisson equation](../../../../poisson-s-equation.md) and linearizing at $|ze\psi|\ll k_BT$ gives

$$
\nabla^2\psi=\kappa_{\mathrm{SI}}^2\psi,\qquad
\boxed{\kappa_{\mathrm{SI}}^2=\frac{2z^2e^2n_\infty}{\varepsilon_0\varepsilon_Rk_BT}=8\pi\ell_Bz^2n_\infty}.
$$

The extra $4\pi$ in the PDF denominator is inconsistent with those SI charge, permittivity and density conventions. Keeping the printed algebra would make its screening length $\sqrt{4\pi}$ times the SI value at the same ion density. No numerical screening length is required here, and the qualitative dependence $\kappa^{-1}\propto n_\infty^{-1/2}$ is the same in either normalization. Added salt shortens the range of repulsion, allowing the attractive potential to capture particles more readily.

**Interaction-potential sketches.** Let $h$ be the surface separation between two spheres of radius $a$. A useful schematic [DLVO theory](../../../../dlvo-theory.md) potential has the form

$$
U(h)\simeq B e^{-\kappa h}-\frac{A_Ha}{12h},
$$

away from the microscopic contact region. Here $A_H>0$ is a [Hamaker constant](../../../../hamaker-constant.md); excluded-core repulsion and molecular details regularize contact. The exponential is the double-layer repulsion and the inverse-gap term the short-gap [Van der Waals force](../../../../van-der-waals-force.md) contribution. A fixed $B$ illustrates the changing screening range; actual charge regulation can change the repulsive amplitude as well.

At low salt there is a high positive barrier between a deep primary minimum near contact and the dispersed state at $U(\infty)=0$. A shallow secondary minimum can occur outside the barrier and support weak reversible association. Increasing salt narrows the repulsive range and lowers the barrier. Thermally activated primary aggregation becomes appreciable when the barrier is only a few $k_BT$; the idealized barrier-free condition defines the fast-aggregation threshold associated with the [critical coagulation concentration](../../../../critical-coagulation-concentration.md). Above that threshold, collisions can result in rapid capture in the primary minimum.

<a id="section-b/b2/image-original-schematic-dlvo-potentials-as-screening-increases"></a>
![](../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018-scm-dlvo-potentials.png)

**[Figure 1](#section-b/b2/image-original-schematic-dlvo-potentials-as-screening-increases). Original schematic DLVO potentials as screening increases**. Illustrative dimensionless amplitudes show the barrier and outer attractive minimum; the near-contact primary well extends below the plotted range. These curves do not determine a material-specific coagulation concentration.

**Aggregate structures.** Well above the [critical coagulation concentration](../../../../critical-coagulation-concentration.md), the sticking probability is close to one. In [diffusion-limited cluster aggregation](../../../../diffusion-limited-cluster-aggregation.md), the first encounter attaches particles or clusters at accessible outer branches before they can explore many alternative configurations. The result is an open, tenuous structure. Typical ideal three-dimensional cluster models have [mass fractal dimension](../../../../mass-fractal-dimension.md) $d_f\simeq1.8$.

Near the threshold on its lower-salt, slow-aggregation side, a remaining barrier makes most encounters unsuccessful. [Reaction-limited cluster aggregation](../../../../reaction-limited-cluster-aggregation.md) then permits repeated approaches and orientations before attachment, commonly giving denser clusters with $d_f\simeq2.1$. Since particle count scales as $N\propto(R_g/a)^{d_f}$, the larger exponent means more particles at a given large cluster size. This explanation does not require already formed bonds to rearrange: unsuccessful encounters themselves alter which configurations eventually bind.

The side of the threshold matters. At the ideal barrier-free threshold itself, or just above it, aggregation can already be diffusion limited; proximity to the [critical coagulation concentration](../../../../critical-coagulation-concentration.md) alone does not universally imply a denser reaction-limited structure. The quoted dimensions are typical of irreversible approximately isotropic cluster models, not exact values for every colloid. Strong bond rearrangement or anisotropic attractions can change this comparison.

## ↑ Ancestors (13)

1. [B2](../b2.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
