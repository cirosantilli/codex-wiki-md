<h1 id="37e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [multigrid method](../../../../../../multigrid-method.md) combines a fine-grid smoother with a [coarse-grid correction](../../../../../../coarse-grid-correction.md). Starting with $u_h$, apply a few smoothing iterations, compute $r_h=b_h-A_hu_h$, restrict this residual to a coarser grid, and approximately solve $A_He_H=Rr_h$. Prolong the coarse error and update $u_h\leftarrow u_h+Pe_H$, then post-smooth. The coarse solve is itself performed recursively, with a direct solve at the coarsest level; visiting each coarser level once gives a V-cycle. The smoother damps rapidly varying error, while error smooth on the fine grid is efficiently represented and corrected on the coarse grid.

For ordinary Jacobi, $\omega=1$, the highest-frequency sine-product error has [eigenvalue](../../../../../../eigenvalue.md) approaching $-1$, not zero. In particular for the discrete Poisson equation it is $-\cos(\pi h)$, whose magnitude approaches one. This nearly alternating error changes sign between sweeps but is barely damped, and ordinary coarse-grid restriction does not represent it well. Thus **with the standard point-Jacobi smoother and coarse-grid transfers one chooses $\omega\ne1$, usually $0<\omega<1$, for fast multigrid convergence**. For example $\omega=2/3$ makes the extreme high-frequency [eigenvalue](../../../../../../eigenvalue.md) approach $-1/3$. Convergence of Jacobi as a standalone iteration is therefore insufficient to guarantee that it is an effective smoother. This conclusion concerns that standard multigrid choice; other smoothers or specially designed transfers can change it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [37E](../../37e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
