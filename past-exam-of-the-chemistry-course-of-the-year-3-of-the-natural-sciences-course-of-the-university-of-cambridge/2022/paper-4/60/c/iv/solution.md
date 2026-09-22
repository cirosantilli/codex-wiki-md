<h1 id="60/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

At a Hartree-Fock stationary point the reference-single terms vanish. Expanding the normalized expectation through second order gives

$$
\mathcal E^{(2)}
=\sum_{ia,jb}\lambda_i^a\lambda_j^b
\left[
\langle\Phi_i^a|(\hat H-E_0)|\Phi_j^b\rangle
+\langle\Phi_0|\hat H|\Phi_{ij}^{ab}\rangle
\right].
$$

The reference-double term arises twice in the numerator and cancels the factor $1/2$ in the [wavefunction](../../../../../../wave-function-split.md). The normalization subtracts $E_0\sum_{ia}(\lambda_i^a)^2$.

Using [Slater-Condon rules](../../../../../../slater-condon-rules.md) in canonical orbitals,

$$
\langle\Phi_i^a|(\hat H-E_0)|\Phi_j^b\rangle
=(\gamma_a-\gamma_i)\delta_{ij}\delta_{ab}
+\langle aj|ib\rangle-\langle aj|bi\rangle,
$$

and $\langle\Phi_0|\hat H|\Phi_{ij}^{ab}\rangle
=\langle ab|ij\rangle-\langle ab|ji\rangle$. Combining them gives the requested $X_{ij}^{ab}$. The orbital energies are

$$
\gamma_p=h_{pp}+
\sum_{k\ {\rm occ}}\left(\langle pk|pk\rangle-\langle pk|kp\rangle\right),
$$

for either occupied or virtual $p$. Diagonalizing the occupied and virtual Fock blocks is the suitable orbital choice that makes the delta form valid for coincident as well as distinct indices.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [60](../../../60.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
