<h1 id="1/f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [controlled-NOT gate](../../../../../../controlled-not-gate.md) is its own inverse, so $\mathrm{CNOT}^2=I$. Every remaining nontrivial gate acts on one wire. By the [tensor product](../../../../../../tensor-product.md) rule, any circuit on a product input stays a [product state](../../../../../../product-state.md); in particular, starting at $|00\rangle$ it cannot produce a [Bell state](../../../../../../bell-state-split.md).

This also prevents arbitrary approximation, not merely exact preparation. For normalized single-qubit [vectors](../../../../../../vector.md) $|u\rangle,|v\rangle$,

$$
|\langle\Phi^+|u\otimes v\rangle|^2=\tfrac12|u_0v_0+u_1v_1|^2\leq\tfrac12
$$

by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Hence the [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) with $|\Phi^+\rangle$ is bounded away from one for every reachable state. **This gate set is not universal.** The obstruction is preservation of [product states](../../../../../../product-state.md), a special case of the existing [product-state obstruction to SWAP universality](../../../../../../product-state-obstruction-to-swap-universality.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [F](../../f.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
