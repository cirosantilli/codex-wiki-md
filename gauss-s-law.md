<h1 id="gauss-s-law">Gauss's law</h1>

↑ **Parent:** [Maxwell equations](maxwell-equations-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss's_law)

[Gauss's law](gauss-s-law.md) relates the [electric field](electric-field-split.md) on a [closed surface](closed-surface.md) to the net [electric charge](electric-charge-split.md) inside it. In [SI](international-system-of-units.md) units, with outward [unit normal](unit-normal.md) $\mathbf n$,

$$
\boxed{\oint_{\partial V}\mathbf E\cdot\mathbf n\,dS=\frac{Q_{\mathrm{enclosed}}}{\varepsilon_0},\qquad Q_{\mathrm{enclosed}}=\int_V\rho\,dV.}
$$

Here $\rho$ describes a volume [charge density](charge-density.md), and $\varepsilon_0$ is the [vacuum permittivity](vacuum-permittivity.md); for ideal point or surface charges, use the enclosed [electric charge](electric-charge-split.md) directly rather than an ordinary volume-density integral. The left side is [electric flux](electric-flux.md): the [surface integral](surface-integral.md) of the outward normal component of the [electric field](electric-field-split.md). Field directed outward contributes positively; field directed inward contributes negatively. The equality uses net signed [electric charge](electric-charge-split.md), so positive and negative enclosed charges can cancel. The [Gaussian surface](gaussian-surface.md) is an imagined accounting boundary, not necessarily a material object. See [OpenStax, explaining Gauss's law](https://openstax.org/books/university-physics-volume-2/pages/6-2-explaining-gausss-law).

Where the [electric field](electric-field-split.md) and [charge density](charge-density.md) are smooth, the local statement is $\nabla\cdot\mathbf E=\rho/\varepsilon_0$. The [divergence theorem](divergence-theorem.md) connects this [divergence](divergence.md) to the [surface integral](surface-integral.md). This is the satisfying connection between local sources and global accounting: a surface can register how much net [electric charge](electric-charge-split.md) it encloses without revealing where that charge is located within it. A [point charge](point-charge.md) requires care with the singular field at its position; the integral formulation remains useful with a boundary that avoids the charge.

The law fixes total [electric flux](electric-flux.md), rather than every value of the [electric field](electric-field-split.md). In an uncharged region, a uniform [electric field](electric-field-split.md) $\mathbf E=(E_0,0,0)$ crosses a cube of side $\ell$. Its left and right faces contribute $-E_0\ell^2$ and $+E_0\ell^2$; the other four faces contribute zero. Thus **the net electric flux is zero while the electric field is nonzero everywhere**. Charges outside a [Gaussian surface](gaussian-surface.md) can change the field on it without changing its net [electric flux](electric-flux.md). Conversely, fields cannot generally be reconstructed from enclosed [electric charge](electric-charge-split.md) alone. [Electrostatics](electrostatics-split.md) also requires the [electric field](electric-field-split.md) to be the negative [gradient](gradient.md) of an [electric potential](electric-potential.md), with appropriate boundary information. This distinction is emphasized in [Feynman lectures II.5, application of Gauss' law](https://www.feynmanlectures.caltech.edu/II_05.html).

<a id="image-zero-net-flux-can-coexist-with-a-nonzero-uniform-field-and-equal-enclosed-charge-can-give-different-field-magnitudes-on-different-spheres"></a>
![](gaussian-flux-and-field.png)

**[Figure 6](#image-zero-net-flux-can-coexist-with-a-nonzero-uniform-field-and-equal-enclosed-charge-can-give-different-field-magnitudes-on-different-spheres). Zero net flux can coexist with a nonzero uniform field, and equal enclosed charge can give different field magnitudes on different spheres**.

[Spherical symmetry](spherical-symmetry.md) supplies the extra information needed for a particularly simple calculation. An isolated [spherically symmetric](spherical-symmetry.md) charge distribution in vacuum produces a radial [electric field](electric-field-split.md), constant in magnitude on each concentric [sphere](sphere.md). Its [electric flux](electric-flux.md) is therefore $4\pi r^2E_r(r)$, giving

$$
E_r(r)=\frac{Q_{\mathrm{enclosed}}(r)}{4\pi\varepsilon_0r^2}.
$$

Outside the distribution, doubling $r$ quadruples the [surface area](surface-area.md) and divides the radial [electric field](electric-field-split.md) by four, while the [electric flux](electric-flux.md) stays $Q/\varepsilon_0$. The inverse-square dependence is an area-dilution result. The [electric field of a uniformly charged ball](electric-field-of-a-uniformly-charged-ball.md) and [electric field of a uniformly charged spherical shell](electric-field-of-a-uniformly-charged-spherical-shell.md) show that the same total charge can give different interior fields. These symmetry arguments and their limits are developed in [OpenStax, applying Gauss's law](https://openstax.org/books/university-physics-volume-2/pages/6-3-applying-gausss-law).

**Table of contents**

- [Net charge from the asymptotic radial electric field](net-charge-from-the-asymptotic-radial-electric-field.md)
- [Electric field for a radial power-law charge density](electric-field-for-a-radial-power-law-charge-density.md)
- [Electric field of a uniformly charged ball](electric-field-of-a-uniformly-charged-ball.md)
- [Electric field of a uniformly charged spherical shell](electric-field-of-a-uniformly-charged-spherical-shell.md)
- [Hyperbolic-space Coulomb field](hyperbolic-space-coulomb-field.md)
- [Force between hemispheres of a uniformly charged ball](force-between-hemispheres-of-a-uniformly-charged-ball.md)
- [Gaussian surface](gaussian-surface.md)
- [Gaussian pillbox](gaussian-pillbox.md)

## ↑ Ancestors (5)

1. [Maxwell equations](maxwell-equations-split.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (115)

- [Breakdown-limited energy of a conducting sphere](breakdown-limited-energy-of-a-conducting-sphere.md)
- [Charge conservation](charge-conservation.md)
- [Charge continuity equation](charge-continuity-equation.md)
- [Charge relaxation](charge-relaxation.md)
- [Charged sheet between grounded parallel plates](charged-sheet-between-grounded-parallel-plates.md)
- [Conducting sphere](conducting-sphere.md)
- [Conductor in electrostatic equilibrium](conductor-in-electrostatic-equilibrium.md)
- [Coulomb's law](coulomb-s-law.md)
- [Cylindrical counterion-only Poisson-Boltzmann profile](cylindrical-counterion-only-poisson-boltzmann-profile.md)
- [Cylindrical screening charge](cylindrical-screening-charge.md)
- [Debye-Hückel potential of a charged sphere](debye-huckel-potential-of-a-charged-sphere.md)
- [Displacement current](displacement-current.md)
- [Electric field for a radial power-law charge density](electric-field-for-a-radial-power-law-charge-density.md)
- [Electric field of a hydrogen ground-state electron cloud](electric-field-of-a-hydrogen-ground-state-electron-cloud.md)
- [Electric field of a uniformly charged ball](electric-field-of-a-uniformly-charged-ball.md)
- [Electric flux](electric-flux.md)
- [Electromagnetic wave equation](electromagnetic-wave-equation.md)
- [Electrostatic boundary conditions at a conductor](electrostatic-boundary-conditions-at-a-conductor.md)
- [Electrostatic energy of alternating-charge concentric shells](electrostatic-energy-of-alternating-charge-concentric-shells.md)
- [Electrostatics](electrostatics-split.md)
- [Faraday's ice pail experiment](faraday-s-ice-pail-experiment.md)
- [Force between hemispheres of a uniformly charged ball](force-between-hemispheres-of-a-uniformly-charged-ball.md)
- [Full-depletion capacitance of a symmetric junction slab](full-depletion-capacitance-of-a-symmetric-junction-slab.md)
- [Gauss law constraint in gauge theory](gauss-law-constraint-in-gauge-theory.md)
- [Gauss's law](gauss-s-law.md)
- [Gaussian surface](gaussian-surface.md)
- [Line charge](line-charge.md)
- [Lossless coaxial line parameters](lossless-coaxial-line-parameters.md)
- [Maxwell equations](maxwell-equations-split.md)
- [Net charge from the asymptotic radial electric field](net-charge-from-the-asymptotic-radial-electric-field.md)
- [Osmotic stress in a symmetric electric double layer](osmotic-stress-in-a-symmetric-electric-double-layer.md)
- [Parallel current sheets with a resistive termination](parallel-current-sheets-with-a-resistive-termination.md)
- [Parallel-plate capacitor](parallel-plate-capacitor.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-59/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/16g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/6g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/34e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/17e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/34e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/6a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/11c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/11c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/11a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/18a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-43/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-75/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/16d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/7d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/18c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-3/11c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/7c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/36d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1/16a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/16d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3/15d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-314/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4/36d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-1/15b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-2/4b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-3/11a/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-3/11a/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/3/d/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2012/paper-1/4/a/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2013/paper-1/1/c/i/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2017/4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-b/b6/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1/section-a/a1/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-b/b6/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-a/a2/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1/section-a/a1/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1/section-b/b6/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-a/a4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-b/b7/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/section-e/e14/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/section-e/e14/a/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-e/e15/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/section-a/4/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-e/e15/a/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-e/e15/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-e/14/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-e/15/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/section-b/10/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/section-b/b6/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-a/a3/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-a/a3/c/iii/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2012/paper-1/2/c/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/6/c/solution.md)
- [Permittivity](permittivity-split.md)
- [Potential of an inverse-radius spherical charge density](potential-of-an-inverse-radius-spherical-charge-density.md)
- [Radiation gauge](radiation-gauge.md)
- [Relativistic charge density of counterstreaming beams](relativistic-charge-density-of-counterstreaming-beams.md)
- [Spherical capacitor](spherical-capacitor.md)
