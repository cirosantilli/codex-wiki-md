<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [steady state](../../../../../../steady-state.md) is a time-independent physical state: its derivative vanishes. With $n=N^2-1$, the [Affine Bloch equation](../../../../../../affine-bloch-equation.md) therefore requires

$$
\boxed{As_*=-c.}
$$

As a real linear equation, it has a solution exactly when $\operatorname{rank}A=\operatorname{rank}[A\mid-c]$. If $s_p$ is one solution, all algebraic solutions are $s_p+\ker A$, an affine set of dimension $n-\operatorname{rank}A$. Physical [steady states](../../../../../../steady-state.md) are its intersection with the set of [Bloch vectors](../../../../../../bloch-vector.md) corresponding to positive [trace](../../../../../../matrix-trace.md)-one [density operators](../../../../../../density-matrix.md). An arbitrary affine equation need not have a [steady state](../../../../../../steady-state.md): $A=0$, $c\ne0$ is a counterexample.

The equation here comes from a finite-dimensional time-independent [Lindblad equation](../../../../../../lindblad-equation.md), however, so it always has at least one physical [steady state](../../../../../../steady-state.md). To prove this, start from any [density operator](../../../../../../density-matrix.md) and average its trajectory:

$$
\overline\rho_T=\frac1T\int_0^T\rho(t)\,dt.
$$

These averages remain positive with [trace](../../../../../../matrix-trace.md) one. That set is a [compact set](../../../../../../compact-space.md), so some sequence has a limit $\rho_*$. If $\mathcal L$ is the time-independent generator, then

$$
\mathcal L(\overline\rho_T)=\frac{\rho(T)-\rho(0)}T\longrightarrow0,
$$

because [density operators](../../../../../../density-matrix.md) are bounded. Continuity gives $\mathcal L(\rho_*)=0$. This proves directly that [Finite-dimensional Lindbladians have stationary states](../../../../../../finite-dimensional-lindbladians-have-stationary-states.md).

If $A$ has full rank, its algebraic solution $s_*=-A^{-1}c$ is unique and existence makes that solution physical. For these Lindblad dynamics the converse also holds, even for a boundary [steady state](../../../../../../steady-state.md). If $A$ is singular, choose a nonzero traceless Hermitian stationary direction $X$. The two parts of its [positive-negative decomposition](../../../../../../positive-negative-decomposition-of-a-hermitian-operator.md) have the same [trace](../../../../../../matrix-trace.md) $\tau>0$, so $X=\tau(\rho_+-\rho_-)$ for two [density operators](../../../../../../density-matrix.md). Time-average their trajectories along a common convergent subsequence. Their limits are stationary by the preceding argument, and their difference remains $X/\tau$, since $X$ itself is stationary. The limits are therefore distinct physical stationary states.

Thus **the finite-dimensional physical Bloch equation has a unique [steady state](../../../../../../steady-state.md) exactly when $\operatorname{rank}A=n$**. These [steady states of an affine Bloch equation](../../../../../../steady-states-of-an-affine-bloch-equation.md) must be distinguished from convergence to that [steady state](../../../../../../steady-state.md), which requires the additional spectral condition in (b). The possibly nonorthonormal coordinate basis does not affect existence or uniqueness, since it still gives an invertible parametrization of the traceless Hermitian space.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
