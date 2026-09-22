<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each summand of $J_X$ acts on one [qubit](../../../../../../qubit.md), while each summand $Z_iZ_j$ of $J_Z$ acts on two. Therefore $J=J_X+J_Z$ is a [2-local Hamiltonian](../../../../../../k-local-hamiltonian.md). We have

$$
\|J_X\|=O(n),
\qquad
\|J_Z\|\leq\binom n2=O(n^2).
$$

Split $t$ into $r$ steps of length $\delta=t/r$ and use the [second-order product formula](../../../../../../second-order-product-formula.md)

$$
S_2(\delta)=
e^{-i\delta J_X/2}e^{-i\delta J_Z}e^{-i\delta J_X/2}.
$$

For one step, $\Lambda=O(\delta n^2)$ in the stated estimate, so the [spectral-norm error](../../../../../../matrix-2-norm.md) is $O(\delta^3n^6)$. The error bound for a product of [unitary operators](../../../../../../unitary-operator.md) makes the total error

$$
O(r\delta^3n^6)=O\left(\frac{n^6t^3}{r^2}\right).
$$

It is therefore enough to choose

$$
r=O\left(\frac{n^3t^{3/2}}{\sqrt\epsilon}\right),
$$

with $r$ also large enough that the small-step estimate applies.

All $Z_iZ_j$ terms [commute](../../../../../../commuting-operators.md). A factor $e^{-i\delta Z_iZ_j}$ uses a constant-size circuit of two [controlled-NOT gates](../../../../../../controlled-not-gate.md) and one [phase gate](../../../../../../phase-gate.md), up to a [global phase](../../../../../../global-phase.md), so one product-formula step costs $O(n^2)$ gates. The complete [Hamiltonian simulation](../../../../../../hamiltonian-simulation.md) consequently has size

$$
\boxed{O\left(\frac{n^5t^{3/2}}{\sqrt\epsilon}\right)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
