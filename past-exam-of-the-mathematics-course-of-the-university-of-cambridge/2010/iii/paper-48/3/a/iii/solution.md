<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We first establish the purification-overlap formula for [quantum fidelity](../../../../../../../fidelity-of-quantum-states.md), rather than assume the desired monotonicity. Write a canonical [purification of a density operator](../../../../../../../purification-of-a-density-operator.md) as

$$
|\sqrt\rho\rangle\!\rangle=\sum_{i,j}(\sqrt\rho)_{ij}|i\rangle|j\rangle.
$$

Tracing the second factor gives $\rho$. The [Schmidt decomposition](../../../../../../../schmidt-decomposition.md) shows that any other purification on a sufficiently large fixed ancillary space differs by a unitary on that space: its orthonormal ancillary vectors can be mapped to those of the canonical purification and the map extended to a [unitary operator](../../../../../../../unitary-operator.md). Zero eigenvalues are handled by padding the ancillary basis.

The overlap of two canonical purifications, with a relative ancillary unitary $U$, is $\operatorname{Tr}(\sqrt\rho\sqrt\sigma\,U^T)$, with zero padding when the ancillary dimension is larger. The [unitary variational formula for the trace norm](../../../../../../../unitary-variational-formula-for-the-trace-norm.md) is

$$
\max_{V\ {\rm unitary}}|\operatorname{Tr}(XV)|=\|X\|_1.
$$

Indeed if $X=PDQ^\dagger$ is a [singular value decomposition](../../../../../../../singular-value-decomposition.md), the trace is $\operatorname{Tr}(DW)$ with $W=Q^\dagger VP$ unitary. Its modulus is at most $\sum_jD_{jj}$ because $|W_{jj}|\leq1$, and $V=QP^\dagger$ attains that bound. Thus the maximal absolute overlap of purifications equals $F(\rho,\sigma)$; this also proves the needed form of [Uhlmann's theorem](../../../../../../../uhlmann-s-theorem.md).

Choose purifications $|\psi\rangle_{ABE}$ and $|\phi\rangle_{ABE}$ attaining $F(\rho_{AB},\sigma_{AB})$. Regard the very same vectors as purifications of $\rho_A,\sigma_A$ with ancillary system $BE$. Their overlap is among those maximized in the marginal purification formula, so

$$
\boxed{F(\rho_{AB},\sigma_{AB})=|\langle\psi|\phi\rangle|\leq F(\rho_A,\sigma_A)}.
$$

This proves the [monotonicity of quantum fidelity under partial trace](../../../../../../../monotonicity-of-quantum-fidelity-under-partial-trace.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
