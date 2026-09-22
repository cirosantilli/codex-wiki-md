<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[QMA](../../../../../../qma.md) is the class of [promise problems](../../../../../../promise-problem.md) for which a uniform polynomial-size [quantum circuit](../../../../../../quantum-circuit-split.md) checks a polynomial-size [quantum witness](../../../../../../quantum-witness.md). A YES instance has some [quantum witness](../../../../../../quantum-witness.md) accepted with probability at least $2/3$; on a NO instance every [quantum witness](../../../../../../quantum-witness.md) is accepted with probability at most $1/3$. The verifier initializes its own [ancilla qubits](../../../../../../ancilla-qubit.md) to zero. Mixed [quantum witnesses](../../../../../../quantum-witness.md) do not improve the maximum because acceptance is linear in their [density operator](../../../../../../density-matrix.md).

For a verifier $U_x$ and [quantum witness](../../../../../../quantum-witness.md) embedding $J|w\rangle=|w\rangle|0\cdots0\rangle$, define the [witness acceptance operator](../../../../../../witness-acceptance-operator.md)

$$
F=J^\dagger U_x^\dagger\Pi_1U_xJ,\qquad0\leq F\leq I.
$$

The [Rayleigh quotient](../../../../../../rayleigh-quotient.md) gives $\max_{\|w\|=1}\langle w|F|w\rangle=\lambda_{\max}(F)$. Every entry of $F$ can be recomputed by the polynomial-storage path summation of part (b); no full [quantum witness](../../../../../../quantum-witness.md) matrix needs to be stored.

Let the [quantum witness](../../../../../../quantum-witness.md) have $m$ qubits, so its dimension is $D=2^m$. For this positive operator, [trace-power witness optimization](../../../../../../trace-power-witness-optimization.md) uses

$$
\lambda_{\max}(F)^d\leq\operatorname{Tr}(F^d)\leq D\lambda_{\max}(F)^d.
$$

This is the useful exponentiated form of the supplied logarithmic inequality. Positivity is required; such a logarithmic statement is not true for an arbitrary operator. No logarithms or roots need to be calculated.

Choose $d=2m+2$. On a NO instance,

$$
\operatorname{Tr}(F^d)\leq 2^m(1/3)^d<(1/2)^d,
$$

since $2^m(2/3)^{2m+2}=(4/9)(8/9)^m<1$. On a YES instance, $\operatorname{Tr}(F^d)\geq(2/3)^d>(1/2)^d$. Thus comparison of $2^d\operatorname{Tr}(F^d)$ with one distinguishes the cases using only multiplication and a final comparison.

Evaluate the trace by

$$
\operatorname{Tr}(F^d)=\sum_{i_0,\ldots,i_{d-1}}F_{i_0i_1}F_{i_1i_2}\cdots F_{i_{d-1}i_0}.
$$

There are $d=O(m)$ active [quantum witness](../../../../../../quantum-witness.md) indices, each requiring $m$ bits. Accumulate one product at a time and recompute its matrix entries as required. Together with the verifier path workspace, this uses polynomially many real registers. The potentially enormous time and the numerical precision are unrestricted in $C$. **Therefore $\mathrm{QMA}\subseteq C$**, without solving an exponentially large [eigenvalue](../../../../../../eigenvalue.md) problem by storing its matrix.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
