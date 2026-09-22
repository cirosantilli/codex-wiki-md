<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Neither monotonic decrease alone nor equality of the initial spectra guarantees convergence**. A nonnegative [Lyapunov function](../../../../../../lyapunov-function.md) can approach a positive limiting value, and the set where $\dot V=0$ can contain trajectories other than the target. Different initial spectra already obstruct exact tracking: [unitary time evolution](../../../../../../unitary-time-evolution.md) preserves the eigenvalues of each [density operator](../../../../../../density-matrix.md), while two matrices approaching one another in norm must have the same limiting eigenvalues.

Even the spectral obstruction can be absent while the [Lyapunov quantum control](../../../../../../lyapunov-quantum-control.md) stalls. Take a [qubit](../../../../../../qubit.md) with $H_0=Z/2$, $H_1=X$, $\rho_d(0)=|0\rangle\langle0|$ and $\rho(0)=|1\rangle\langle1|$. Both [density operators](../../../../../../density-matrix.md) commute with $H_0$, and the [commutator](../../../../../../commutator.md) of $X$ with $\rho$ has zero diagonal, so $f=\operatorname{Tr}(\rho_d[-iX,\rho])=0$. Both states remain constant. They have the identical spectrum $(1,0)$, but $\boxed{\|\rho(t)-\rho_d(t)\|_{\mathrm{HS}}=\sqrt2\text{ for all }t}$. Moreover $iZ,iX$ generate the full [special unitary Lie algebra](../../../../../../special-unitary-lie-algebra.md) $\mathfrak{su}(2)$, so the failure here is a limitation of this particular feedback law, not a lack of available state-transfer controls.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
