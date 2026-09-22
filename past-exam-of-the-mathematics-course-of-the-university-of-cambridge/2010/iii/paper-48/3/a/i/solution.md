<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the unsquared [quantum fidelity](../../../../../../../fidelity-of-quantum-states.md) convention in the question. For any [matrix](../../../../../../../matrix.md) $X$, its [trace norm](../../../../../../../trace-norm.md) is $\|X\|_1=\operatorname{Tr}\sqrt{X^\dagger X}=\operatorname{Tr}\sqrt{XX^\dagger}$: the two positive matrices have the same nonzero eigenvalues, namely the squared [singular values](../../../../../../../singular-value.md). This follows directly from the [singular value decomposition](../../../../../../../singular-value-decomposition.md).

Set $X=\sqrt\rho\sqrt\sigma$. Then $XX^\dagger=\sqrt\rho\,\sigma\sqrt\rho$ and $X^\dagger X=\sqrt\sigma\,\rho\sqrt\sigma$. Their positive square roots therefore have the same trace, proving

$$
\boxed{F(\rho,\sigma)=\|\sqrt\rho\sqrt\sigma\|_1=F(\sigma,\rho)}.
$$

The argument also covers singular density operators, since zero singular values contribute zero.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 48](../../../../paper-48-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
