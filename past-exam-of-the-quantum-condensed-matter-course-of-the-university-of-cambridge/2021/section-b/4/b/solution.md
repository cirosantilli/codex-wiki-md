<h1 id="section-b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use one orthonormalized localized [atomic orbital](../../../../../atomic-orbital.md) $|j\rangle$ at each position $ja$. In the nearest-neighbour [tight-binding model](../../../../../tight-binding.md), translation invariance gives the on-site energy and real [hopping integral](../../../../../hopping-integral.md)

$$
E_0=\langle j|H|j\rangle,\qquad
 t=\langle j|H|j+1\rangle=\langle j+1|H|j\rangle.
$$

The [Bloch state](../../../../../bloch-state.md) is

$$
|k\rangle=\frac1{\sqrt N}\sum_j e^{ikja}|j\rangle.
$$

Since $H|j\rangle=E_0|j\rangle+t|j-1\rangle+t|j+1\rangle$, shifting the two summation indices gives

$$
H|k\rangle=[E_0+te^{ika}+te^{-ika}]|k\rangle,
\qquad\boxed{E(k)=E_0+2t\cos(ka).}
$$

The [hopping integral](../../../../../hopping-integral.md) is an energy, and its sign sets whether $k=0$ is a minimum or maximum. $E_0$ is the diagonal matrix element in the crystal Hamiltonian, which can differ from an isolated-atom energy.

The [orthogonal tight-binding approximation](../../../../../orthogonal-tight-binding-approximation.md) matters. If raw neighbouring orbitals retain a nonzero [orbital overlap](../../../../../orbital-overlap.md) $s$ in their normalization, projection instead gives a [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md) and the [nonorthogonal nearest-neighbour tight-binding band](../../../../../nonorthogonal-nearest-neighbour-tight-binding-band.md) $E(k)=[E_0+2h\cos(ka)]/[1+2s\cos(ka)]$. The stated cosine band follows after orthonormalization and nearest-neighbour truncation, or after neglecting that overlap metric while retaining the hopping it motivates.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
