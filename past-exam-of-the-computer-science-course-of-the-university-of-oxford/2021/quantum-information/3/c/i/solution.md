<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**No test on Alice and Bob's systems gives any information about which global state was prepared, even with arbitrarily many independent copies.** In the pure GHZ [density matrix](../../../../../../density-matrix-split.md), the off-diagonal terms contain $|0\rangle\langle1|_C$ or its adjoint. Their [partial traces](../../../../../../partial-trace.md) vanish. Hence both preparations have the same [reduced density matrix](../../../../../../reduced-density-matrix.md)

$$
\sigma_{AB}=\operatorname{Tr}_C(|\mathrm{GHZ}\rangle\langle\mathrm{GHZ}|)
=\operatorname{Tr}_C\rho
=\tfrac12\bigl(|00\rangle\langle00|+|11\rangle\langle11|\bigr).
$$

For any [POVM](../../../../../../positive-operator-valued-measure.md) effect $E$ acting jointly on $AB$, the outcome [probability](../../../../../../probability.md) is $\operatorname{Tr}(E\sigma_{AB})$ in either case. [Equal reduced states give identical local statistics](../../../../../../equal-reduced-states-give-identical-local-statistics.md), where local here means local to the entire accessible laboratory $AB$, not separate operations on $A$ and $B$.[§2.3.1, printed pp. 14–17, reduced density operators and accessible expectation values](../../../../../../foundations-i-states-and-ensembles-by-john-preskill.md)

For $n$ independent copies, taking the [partial trace](../../../../../../partial-trace.md) of each inaccessible $C$ system yields $\sigma_{AB}^{\otimes n}$ under either hypothesis. Even an arbitrary collective [quantum measurement](../../../../../../quantum-measurement-split.md) on all $2n$ accessible [qubits](../../../../../../qubit.md) therefore has identical outcome [probabilities](../../../../../../probability.md). Adaptive local processing cannot change equality of the accessible [density matrices](../../../../../../density-matrix-split.md). With equal prior [probabilities](../../../../../../probability.md) the optimal guessing [probability](../../../../../../probability.md) remains $1/2$; with other priors, no observation updates their ratio.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
