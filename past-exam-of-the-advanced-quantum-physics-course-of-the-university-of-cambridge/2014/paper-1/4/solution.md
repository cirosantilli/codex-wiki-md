<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The quoted expansion is [nondegenerate perturbation theory](../../../../nondegenerate-perturbation-theory.md) for a known isolated eigenstate of a time-independent [Hamiltonian](../../../../hamiltonian.md). A useful small-mixing condition is $|\langle k|H_1|i\rangle|\ll|E_i-E_k|$ for coupled states. First order is a diagonal expectation value; second order describes virtual mixing. A degenerate or nearly degenerate coupled subspace must first be treated by diagonalization there. Symmetry can eliminate terms, and convergence still needs checking. Ground-state second-order shifts are nonpositive because all denominators are negative.[Non-degenerate perturbation theory and its breakdown at coupled degeneracies](../../../../quantum-mechanics-by-richard-fitzpatrick.md)

For the [rotational Stark effect](../../../../rotational-stark-effect.md), $H_1=-pE\cos\theta$, where $\theta$ is the **[polar angle](../../../../polar-angle.md) to the field**. The source calls it azimuthal, which is inconsistent with this coupling. Rotor states have [parity](../../../../parity.md) $(-1)^J$, while $\cos\theta$ is odd, so every first-order [matrix element](../../../../matrix-element.md) within one fixed-$J$ manifold vanishes. The $m$ degeneracy therefore causes no first-order splitting.

Only $J\pm1$ with the same $m$ contribute in second order. Using their [energy](../../../../energy-split.md) differences $2BJ$ and $-2B(J+1)$,

$$
\delta E_{Jm}^{(2)}=\frac{(pE)^2}{2B}\left[\frac{J^2-m^2}{J(2J-1)(2J+1)}-\frac{(J+1)^2-m^2}{(J+1)(2J+1)(2J+3)}\right].
$$

For $J\ge1$ this simplifies to the [quadratic Stark shift of a polar linear rotor](../../../../quadratic-stark-shift-of-a-polar-linear-rotor.md),

$$
\boxed{\delta E_{Jm}^{(2)}=\frac{(pE)^2[J(J+1)-3m^2]}{2BJ(J+1)(2J-1)(2J+3)}.}
$$

For $J=0$, only $J'=1,m=0$ contributes, with squared angular [matrix element](../../../../matrix-element.md) $1/3$ and denominator $-2B$:

$$
\boxed{\delta E_{00}^{(2)}=-\frac{(pE)^2}{6B}.}
$$

Here $B$ is the rotational [energy](../../../../energy-split.md) constant, unlike the [magnetic field](../../../../magnetic-field-split.md) in Question3.

The unperturbed line gives $B/h=6.08\,\mathrm{GHz}$. The $J=1$ shifts are $(pE)^2/(10B)$ for $m=0$ and $-(pE)^2/(20B)$ for $m=\pm1$. Subtracting the common lower-state shift gives transition shifts $4(pE)^2/(15Bh)$ and $7(pE)^2/(60Bh)$. Their separation determines the [dipole moment from a rotational Stark doublet](../../../../dipole-moment-from-a-rotational-stark-doublet.md):

$$
\Delta\nu=\frac{3(pE)^2}{20Bh},\qquad\boxed{p=\frac hE\sqrt{\frac{20}{3}\frac Bh\Delta\nu}=2.39\times10^{-30}\,\mathrm{C\,m}\simeq0.717\,\mathrm D.}
$$

The $\mathrm D$ unit is the [debye](../../../../debye-unit.md). Using external $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$ and $1\,\mathrm D=3.33564\times10^{-30}\,\mathrm{C\,m}$ gives $pE/B\simeq0.0593$, consistent with weak-field perturbation theory. The two shifted [frequencies](../../../../frequency.md) are about $12.165707$ and $12.162497\,\mathrm{GHz}$; [polarization](../../../../polarization-waves.md) selects $\Delta m=0$ or $\pm1$. The inferred value is a magnitude; these shifts do not determine the dipole's sign.[Exact SI Planck constant](../../../../codata-recommended-values-of-the-fundamental-physical-constants-2022-by-national-institute-of-standards-and-technology.md)[Section5: [debye](../../../../debye-unit.md) conversion](../../../../triatomic-spectral-database-by-national-institute-of-standards-and-technology.md)

<a id="4/image-opposite-parity-mixing-produces-quadratic-rotor-shifts-and-a-polarization-dependent-rotational-doublet"></a>
![](../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2014/paper-1-aqp2014-rotor-stark-shifts.png)

**[Figure 3](#4/image-opposite-parity-mixing-produces-quadratic-rotor-shifts-and-a-polarization-dependent-rotational-doublet). Opposite-parity mixing produces quadratic rotor shifts and a polarization-dependent rotational doublet**. [Source](paper-1-aqp2014-rotor-stark-shifts.py).

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
