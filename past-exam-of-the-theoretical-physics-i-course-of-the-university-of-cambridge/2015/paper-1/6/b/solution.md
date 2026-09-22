<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the coordination number be $z_c=4$, and choose the spin-space $z$ axis along $\mathbf S=S\hat{\mathbf z}$. The mean-field decoupling of a bond is

$$
\mathbf S_i\cdot\mathbf S_j\simeq
\mathbf S_i\cdot\mathbf S+\mathbf S\cdot\mathbf S_j-S^2.
$$

The original directed neighbor sum counts each bond twice, so its factor $1/2$ cancels that double counting. The resulting energy is

$$
\boxed{E_{\rm MF}=-z_cJS\sum_i S_{iz}+\frac{Nz_cJ}{2}S^2.}
$$

The constant prevents double counting of the mean interaction energy and is necessary if [free energy](../../../../../thermodynamic-free-energy.md) is minimized with respect to $S$. With the source's unnormalized solid-angle measure, the single-site integral is

$$
Z_1(x)=2\pi\int_{-1}^{1}e^{x u}\,du
=4\pi\frac{\sinh x}{x},\qquad x=\beta z_cJS.
$$

Therefore

$$
\boxed{Z_{\rm MF}(S)=e^{-\beta Nz_cJS^2/2}
\left(4\pi\frac{\sinh(\beta z_cJS)}{\beta z_cJS}\right)^N,
\qquad z_c=4.}
$$

At $S=0$ take $\sinh x/x\to1$. A normalized solid-angle measure would remove the factor $(4\pi)^N$ without changing the [self-consistency equation](../../../../../self-consistency-equation.md). These are three-component classical [spins](../../../../../spin.md) on a two-dimensional positional lattice, not [spins](../../../../../spin.md) constrained to a plane.

The PDF's hint is a correct angular-integration identity for a term with coefficient $\beta J/2$. That coefficient is not the full single-site molecular field after summing all four neighbors and decoupling both entries of each bond. The net coefficient is $\beta z_cJ$, as follows from the explicitly stated [Hamiltonian](../../../../../hamiltonian.md); inserting the hint's coefficient as the total field would lose the coordination and double-counting factors.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
