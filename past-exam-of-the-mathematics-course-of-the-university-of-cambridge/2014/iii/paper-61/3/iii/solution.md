<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The binary phase is $\phi=0.i_1\cdots i_n=\sum_{j=1}^ni_j2^{-j}$. Therefore

$$
\boxed{\frac{2\pi\phi}{M}=\sum_{j=1}^ni_j\frac{2\pi}{2^jM}}.
$$

On the phase register, apply the [tensor product](../../../../../../tensor-product.md) of [phase gates](../../../../../../phase-gate.md)

$$
D_M=\bigotimes_{j=1}^nP\!\left(\frac{2\pi}{2^jM}\right).
$$

Its action on $|y\rangle=|i_1\cdots i_n\rangle$ is multiplication by $e^{2\pi i\phi/M}$. Thus the [positive-phase fractional power of a unitary operator](../../../../../../positive-phase-fractional-power-of-a-unitary-operator.md) is implemented by [uncomputation](../../../../../../uncomputation.md) after coherent phase estimation:

$$
|0^n\rangle\sum_jc_j|v_j\rangle
\stackrel V\longmapsto\sum_jc_j|y_j\rangle|v_j\rangle
\stackrel{D_M}\longmapsto\sum_jc_je^{2\pi i\phi_j/M}|y_j\rangle|v_j\rangle
\stackrel{V^\dagger}\longmapsto
|0^n\rangle\sum_jc_je^{2\pi i\phi_j/M}|v_j\rangle.
$$

Hence

$$
\boxed{V^\dagger(D_M\otimes I)V\bigl(|0^n\rangle|\xi\rangle\bigr)
=|0^n\rangle U^{1/M}|\xi\rangle}.
$$

The inverse phase-estimation circuit uses controlled powers of $U^{-1}$ built from the supplied inverse oracle, with all other [quantum gates](../../../../../../quantum-logic-gate.md) reversed. No phase-register measurement is made, so arbitrary superpositions are preserved and the [ancilla qubits](../../../../../../ancilla-qubit.md) return to zero. The straightforward implementation uses $2(2^n-1)$ controlled-unitary queries plus the Fourier and phase circuitry; the arbitrary [phase gates](../../../../../../phase-gate.md) are accepted exactly as stipulated.

The branch convention matters. This construction uses the phase representative $0<\phi<1$ specified here, corresponding to argument in $(0,2\pi)$. It implements that explicitly defined root, even for $\phi>1/2$. The usual complex principal branch with argument in $(-\pi,\pi]$ would choose a different root on some [eigenvalues](../../../../../../eigenvalue.md). No substitution of that alternative branch is implicit.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
