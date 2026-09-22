<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [coupled quantum rotor chain](../../../../../coupled-quantum-rotor-chain.md) has a compact phase and conjugate integer number $n_j=\ell_j/\hbar$. Expanding the cosine gives

$$
H\simeq-NJ+\sum_j\left[\frac{\ell_j^2}{2I}+\frac J2(\phi_{j+1}-\phi_j)^2\right].
$$

In the phase-space [Euclidean path integral](../../../../../euclidean-path-integral.md), using inverse-energy time, each rotor has the action term $\ell_j^2/(2I)-i\ell_j\dot\phi_j/\hbar$. Completing its Gaussian square produces $I\dot\phi_j^2/(2\hbar^2)$. Equivalently, apply the short-time free-rotor kernel locally and retain winding sectors. The smooth-sector continuum limit at unit spacing is consequently

$$
\boxed{Z\simeq e^{\beta NJ}\int\mathcal D\phi\,e^{-\mathcal S},\qquad
\mathcal S=\int_0^\beta d\tau\int dx\left[\frac{I}{2\hbar^2}(\partial_\tau\phi)^2+\frac J2(\partial_x\phi)^2\right].}
$$

The overall constant is omitted when the reference bond energy is subtracted. **With the same physical J as the Hamiltonian, the printed spatial coefficient has an extra factor $1/\hbar^2$.** The [imaginary-time normalization for a coupled rotor chain](../../../../../imaginary-time-normalization-for-a-coupled-rotor-chain.md) requires $\hbar^2J/2$ inside a bracket with common prefactor $1/\hbar^2$. Setting $\hbar=1$ hides the discrepancy; it cannot establish the printed formula with explicit physical units.

Returning to physical time gives $I\partial_t^2\phi=J\partial_x^2\phi$. The [harmonic phase mode of a quantum rotor chain](../../../../../harmonic-phase-mode-of-a-quantum-rotor-chain.md) therefore has

$$
\boxed{\omega(k)=2\sqrt{J/I}\,|\sin(k/2)|\simeq c|k|,\qquad
c=\sqrt{J/I},\qquad E_k=\hbar\omega(k).}
$$

This is a gapless sound-like collective phase mode, analogous to neutral [superfluid](../../../../../superfluid.md) sound. In [rotor-chain phase-number hydrodynamics](../../../../../rotor-chain-phase-number-hydrodynamics.md), number fluctuations supply the compressibility and the intersite coupling supplies [phase stiffness](../../../../../phase-stiffness.md). The mode is a phase-density oscillation, not a free single-rotor transition. The [global phase zero mode of a finite rotor chain](../../../../../global-phase-zero-mode-of-a-finite-rotor-chain.md) is a compact rotor with inertia NI, which should not be counted as an independent zero-frequency oscillator.

The [compactness qualification of a harmonic rotor chain](../../../../../compactness-qualification-of-a-harmonic-rotor-chain.md) matters here. The smooth harmonic theory requires small neighbouring phase differences and cannot settle the entire strong-fluctuation phase diagram. In one dimension its zero-temperature phase variance grows logarithmically, so the gapless regime has algebraic phase correlations rather than a true condensate. Thermal fluctuations and compact [phase slips](../../../../../phase-slip.md) require additional care; phase-slip proliferation can produce a gapped phase outside the Gaussian regime. [§5.2, rotor phase/number variables and limits of smooth superfluid theory](../../../../../physics-215c-quantum-field-theory-part-3-by-john-mcgreevy.md)

## ↑ Ancestors (14)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
