<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a lattice-periodic one-electron [Hamiltonian](../../../../hamiltonian.md), [Bloch's theorem](../../../../bloch-s-theorem-split.md) gives

$$
\boxed{\psi_{n\mathbf k}(\mathbf r)=e^{i\mathbf k\cdot\mathbf r}u_{n\mathbf k}(\mathbf r),\qquad
u_{n\mathbf k}(\mathbf r+\mathbf R)=u_{n\mathbf k}(\mathbf r).}
$$

Here $\mathbf R$ is any lattice translation and $n$ labels an [energy band](../../../../energy-band.md). Under that translation the [wavefunction](../../../../wave-function-split.md) gains phase $e^{i\mathbf k\cdot\mathbf R}$. The [crystal momentum](../../../../crystal-momentum.md) $\hbar\mathbf k$ labels this translation eigenvalue and is defined modulo $\hbar\mathbf G$ for a [reciprocal lattice](../../../../reciprocal-lattice.md) vector $\mathbf G$.

The [mechanical momentum](../../../../mechanical-momentum.md) is different. In zero [magnetic field](../../../../magnetic-field-split.md) its operator is $-i\hbar\nabla$, which acts as

$$
-i\hbar\nabla\psi_{n\mathbf k}
=\hbar\mathbf k\psi_{n\mathbf k}
+e^{i\mathbf k\cdot\mathbf r}(-i\hbar\nabla u_{n\mathbf k}).
$$

A general [Bloch state](../../../../bloch-state.md) is therefore not a mechanical-momentum eigenstate. Expanding its periodic factor gives plane-wave components with momenta $\hbar(\mathbf k+\mathbf G)$, with probabilities determined by their [Fourier coefficients](../../../../fourier-coefficient.md). For a local [Hamiltonian](../../../../hamiltonian.md) $p^2/(2m_e)+V(\mathbf r)$, its mean momentum satisfies

$$
\boxed{\langle\mathbf p\rangle=m_e\mathbf v_g=\frac{m_e}{\hbar}\nabla_{\mathbf k}E_n(\mathbf k),}
$$

not generally $\hbar\mathbf k$. The lattice exchanges actual momentum with the electron; crystal-momentum conservation in scattering is instead modulo reciprocal-lattice vectors, as in [Umklapp scattering](../../../../umklapp-scattering.md).

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
