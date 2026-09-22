<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For sufficiently weak local fields the bulk gap remains open, so [quasi-adiabatic continuation](../../../../../../quasi-adiabatic-continuation.md) supplies a quasi-local unitary $U$ mapping the unperturbed ground space to the span of the $2^k$ lowest eigenstates:

$$
|\varphi_\alpha\rangle=U|\psi_\alpha\rangle.
$$

If $S_j$, $j=1,\ldots,n-k$, are independent original stabilizer generators, define

$$
\boxed{\widetilde S_j=US_jU^\dagger.}
$$

Then $\widetilde S_j|\varphi_\alpha\rangle=|\varphi_\alpha\rangle$, and independence is preserved by conjugation. The operators $\widetilde S_j$ are quasilocal, with exponentially decaying tails, but a generic perturbation makes them non-Pauli; this is the [dressed stabilizer under a weak local perturbation](../../../../../../dressed-stabilizer-under-a-weak-local-perturbation.md).

Exact error correction is transported with the code: the exactly correctable dressed errors are $UE_aU^\dagger$. A bare Pauli error is generally not one of these dressed operators. Its expansion in the dressed algebra has exponentially small long-range components that can act within the logical space, so

$$
\Pi_H E_a^\dagger E_b\Pi_H
=c_{ab}\Pi_H+\text{exponentially small logical terms}.
$$

**Thus a set of bare Pauli errors satisfies the KL conditions only approximately, with deviations suppressed exponentially by the code distance relative to the dressing length, except at specially tuned points.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
