<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) convention $F_N|k\rangle=N^{-1/2}\sum_{j=0}^{N-1}\omega^{jk}|j\rangle$, where $\omega=e^{2\pi i/N}$. Reindexing the shifted sum gives

$$
S F_N|k\rangle=\frac1{\sqrt N}\sum_j\omega^{jk}|j+1\rangle=\omega^{-k}\frac1{\sqrt N}\sum_{\ell}\omega^{\ell k}|\ell\rangle.
$$

Thus the [cyclic shift operator](../../../../../../cyclic-shift-operator.md) has these [eigenvectors](../../../../../../eigenvector.md), with [eigenvalues](../../../../../../eigenvalue.md) $e^{-2\pi i k/N}$. This is [cyclic shift diagonalization by the quantum Fourier transform](../../../../../../cyclic-shift-diagonalization-by-the-quantum-fourier-transform.md), and it implies $S=F_ND F_N^\dagger$ with $D|k\rangle=\omega^{-k}|k\rangle$.

For $N=4$, the binary encoding is $k=2x+y$, with $x$ the more significant [qubit](../../../../../../qubit.md). The required diagonal phase is

$$
e^{-2\pi i(2x+y)/4}=(-1)^x(-i)^y,
$$

so $D=P_{-1}\otimes P_{-i}$. **The allowed-gate circuit is therefore**

$$
\boxed{S=\operatorname{QFT}_4(P_{-1}\otimes P_{-i})\operatorname{QFT}_4^{-1}.}
$$

In execution order, apply the inverse [QFT](../../../../../../quantum-fourier-transform.md), then the two [phase gates](../../../../../../phase-gate.md), then the forward [QFT](../../../../../../quantum-fourier-transform.md). There is no extra global phase. Reversing the Fourier sign convention would conjugate both [phase gate](../../../../../../phase-gate.md) parameters.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
