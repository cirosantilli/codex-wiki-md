# First-order two-local Hamiltonian simulation

↑ **Parent:** [Product-formula Hamiltonian simulation](product-formula-hamiltonian-simulation.md)

For a sum of $M$ Hermitian two-local terms of norm below one, repeat a first-order [Lie-Trotter product formula](lie-product-formula.md) step $r$ times. The [first-order unitary product-formula error bound](first-order-unitary-product-formula-error-bound.md) gives total error at most $t^2\sum_{j<k}\|[H_j,H_k]\|/(2r)<M(M-1)t^2/(2r)$ for $M>1$. Taking $r=\max(1,\lceil M(M-1)t^2/(2\epsilon)\rceil)$ uses $Mr$ arbitrary two-qubit gates. At unit time and $M=O(n^2)$ this is a sufficient $O(n^6/\epsilon)$ bound; additional commutation structure can improve it.

## ↑ Ancestors (6)

1. [Product-formula Hamiltonian simulation](product-formula-hamiltonian-simulation.md)
2. [Hamiltonian simulation](hamiltonian-simulation.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/4/ii/solution.md)
