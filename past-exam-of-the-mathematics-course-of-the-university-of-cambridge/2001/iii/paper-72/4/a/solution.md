<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the finite-chain spin vector as $\sigma$ and the exchange matrix as $\mathsf J$. For $J>0$ and $\kappa>0$ this matrix is positive definite, as can be seen from the positive Fourier symbol in part (b), or from the explicit positive open-chain inverse. The [linear-source multivariate Gaussian integral](../../../../../../linear-source-multivariate-gaussian-integral.md), obtained by completing the square, gives

$$
\int_{\mathbb R^N}d^Nm\,\exp[-m^T\mathsf J^{-1}m+2m^T\sigma]
=\pi^{N/2}(\det\mathsf J)^{1/2}\exp[\sigma^T\mathsf J\sigma].
$$

Indeed the exponent is $-(m-\mathsf J\sigma)^T\mathsf J^{-1}(m-\mathsf J\sigma)+\sigma^T\mathsf J\sigma$. Insert this [Hubbard–Stratonovich transformation](../../../../../../hubbard-stratonovich-transformation.md) into the spin [partition function](../../../../../../canonical-partition-function.md). The field term remains $h\sum_i\sigma_i$, and each independent spin sum is

$$
\sum_{\sigma_i=\pm1}e^{(2m_i+h)\sigma_i}=2\cosh(2m_i+h).
$$

Consequently

$$
\boxed{Z=C\int_{\mathbb R^N}d^Nm\,
\exp\left[-m^T\mathsf J^{-1}m+\sum_i\log\{2\cosh(2m_i+h)\}\right],\quad
C=\frac1{\pi^{N/2}\sqrt{\det\mathsf J}}.}
$$

The interaction convention counts the full ordered pair sum, with no factor of one-half, so the auxiliary coupling is $2m_i\sigma_i$. Diagonal terms $J_{ii}\sigma_i^2$ only contribute a constant to the spin [Hamiltonian](../../../../../../hamiltonian.md); retaining them makes the given positive exchange matrix and normalization convenient. The auxiliary field is not itself the physical spin [magnetization](../../../../../../magnetization.md): the conditional spin expectation is $\tanh(2m_i+h)$, so $\langle\sigma_i\rangle=\langle\tanh(2m_i+h)\rangle$ in the auxiliary-field integral.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
