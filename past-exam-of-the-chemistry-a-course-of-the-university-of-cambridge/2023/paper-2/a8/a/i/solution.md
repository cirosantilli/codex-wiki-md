<h1 id="a8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an ideal mixture, the [Helmholtz free energy](../../../../../../helmholtz-free-energy.md) is a sum over species. At fixed $T,V$ and all other populations, the [molecular partition function](../../../../../../molecular-partition-function.md) $q_i$ does not depend on $N_i$. Differentiating the contribution written using each species' own energy reference gives

$$
\frac{\partial}{\partial N_i}\left[-N_i k_BT\ln q_i+k_BT(N_i\ln N_i-N_i)\right]
=-k_BT\ln q_i+k_BT\ln N_i.
$$

The desired additive energy term requires a consistent [energy reference in molecular partition functions](../../../../../../energy-reference-in-molecular-partition-functions.md). Let $\varepsilon^{0,i}$ be the energy per molecule of species $i$ in its reference state, measured relative to a common chemical energy zero, and let $q_i$ sum excitations above that reference. Then

$$
q_i^{\rm abs}=e^{-\varepsilon^{0,i}/(k_BT)}q_i,
\qquad
A_i=N_i\varepsilon^{0,i}-N_i k_BT\ln q_i+k_BT(N_i\ln N_i-N_i).
$$

Therefore

$$
\boxed{\mu_i=\left(\frac{\partial A}{\partial N_i}\right)_{T,V,N_{j\ne i}}
=\varepsilon^{0,i}-k_BT\ln\frac{q_i}{N_i}}.
$$

One convenient choice is each species' rovibrational ground state, so the molecular reference includes its [zero-point energy](../../../../../../zero-point-energy.md). A different consistent reference is possible, but the corresponding [partition function](../../../../../../canonical-partition-function.md) must change. The offset cannot arise from differentiation of a formula that has already omitted it, and it must not be counted twice. These [chemical potentials](../../../../../../chemical-potential-split.md) are per particle; molar expressions instead use the [molar gas constant](../../../../../../molar-gas-constant.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [A8](../../../a8.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
