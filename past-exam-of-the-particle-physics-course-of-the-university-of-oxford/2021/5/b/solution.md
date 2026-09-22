<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Independent fluctuations add as [variances](../../../../variance-split.md). A useful parametrization of the [electromagnetic calorimeter](../../../../electromagnetic-calorimeter.md) [energy resolution](../../../../energy-resolution.md) is

$$
\boxed{\left(\frac{\sigma_E}{E}\right)^2=\frac{a^2}{E/\mathrm{GeV}}+\frac{b^2}{(E/\mathrm{GeV})^2}+c^2.}
$$

The convention makes $a,b,c$ dimensionless when $E$ is inserted in GeV. The three terms describe different mechanisms.

The stochastic term comes from fluctuations in the [electromagnetic shower](../../../../electromagnetic-shower.md), scintillation production and detected photoelectron counts. If the number of detected photoelectrons is $N=kE$, [Poisson distribution](../../../../poisson-distribution.md) gives $\sigma_N=\sqrt N$, hence $\sigma_E/E=1/\sqrt{kE}\propto E^{-1/2}$. A sampling [electromagnetic calorimeter](../../../../electromagnetic-calorimeter.md) also has fluctuations in the fraction deposited in its active material, contributing to the same approximate scaling. A homogeneous detector suppresses that sampling contribution.

The noise term represents approximately fixed absolute electronics and dark-current noise for a chosen reconstruction window. Additional [collision pileup](../../../../collision-pileup.md) fluctuations can behave similarly over a specified operating range. A nearly constant $\sigma_E$ gives $\sigma_E/E\propto E^{-1}$.

The constant term describes residual fractional cell-calibration errors, gain drifts, temperature dependence, nonuniform light collection, dead material, and imperfect correction for longitudinal and transverse leakage. These effects often scale approximately with the incident [energy](../../../../energy-split.md), so they approach a constant fractional error. For [electrons](../../../../electron.md), upstream [bremsstrahlung](../../../../bremsstrahlung.md) and conversion of the radiated [photons](../../../../photon.md) spread the deposit over multiple cells; material mapping and clustering are essential. Leakage and material losses can also produce non-Gaussian tails, so the three-term parametrization describes a resolution core rather than every feature of the response. Noise dominates at low [energy](../../../../energy-split.md), stochastic fluctuations at intermediate [energy](../../../../energy-split.md), and the constant term eventually limits performance.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
