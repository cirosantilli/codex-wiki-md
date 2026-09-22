<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A charged biological [molecule](../../../../molecule-split.md) attracts counterions and repels [ions](../../../../ion.md) of the same sign. Thermal [diffusion](../../../../diffusion.md) opposes complete localization, producing a mobile ionic atmosphere whose charge partly cancels the [molecule](../../../../molecule-split.md)'s [electric field](../../../../electric-field-split.md) at larger distances. Solvent polarization also reduces the field through its [permittivity](../../../../permittivity-split.md), but that dielectric response is distinct from the mobile-[ion](../../../../ion.md) screening cloud.

For an ideal [electrolyte](../../../../electrolyte.md) in [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) at [temperature](../../../../temperature-split.md) $T$, an [ion](../../../../ion.md) of valence $z_i$ has local [number density](../../../../number-density.md)

$$
n_i(\mathbf r)=n_i^{\infty}\exp\left[-\frac{z_ie\phi(\mathbf r)}{k_BT}\right].
$$

For $|z_ie\phi|\ll k_BT$, linearization about an electroneutral bulk gives

$$
\rho_{\rm ions}\simeq-\phi\frac{\sum_i n_i^{\infty}z_i^2e^2}{k_BT},\qquad
\nabla^2\phi=\kappa^2\phi,\qquad
\boxed{\lambda_D=\kappa^{-1}=\sqrt{\frac{\epsilon k_BT}{e^2\sum_i n_i^{\infty}z_i^2}}.}
$$

This is the [Debye length](../../../../debye-length.md). Here $n_i^{\infty}$ counts _each species separately_ and $\epsilon$ is the absolute solvent [permittivity](../../../../permittivity-split.md). For a point charge $Q$, outside its immediate molecular environment the linearized solution is

$$
\boxed{\phi(r)=\frac{Q}{4\pi\epsilon r}e^{-r/\lambda_D}.}
$$

It is a screened potential, not a claim that the molecular charge has disappeared.

In terms of [ionic strength](../../../../ionic-strength.md) $I=\tfrac12\sum_i c_i z_i^2$ with $c_i$ in $\mathrm{mol\,L^{-1}}$, the density sum is $2N_A10^3I$, so

$$
\lambda_D=\sqrt{\frac{\epsilon k_BT}{2e^2N_A10^3I}}.
$$

In water near $298\,\mathrm K$, $\lambda_D\simeq0.304\,\mathrm{nm}/\sqrt{I/(1\,\mathrm{mol\,L^{-1}})}$: about $9.6\,\mathrm{nm}$ at $1\,\mathrm{mM}$ and $0.79\,\mathrm{nm}$ at $0.15\,\mathrm M$. Increasing [ion](../../../../ion.md) density or valence shortens the range; [temperature](../../../../temperature-split.md) and solvent [permittivity](../../../../permittivity-split.md) also matter. The displayed [temperature](../../../../temperature-split.md) dependence holds at fixed [permittivity](../../../../permittivity-split.md), which itself changes with [temperature](../../../../temperature-split.md) in water.

The derivation assumes dilute mobile [ions](../../../../ion.md), a continuum uniform dielectric and weak potentials. Near highly charged [DNA](../../../../deoxyribonucleic-acid.md) or [protein](../../../../protein-split.md) surfaces, nonlinear [Poisson-Boltzmann equation](../../../../poisson-boltzmann-equation.md) behaviour, [counterion condensation](../../../../counterion-condensation.md), finite [ion](../../../../ion.md) sizes, specific binding and correlations can matter. At physiological salt the predicted length approaches molecular scales, so the formula is a useful far-field scale with limited microscopic accuracy, rather than a complete account of the first hydration layer.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
