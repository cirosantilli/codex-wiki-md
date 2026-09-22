<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $L=2^n$ and use an $n$-qubit phase register. Begin with $|0^n\rangle|v\rangle$ and apply $H^{\otimes n}$ to the phase register, creating $L^{-1/2}\sum_{m=0}^{L-1}|m\rangle|v\rangle$. Controlled powers implement

$$
|m\rangle|v\rangle\longmapsto|m\rangle U^m|v\rangle
=e^{2\pi im\phi}|m\rangle|v\rangle.
$$

For phase [qubit](../../../../../../qubit.md) $j$, counted from the most significant bit, the controlled power is $U^{2^{n-j}}$. It can be built from $2^{n-j}$ calls to the supplied controlled-$U$ gate. By [quantum phase kickback](../../../../../../phase-kickback.md), the phase-register state is

$$
\frac1{\sqrt L}\sum_m e^{2\pi imy/L}|m\rangle=F_L|y\rangle.
$$

Apply the inverse [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) to obtain the [exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md) mapping

$$
\boxed{V:\ |0^n\rangle|v\rangle\longmapsto|y\rangle|v\rangle}.
$$

A [computational basis](../../../../../../computational-basis.md) measurement of the first register determines $y$ with certainty, hence $\phi=y/L$ and the [eigenvalue](../../../../../../eigenvalue.md) $e^{2\pi i\phi}$. Exactness follows from the promised dyadic phase; no approximation or continued-fraction reconstruction is needed.

With only controlled-$U$ available as a query, the repeated-power construction uses $L-1=2^n-1$ oracle calls. The other Fourier-transform circuitry has polynomial size in $n$ in the ideal phase-gate model. The [cost of exact phase estimation on a dyadic spectrum](../../../../../../cost-of-exact-phase-estimation-on-a-dyadic-spectrum.md) is therefore not polynomial in $n$ in this primitive-query model unless powered queries have additional implementations. The task does not require such a polynomial bound.

## ↑ Ancestors (11)

1. [I](../i.md)
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
