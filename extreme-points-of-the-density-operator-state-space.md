# Extreme points of the density-operator state space

↑ **Parent:** [Density matrix](density-matrix.md)

The [density operators](density-matrix.md) on a finite-dimensional [Hilbert space](hilbert-space-split.md) form a convex set. Its [extreme points](extreme-point.md) are exactly the rank-one projectors, hence exactly the [pure states](pure-state.md). To prove this, suppose $|\psi\rangle\langle\psi|=\sum_i a_i\rho_i$ with $a_i>0$ and $\rho_i$ [positive semidefinite](positive-semidefinite-matrix.md). For $w\perp\psi$, $0=\sum_i a_i\langle w|\rho_i|w\rangle$ is a sum of nonnegative numbers, so every term vanishes. Diagonalizing $\rho_i$ shows that $\langle w|\rho_i|w\rangle=0$ implies $\rho_iw=0$. Thus each $\rho_i$ is supported on the line spanned by $\psi$, and its unit [trace](matrix-trace.md) forces $\rho_i=|\psi\rangle\langle\psi|$.

Conversely, a [density operator](density-matrix.md) of [rank](rank-one-quadratic-form.md) at least two has a [spectral decomposition](spectral-decomposition.md) with at least two positive [eigenvalues](eigenvalue.md). If $\lambda$ is one of them, $0<\lambda<1$ and $\rho=\lambda|e\rangle\langle e|+(1-\lambda)\sigma$, where $\sigma$ is the normalized remainder. These are distinct [density operators](density-matrix.md), proving that $\rho$ is not an [extreme point](extreme-point.md).

## ↑ Ancestors (5)

1. [Density matrix](density-matrix.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/1/b/solution.md)
