<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The gate set is not universal.** The displayed two-[qubit](../../../../../../qubit.md) [matrix](../../../../../../matrix.md) is the [SWAP gate](../../../../../../swap-gate.md):

$$
W(|u\rangle\otimes|v\rangle)=|v\rangle\otimes|u\rangle.
$$

Both $V$ and the [Hadamard gate](../../../../../../hadamard-gate.md) act on one [qubit](../../../../../../qubit.md). Thus every gate preserves a fully factored [product state](../../../../../../product-state.md), and induction gives the same property for every [quantum circuit](../../../../../../quantum-circuit-split.md) built from them. This is the [product-state obstruction to SWAP universality](../../../../../../product-state-obstruction-to-swap-universality.md).

For a quantitative obstruction to even approximate universality, every two-[qubit](../../../../../../qubit.md) [product state](../../../../../../product-state.md) has squared overlap at most $1/2$ with a [Bell state](../../../../../../bell-state-split.md). Indeed, for normalized coefficient vectors $u,v$,

$$
|\langle\phi_+|u\otimes v\rangle|^2
=\frac{|u_0v_0+u_1v_1|^2}{2}\leq\frac12
$$

by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). A [controlled-NOT gate](../../../../../../controlled-not-gate.md) acting on $|+\rangle|0\rangle$ would instead produce that [Bell state](../../../../../../bell-state-split.md), so these circuits cannot approximate all [unitary transformations](../../../../../../unitary-operator.md). The fact that $V^2=e^{-i\pi/8}T$ supplies a [T gate](../../../../../../t-gate.md) up to [global phase](../../../../../../global-phase.md) does not supply an [entangling gate](../../../../../../entangling-gate.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
