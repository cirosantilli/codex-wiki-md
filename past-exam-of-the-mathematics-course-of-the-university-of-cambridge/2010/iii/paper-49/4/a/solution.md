<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $N=2^n$ and label the binary digits of $x$ by $x_{n-1},\ldots,x_0$, with $x=\sum_{j=0}^{n-1}2^jx_j$. The [Walsh-Hadamard transform](../../../../../../walsh-hadamard-transform.md) prepares the [uniform quantum superposition](../../../../../../uniform-quantum-superposition.md) $N^{-1/2}\sum_x|x\rangle$. Applying the [phase gate](../../../../../../phase-gate.md) $R_a^{2^j}$ to the qubit for digit $x_j$ multiplies its basis amplitude by $\exp(2\pi ia2^jx_j/N)$. Taking their product gives

$$
\prod_{j=0}^{n-1}e^{2\pi ia2^jx_j/N}=e^{2\pi iax/N}.
$$

With the most significant qubit written first, this proves

$$
\boxed{\left(R_a^{2^{n-1}}\otimes R_a^{2^{n-2}}\otimes\cdots\otimes R_a\right)H^{\otimes n}|0^n\rangle
=\frac1{\sqrt N}\sum_{x=0}^{N-1}e^{2\pi iax/N}|x\rangle.}
$$

Each power is implemented by repeated uses of the supplied gate. The total is $\sum_{j=0}^{n-1}2^j=N-1$ uses. This realizes [dyadic phase-gate identification](../../../../../../dyadic-phase-gate-identification.md) without needing an unknown controlled gate or asserting a gate-call cost polynomial in $n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
