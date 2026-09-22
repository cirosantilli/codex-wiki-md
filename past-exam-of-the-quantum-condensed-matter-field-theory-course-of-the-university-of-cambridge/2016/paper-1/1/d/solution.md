<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For occupations small compared with $S$, use $S^z=S-n$, $S^-\simeq\sqrt{2S}\,a^\dagger$ and $S^+\simeq\sqrt{2S}\,a$. The longitudinal bond contributes $-J\Delta S^2+JS\Delta(n_m+n_{m+1})+O(S^0)$; the transverse pair terms contribute $JS(a_ma_{m+1}+a_m^\dagger a_{m+1}^\dagger)+O(S^0)$. Thus the direct real-space expansion is

$$
H_2=-J\Delta NS^2+JS\sum_m\{2\Delta n_m+a_ma_{m+1}+a_m^\dagger a_{m+1}^\dagger\}.
$$

Take $a_m=N^{-1/2}\sum_k e^{ikm}a_k$, with $k=2\pi j/N$ over one full [Brillouin zone](../../../../../brillouin-zone.md) and the lattice spacing set to one in $k$. Symmetrizing $k$ and $-k$ changes the phase in the pair sum to $\cos k$, giving

$$
H_2=-J\Delta NS^2+JS\sum_k\{2\Delta a_k^\dagger a_k+\cos k(a_ka_{-k}+a_k^\dagger a_{-k}^\dagger)\}.
$$

[normal ordering](../../../../../normal-ordering.md) the second [Nambu spinor](../../../../../nambu-spinor.md) component then yields

$$
\boxed{H_2=-J\Delta NS(S+1)+JS\sum_k(a_k^\dagger\ \ a_{-k})\begin{pmatrix}\Delta&\cos k\\\cos k&\Delta\end{pmatrix}\binom{a_k}{a_{-k}^\dagger}.}
$$

**The printed matrix has a factor-of-two error on its diagonal.** With a full-zone sum its printed $2\Delta$ would produce $4\Delta a_k^\dagger a_k$, and even its vacuum expectation would differ from the direct expansion by $J\Delta NS$. A half-zone convention cannot repair both coefficients: one must then group each $k,-k$ pair and double its off-diagonal pair coefficient as well. The formula above follows from the specified [Hamiltonian](../../../../../hamiltonian.md) and has the expected gapless isotropic limit; subsequent physical results use this consistent expansion. Terms quartic in [bosons](../../../../../boson.md) first enter at order $S^0$.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
