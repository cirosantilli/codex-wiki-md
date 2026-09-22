# Controlled-unitary entangling criterion

↑ **Parent:** [Controlled unitary gate](controlled-unitary-gate.md)

For a [qubit](qubit.md) control and finite-dimensional target with [unitary operator](unitary-operator.md) V, the [controlled unitary gate](controlled-unitary-gate.md) $C(V)=|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes V$ is entangling if and only if V is not scalar. If $V=e^{i\theta}I$, the controlled operation is a [phase gate](phase-gate.md) on the control tensored with the target identity and preserves every [product state](product-state.md).

Otherwise the [spectral theorem](spectral-theorem.md) supplies two [orthonormal](orthonormal-set.md) [eigenvectors](eigenvector.md) with distinct [eigenvalues](eigenvalue.md) $\lambda_0,\lambda_1$. Set $|b\rangle=(|v_0\rangle+|v_1\rangle)/\sqrt2$ and use product input $|+\rangle|b\rangle$. The two conditional target [vectors](vector.md) $|b\rangle$ and $V|b\rangle$ are [linearly independent](linear-independence.md) because their eigenbasis coefficients would otherwise require $\lambda_0=\lambda_1$. The [conditional-vector product-state criterion](conditional-vector-product-state-criterion.md) shows that their coherent controlled superposition is entangled. Thus even a target gate arbitrarily close to scalar can be entangling, although the resulting entanglement need not be large.

## ↑ Ancestors (5)

1. [Controlled unitary gate](controlled-unitary-gate.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/quantum-information/3/c/solution.md)
