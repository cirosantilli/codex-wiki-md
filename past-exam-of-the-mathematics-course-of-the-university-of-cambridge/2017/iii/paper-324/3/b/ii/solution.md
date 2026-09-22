<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply $V^{-1}$ to the data and phase [quantum registers](../../../../../../../quantum-register.md), leaving the flag [quantum ancilla](../../../../../../../quantum-ancilla.md) untouched. This inverse needs no extra oracle assumption: the promised dyadic [eigenvalues](../../../../../../../eigenvalue.md) give $U^{2^n}=I$, hence $U^{-1}=U^{2^n-1}$. The inverse of each [controlled unitary gate](../../../../../../../controlled-unitary-gate.md) used in $V$ can therefore be built from repeated uses of the supplied controlled-$U$, and the known [Hadamard gates](../../../../../../../hadamard-gate.md) and [quantum Fourier transform](../../../../../../../quantum-fourier-transform.md) gates can be reversed. [Uncomputation](../../../../../../../uncomputation.md) is necessary to erase the [eigenvalue](../../../../../../../eigenvalue.md) label coherently. The resulting [quantum state](../../../../../../../quantum-state.md) is

$$
\sum_j\beta_j|u_j\rangle|0^n\rangle\left(\sqrt{1-\lambda_j^2}|0\rangle+\lambda_j|1\rangle\right).
$$

A [quantum measurement in the computational basis](../../../../../../../quantum-measurement-in-the-computational-basis.md) of the flag followed by [postselection](../../../../../../../postselection.md) on one yields

$$
\boxed{|\psi\rangle=\frac{A|b\rangle}{\|A|b\rangle\|},\qquad P_{\mathrm{success}}=\sum_j|\beta_j|^2\lambda_j^2=\|A|b\rangle\|^2.}
$$

This requires $A|b\rangle\neq0$. For a normalized input and nonnegative [eigenvalues](../../../../../../../eigenvalue.md), the [success probability of positive quantum spectral filtering](../../../../../../../success-probability-of-positive-quantum-spectral-filtering.md) satisfies $P_{\mathrm{success}}\geq\lambda_{\min}^2$. In the general inequality, equality holds precisely when the input is supported on the minimum-[eigenvalue](../../../../../../../eigenvalue.md) [eigenspace](../../../../../../../eigenspace.md). Omitting [uncomputation](../../../../../../../uncomputation.md) and discarding the phase [quantum register](../../../../../../../quantum-register.md) would instead leave a [mixed state](../../../../../../../mixed-state.md) with diagonal weights proportional to $|\beta_j|^2\lambda_j^2$, rather than the desired coherent [pure state](../../../../../../../pure-state.md).

**The printed universal nonzero-success request needs a nonkernel-input hypothesis.** An $n$-[qubit](../../../../../../../qubit.md) [Hermitian operator](../../../../../../../hermitian-operator.md) has $2^n$ [eigenvalues](../../../../../../../eigenvalue.md), counted with multiplicity. All are distinct, and the printed dyadic grid contains exactly $2^n$ possible values. They therefore occupy the entire grid, including zero: this is a [multiplicity-free complete dyadic spectrum](../../../../../../../multiplicity-free-complete-dyadic-spectrum.md), and $\lambda_{\min}=0$. Taking $n=1$, $A=\operatorname{diag}(0,1/2)$, and $|b\rangle=|0\rangle$ satisfies every printed spectral promise but gives $A|b\rangle=0$. No normalized output vector exists, so no algorithm can deliver it with nonzero probability.

For every input outside the [kernel](../../../../../../../kernel-of-a-linear-map.md), the procedure above has $P_{\mathrm{success}}>0=\lambda_{\min}^2$, giving the requested strict bound on the meaningful domain. The corrected result is therefore exact [quantum spectral filtering](../../../../../../../quantum-spectral-filtering.md) conditional on $A|b\rangle\neq0$, with the boxed probability. This does not require knowing the input [probability amplitudes](../../../../../../../probability-amplitude.md) or making extra copies of an unknown [quantum state](../../../../../../../quantum-state.md). Arbitrarily small nonzero support outside the [kernel](../../../../../../../kernel-of-a-linear-map.md) gives arbitrarily small success probability, and a failed flag measurement disturbs the input; fresh independent trials cannot be assumed when only one unknown physical input is supplied.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
