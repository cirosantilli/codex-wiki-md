# Quantum spectral filtering

↑ **Parent:** [Quantum phase estimation](quantum-phase-estimation.md)

Let a [Hermitian operator](hermitian-operator.md) $A$ have dyadic [eigenvalues](eigenvalue.md) $\lambda_j=c_j/2^t$ in $[0,1)$ for known $t$, with controlled access to the [unitary operator](unitary-operator.md) $U=e^{2\pi iA}$. This interval ensures that different [eigenvalues](eigenvalue.md) have different [eigenphases](eigenphase.md); exact representability alone would not exclude phase aliasing, as $0$ and $1$ both give phase zero. Let a real [function](function-split.md) $h$ obey $|h(\lambda_j)|\leq1$, and assume the required [quantum variable rotations](quantum-variable-rotation.md) are available. Coherent [exact quantum phase estimation](exact-quantum-phase-estimation.md), a [quantum variable rotation](quantum-variable-rotation.md) and [uncomputation](uncomputation.md) implement

$$
|u_j\rangle|0\rangle\longmapsto|u_j\rangle\left(\sqrt{1-h(\lambda_j)^2}|0\rangle+h(\lambda_j)|1\rangle\right).
$$

[Postselection](postselection.md) on flag one gives $h(A)|b\rangle$ normalized, with [probability](probability.md) $\|h(A)|b\rangle\|^2$, provided this vector is nonzero. Erasing the [eigenvalue](eigenvalue.md) label by [uncomputation](uncomputation.md) is essential to preserve coherence between different [eigenvectors](eigenvector.md). On this dyadic spectrum, $U^{2^t}=I$ gives $U^{-1}=U^{2^t-1}$, so reversing the phase-estimation gates is possible using forward controlled-$U$ calls. The choice $h(\lambda)=\lambda$ multiplies by $A$; a scaled reciprocal gives the different filter used in the [HHL algorithm](hhl-algorithm.md).

**Table of contents**

- [Singular obstruction to normalized quantum matrix multiplication](singular-obstruction-to-normalized-quantum-matrix-multiplication.md)
- [Success probability of positive quantum spectral filtering](success-probability-of-positive-quantum-spectral-filtering.md)

## ↑ Ancestors (6)

1. [Quantum phase estimation](quantum-phase-estimation.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/3/b/ii/solution.md)
