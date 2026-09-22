<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the unsquared convention for [quantum fidelity](../../../../../../fidelity-of-quantum-states.md). For [density operators](../../../../../../density-matrix.md) on a common finite-dimensional [Hilbert space](../../../../../../hilbert-space-split.md),

$$
\boxed{F(\rho,\sigma)=\|\sqrt\rho\sqrt\sigma\|_1=\operatorname{Tr}\sqrt{\sqrt\rho\,\sigma\sqrt\rho}.}
$$

Here $\|A\|_1=\operatorname{Tr}\sqrt{A^\dagger A}$ is the [trace norm](../../../../../../trace-norm.md), and all square roots are the positive operator square roots. The two displayed expressions agree because $\sqrt\rho\sqrt\sigma$ and its adjoint have the same singular values. This convention has $0\leq F\leq1$; some literature squares this quantity, but that convention is not used here.

For normalized [pure states](../../../../../../pure-state.md), the rank-one operator $\sqrt\rho\sqrt\sigma=\langle\varphi|\psi\rangle|\varphi\rangle\langle\psi|$ has a single nonzero singular value. Therefore

$$
\boxed{F(|\varphi\rangle\langle\varphi|,|\psi\rangle\langle\psi|)=|\langle\varphi|\psi\rangle|.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
