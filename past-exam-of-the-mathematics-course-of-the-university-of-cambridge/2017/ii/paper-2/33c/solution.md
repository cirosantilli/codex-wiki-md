<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

For a normalized trial state $|\psi\rangle=\sum_nc_n|n\rangle$ in the form domain of a bounded-below [Hamiltonian](../../../../../hamiltonian.md), the [quantum variational principle](../../../../../quantum-variational-principle.md) gives $\langle H\rangle=\sum_n|c_n|^2E_n\geq E_0$. Thus each trial [expectation](../../../../../expected-value.md) is an upper bound for the ground-state energy. The same spectral argument covers a continuum: for a decaying potential whose essential spectrum begins at $0$, a negative trial [expectation](../../../../../expected-value.md) guarantees a negative-energy [bound state](../../../../../bound-state.md).

For the stated exponential trial function, normalization follows from $4\alpha^3\int_0^\infty r^2e^{-2\alpha r}\,dr=1$. The kinetic [expectation](../../../../../expected-value.md), using $\int|\nabla\psi|^2$, is $\hbar^2\alpha^2/(2m)$. The potential [expectation](../../../../../expected-value.md) is $-4A\alpha^3\int_0^\infty re^{-(\mu+2\alpha)r}\,dr$. Therefore

$$
\boxed{E(\alpha)=\frac{\hbar^2\alpha^2}{2m}-\frac{4A\alpha^3}{(\mu+2\alpha)^2}.}
$$

The [exponential variational bound for the Yukawa potential](../../../../../exponential-variational-bound-for-the-yukawa-potential.md) at $\alpha=\mu/2$ gives $E=(\mu/8)(\hbar^2\mu/m-A)<0$ if $\mu<Am/\hbar^2$. Thus **a [bound state](../../../../../bound-state.md) necessarily exists in the stated range**.

For $\mu\geq Am/\hbar^2$, this single-exponential family cannot prove binding: the maximum of $4A\alpha/(\mu+2\alpha)^2$ is $A/(2\mu)$, so every $E(\alpha)\geq0$. This does not prove absence of [bound states](../../../../../bound-state.md).

The equality case can in fact be strengthened. At $\mu=Am/\hbar^2$, use normalized exponentials $\psi_{\mu/2},\psi_\mu$ and write $Q=\hbar^2\mu^2/m$. Their [matrix](../../../../../matrix.md) elements are

$$
\langle\psi_{\mu/2},H\psi_{\mu/2}\rangle=0,\quad
\langle\psi_{\mu/2},H\psi_\mu\rangle=-\frac{8\sqrt2}{675}Q,\quad
\langle\psi_\mu,H\psi_\mu\rangle=\frac Q{18}.
$$

The Rayleigh numerator for $\psi_{\mu/2}+\epsilon\psi_\mu$ is negative for sufficiently small $\epsilon>0$, and its norm is nonzero. Hence **binding also holds at equality, and by [continuity](../../../../../continuous-function.md) in a small interval beyond it**. For arbitrary larger $\mu$, these trials alone do not settle existence; a nonnegative variational upper bound cannot establish a nonnegative ground-state energy.

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
