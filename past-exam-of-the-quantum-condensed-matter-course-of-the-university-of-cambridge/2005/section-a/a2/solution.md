<h1 id="section-a/a2/solution">Solution</h1>

↑ **Parent:** [A2](../a2.md)

For a dilute suspended sphere in [Stokes flow](../../../../stokes-flow-split.md), the translational friction coefficient is $f_h=6\pi\eta R$, with dynamic viscosity $\eta$ and hydrodynamic radius $R$. To derive the diffusion-friction relation, put particles in a weak conservative force $F=-U'$. Their drift velocity is $F/f_h$, while the diffusive flux is $-D\,dc/dx$. At equilibrium the [Boltzmann distribution](../../../../boltzmann-distribution.md) gives $c'=-cU'/(k_BT)=cF/(k_BT)$. Zero total flux therefore gives $cF/f_h-DcF/(k_BT)=0$, hence the [Stokes–Einstein relation](../../../../stokes-einstein-relation.md)

$$
\boxed{D=\frac{k_BT}{f_h}=\frac{k_BT}{6\pi\eta R}.}
$$

Here $k_B$ is the [Boltzmann constant](../../../../boltzmann-constant.md), $T$ absolute temperature and $D$ the translational [diffusion coefficient](../../../../diffusion-coefficient.md). The sphere, no-slip continuum-fluid and dilute thermal-equilibrium assumptions enter through the drag law and flux balance.

At $T=293.15\,\mathrm K$ and the supplied viscosity, the predicted product is $D R=2.1472\times10^{-19}\,\mathrm{m^3\,s^{-1}}$. The derived predictions and radii inferred from the measured diffusion coefficients are:

| Protein | Predicted $D/(10^{-9}\,\mathrm{m^2\,s^{-1}})$ | Inferred [hydrodynamic radius](../../../../hydrodynamic-radius.md) / nm |
| --- | --- | --- |
| [Ribonuclease](../../../../ribonuclease.md) | $0.119$ | $2.15$ |
| [Beta-lactoglobulin](../../../../beta-lactoglobulin.md) | $0.0795$ | $2.68$ |
| [Haemoglobin](../../../../hemoglobin.md) | $0.0693$ | $3.07$ |
| [Collagen](../../../../collagen.md) | $0.00693$ | $30.7$ |

The last three agree closely at the precision of the supplied data. The ribonuclease diffusion coefficient is about $16\%$ below the spherical prediction, corresponding to a larger frictional radius than the stated radius. Hydration, shape, a different operational radius and coarse measurement precision can matter; molar mass is not an independent parameter in the spherical diffusion law. A compact constant-density globule would have $R\propto M^{1/3}$, whereas collagen's large frictional radius relative to its mass is consistent with an extended nonspherical molecule. The inferred [Stokes radius](../../../../hydrodynamic-radius.md) is a friction-equivalent radius, not automatically a geometric half-length.

In [analytical ultracentrifugation](../../../../analytical-ultracentrifugation.md), scan the radial protein concentration while a rotor spins at known angular speed $\omega$. Optical absorbance or refractive-index interference records a moving sedimentation boundary and its diffusive broadening.[Radial scans during rotation, absorbance spectrophotometry and Rayleigh interference detection](../../../../optical-systems-used-for-auc-by-beckman-coulter-life-sciences.md) With solvent density $\rho_s$, partial specific volume $\bar v$ and molar mass $M$ in $\mathrm{kg\,mol^{-1}}$, the buoyant mass is $m_b=M(1-\bar v\rho_s)/N_A$. Force balance gives $f_hv=m_b\omega^2r$, so the [sedimentation coefficient](../../../../sedimentation-coefficient.md) is $s=v/(\omega^2r)=m_b/f_h$. A boundary trajectory gives $s=\omega^{-2}d\ln r/dt$; diffusion gives $f_h=k_BT/D$.

Combining them gives the [molar mass from sedimentation and diffusion](../../../../molar-mass-from-sedimentation-and-diffusion.md):

$$
\boxed{M=\frac{R_{\rm gas}Ts}{D(1-\bar v\rho_s)},\qquad R_h=\frac{k_BT}{6\pi\eta D}.}
$$

Known mass and buoyancy can instead determine friction from $s$ alone, and comparison with a compact sphere tests shape or hydration. In [sedimentation equilibrium](../../../../sedimentation-equilibrium.md), the stationary radial profile obeys $d\ln c/d(r^2)=m_b\omega^2/(2k_BT)$, providing buoyant mass without a friction model. This is a sedimentation-diffusion balance in a uniform solvent, rather than density-gradient banding at an isopycnic point.

## ↑ Ancestors (13)

1. [A2](../a2.md)
2. [Section A](../../section-a.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
