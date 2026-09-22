<h1 id="a6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the adsorbed [lattice gas](../../../../../lattice-gas.md), the [Helmholtz free energy](../../../../../helmholtz-free-energy.md) is

$$
A_{\rm ads}=-k_{\rm B}T\left[\ln\binom MN+N\ln z\right].
$$

Use [Stirling's approximation](../../../../../stirling-formula.md) with $M,N,M-N$ large, then differentiate at fixed $M,T,B$. Writing [surface coverage](../../../../../surface-coverage.md) as $\theta=N/M$ gives the [adsorption chemical potential](../../../../../adsorption-chemical-potential.md)

$$
\boxed{\mu_{\rm ads}=k_{\rm B}T\ln\frac{\theta}{1-\theta}
-k_{\rm B}T\ln z
=-E_b-k_{\rm B}T\ln(2\cosh x)
+k_{\rm B}T\ln\frac{\theta}{1-\theta}.}
$$

The occupation ratio comes from site-mixing [entropy](../../../../../entropy-split.md); it is essential near saturation.

Let $N_g$ be the number of free atoms and $n_g=N_g/V$. In the field-free gas, both [spin](../../../../../spin.md) states have zero [energy](../../../../../energy-split.md), so the one-atom [partition function](../../../../../canonical-partition-function.md) is $q_g=2V/\Lambda^3$, where $\Lambda$ is the [thermal de Broglie wavelength](../../../../../thermal-de-broglie-wavelength.md). For a dilute [ideal gas](../../../../../ideal-gas-split.md),

$$
Q_g=\frac{(2V/\Lambda^3)^{N_g}}{N_g!},\qquad
A_g\simeq N_gk_{\rm B}T\left[\ln\frac{n_g\Lambda^3}{2}-1\right].
$$

Therefore

$$
\boxed{\mu_g=k_{\rm B}T\ln\frac{n_g\Lambda^3}{2}
=k_{\rm B}T\ln\frac{p\Lambda^3}{2k_{\rm B}T}.}
$$

The last equality uses $p=n_gk_{\rm B}T$. The bulk [spin degeneracy](../../../../../spin-degeneracy.md) is two even though the bulk [magnetic field](../../../../../magnetic-field-split.md) vanishes: degeneracy is not the absence of [spin](../../../../../spin.md) states.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [A6](../../a6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
