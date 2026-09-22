<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

List the known distinct strings in $A$ as $a_0,\ldots,a_{N-1}$, where $N=2^m$, and use an $m$-[qubit](../../../../../../qubit.md) index [quantum ancilla](../../../../../../quantum-ancilla.md). Apply [Hadamard gates](../../../../../../hadamard-gate.md) to that register to prepare

$$
|0^n\rangle\otimes\frac1{\sqrt N}\sum_{j=0}^{N-1}|j\rangle.
$$

First, for each $j$ with $a_j\ne0^n$, apply the available [unitary operator](../../../../../../unitary-operator.md) that transposes $|0^n,j\rangle$ and $|a_j,j\rangle$. The pairs are disjoint because they have distinct index labels. Skip a transposition when the two vectors coincide. This produces

$$
\frac1{\sqrt N}\sum_j|a_j,j\rangle.
$$

Second, for each $j\ne0$, transpose $|a_j,j\rangle$ and $|a_j,0^m\rangle$. These pairs are disjoint because the data strings $a_j$ are distinct. No pair contains the term with $j=0$, and no later transposition moves an earlier output. The final state is exactly

$$
\boxed{\frac1{\sqrt N}\sum_j|a_j\rangle\otimes|0^m\rangle=|\psi_A\rangle\otimes|0^m\rangle.}
$$

This [clean subset superposition preparation](../../../../../../clean-subset-superposition-preparation.md) uses at most $N+(N-1)=2N-1$ of the given transpositions and $m$ [Hadamard gates](../../../../../../hadamard-gate.md). Since $m=O(\log_2 n)$, $N$ is polynomial in $n$; multiplying this count by the assumed polynomial size of each transposition gives a polynomial-size [quantum circuit](../../../../../../quantum-circuit-split.md). The index [quantum ancilla](../../../../../../quantum-ancilla.md) returns to zero, so the data register is a pure [uniform superposition state](../../../../../../uniform-superposition-state.md), rather than a mixture obtained by discarding its index. The construction uses an available enumeration of the known subset; a membership oracle alone would not justify that enumeration.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
