<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the Grassmann spin density $\mathbf j_n=\bar\psi_n\boldsymbol\sigma\psi_n$. The [Pauli matrices](../../../../../pauli-matrices.md) and Grassmann reordering give

$$
\mathbf j_n^2=-6D_n,\qquad 3UD_n=-\frac U2\mathbf j_n^2.
$$

For example $j_z^2=-2D_n$; each of the other two components gives the same result. For $U>0$, complete the square independently at each site and time slice:

$$
 e^{\Delta\tau U\mathbf j^2/2}=\left(\frac{\Delta\tau}{2\pi U}\right)^{3/2}\int_{\mathbb R^3}d^3M\,\exp\left[-\Delta\tau\left(\frac{\mathbf M^2}{2U}-\mathbf M\cdot\mathbf j\right)\right].
$$

This normalized [spin-vector Hubbard–Stratonovich decoupling](../../../../../spin-vector-hubbard-stratonovich-decoupling.md) yields

$$
\boxed{S=S_0+\int_0^\beta d\tau\sum_n\left[\frac{\mathbf M_n^2}{2U}-\sum_{\alpha\beta}\bar\psi_{n\alpha}\mathbf M_n\cdot\boldsymbol\sigma_{\alpha\beta}\psi_{n\beta}\right].}
$$

The auxiliary [bosonic](../../../../../boson.md) [quantum field](../../../../../quantum-field.md) is real and periodic, while the fermionic fields remain antiperiodic. All three vector components are required to reproduce the original $3U$ interaction; replacing this exact transformation by a single-component identity would change its coefficient.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
