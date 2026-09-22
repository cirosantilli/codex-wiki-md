<h1 id="a6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat each species as a dilute classical ideal gas: molecules of the same species are indistinguishable, while different species are distinguishable. Let $N_i$ be the number of molecules of species $i$, $q_i(T,V)$ its [molecular partition function](../../../../../molecular-partition-function.md) with energies measured from a chosen internal reference, and $\varepsilon^{0,i}$ that reference energy per molecule relative to a common chemical energy convention. Then the mixture's [canonical partition function](../../../../../canonical-partition-function.md) factorizes:

$$
Q=\prod_i\frac{q_i^{N_i}}{N_i!}\exp[-\beta N_i\varepsilon^{0,i}],
\qquad \beta=\frac1{k_{\mathrm B}T}.
$$

The $N_i!$ corrects the overcounting of [indistinguishable particles](../../../../../indistinguishable-particles.md). The exponential restores the species-dependent reference energies that matter for reactions. Thus the [Helmholtz free energy](../../../../../helmholtz-free-energy.md) is

$$
A=-k_{\mathrm B}T\sum_i\left[N_i\ln q_i-\ln(N_i!)\right]
+\sum_iN_i\varepsilon^{0,i}.
$$

Using [Stirling's approximation](../../../../../stirling-formula.md), $\ln(N_i!)\simeq N_i\ln N_i-N_i$, and differentiating at fixed $T,V,N_{j\ne i}$ yields

$$
\boxed{\mu_i=\left(\frac{\partial A}{\partial N_i}\right)_{T,V,N_{j\ne i}}
=-k_{\mathrm B}T\ln\frac{q_i}{N_i}+\varepsilon^{0,i}.}
$$

The ideal-gas $q_i$ does not depend on the number of molecules, so no additional $\partial q_i/\partial N_i$ term appears. These are chemical potentials per molecule; multiply by the [Avogadro constant](../../../../../avogadro-constant.md) for a molar chemical potential. The result assumes the thermodynamic, nondegenerate-gas limit.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [A6](../../a6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
