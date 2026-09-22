<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an open chain there are $L-1$ bonds, with both endpoint [Ising spins](../../../../ising-spin-variable.md) independently summed. Retain the same [spin-chain transfer matrix](../../../../transfer-matrix-for-a-classical-spin-chain.md), but replace the trace by endpoint vectors. With $\mathbf1=(1,1)^{\mathsf T}$,

$$
\boxed{Z_L^{\mathrm{open}}=\mathbf1^{\mathsf T}W^{L-1}\mathbf1.}
$$

This follows directly by expanding the product of $L-1$ [Boltzmann factors](../../../../boltzmann-factor.md). If $\mathbf v_\pm$ are orthonormal [eigenvectors](../../../../eigenvector.md) of the [symmetric matrix](../../../../symmetric-matrix.md) $W$, the equivalent [spectral decomposition](../../../../spectral-decomposition.md) is

$$
Z_L^{\mathrm{open}}=\sum_{\nu=\pm}(\mathbf1^{\mathsf T}\mathbf v_\nu)^2\lambda_\nu^{L-1}.
$$

Fixed endpoint [Ising spins](../../../../ising-spin-variable.md) replace the corresponding $\mathbf1$ by a basis vector; extra endpoint [energies](../../../../energy-split.md) replace its entries by the corresponding [Boltzmann factors](../../../../boltzmann-factor.md). The leading bulk [Helmholtz free energy](../../../../helmholtz-free-energy.md) per spin agrees with the periodic result, because the boundary changes only subextensive terms. In particular, $L=1$ gives $Z_1^{\mathrm{open}}=\mathbf1^{\mathsf T}\mathbf1=2$, as required for one free [Ising spin](../../../../ising-spin-variable.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
