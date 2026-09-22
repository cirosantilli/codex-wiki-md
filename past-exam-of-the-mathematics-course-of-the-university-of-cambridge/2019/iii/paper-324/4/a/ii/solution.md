<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the normalized input as $|b\rangle=\sum_j\beta_j|u_j\rangle$, where $A|u_j\rangle=\lambda_j|u_j\rangle$ and $\lambda_j>0$. Use a data register, an $n$-qubit eigenvalue register, and a flag [quantum ancilla](../../../../../../../quantum-ancilla.md). Begin with $|b\rangle|0^n\rangle|0\rangle$.

Apply [exact quantum phase estimation](../../../../../../../exact-quantum-phase-estimation.md) to $e^{2\pi iA}$. Its controlled evolutions and inverse [quantum Fourier transform](../../../../../../../quantum-fourier-transform.md) produce

$$
\sum_j\beta_j|u_j\rangle|\ell_j\rangle|0\rangle,
\qquad \lambda_j=\ell_j/2^n.
$$

Apply the [HHL controlled reciprocal rotation](../../../../../../../hhl-controlled-reciprocal-rotation.md), with $0<c\leq\lambda_{\min}$:

$$
|\ell_j\rangle|0\rangle\longmapsto
|\ell_j\rangle\left(\sqrt{1-c^2/\lambda_j^2}|0\rangle
+\frac c{\lambda_j}|1\rangle\right).
$$

The function of $\ell_j$ is computed by [quantum arithmetic](../../../../../../../quantum-arithmetic.md); the rotation is a [quantum variable rotation](../../../../../../../quantum-variable-rotation.md). On a zero eigenvalue label with no input amplitude, define any unitary action, for example no rotation.

Run the inverse phase-estimation circuit. Because each amplitude multiplier depends only on $\lambda_j$, the eigenvalue register is reset to $|0^n\rangle$ on both flag branches. Measuring the flag and conditioning on outcome one leaves

$$
\boxed{|\xi\rangle=\frac{\sum_j\beta_j\lambda_j^{-1}|u_j\rangle}
{\sqrt{\sum_j|\beta_j|^2\lambda_j^{-2}}}
=\frac{A^{-1}b}{\|A^{-1}b\|}.}
$$

The successful unnormalized branch is $cA^{-1}|b\rangle$, giving the probability in the preceding part. The operations independent of $A,b$ are the [Hadamard gates](../../../../../../../hadamard-gate.md) preparing the phase register, the inverse [quantum Fourier transform](../../../../../../../quantum-fourier-transform.md), the reversible reciprocal/angle arithmetic, the controlled fixed-angle rotations, and the final flag measurement. [Uncomputation](../../../../../../../uncomputation.md) removes all arithmetic workspace; the $A$-dependent controlled evolutions and the $b$-dependent state-preparation circuit supply the input-specific operations.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
