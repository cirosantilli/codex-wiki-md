<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [spectral theorem](../../../../../spectral-theorem.md), the nonscalar unitary V has [orthonormal](../../../../../orthonormal-set.md) [eigenvectors](../../../../../eigenvector.md) $|v_0\rangle,|v_1\rangle$ with distinct [eigenvalues](../../../../../eigenvalue.md) $\lambda_0\ne\lambda_1$. Choose $|b\rangle=(|v_0\rangle+|v_1\rangle)/\sqrt2$. Then $V|b\rangle=(\lambda_0|v_0\rangle+\lambda_1|v_1\rangle)/\sqrt2$ is not proportional to $|b\rangle$.

On the product input $|+\rangle\otimes|b\rangle$, the [controlled unitary gate](../../../../../controlled-unitary-gate.md) produces

$$
U(|+\rangle\otimes|b\rangle)=\frac1{\sqrt2}\bigl(|0\rangle\otimes|b\rangle+|1\rangle\otimes V|b\rangle\bigr).
$$

Its two conditional target [vectors](../../../../../vector.md) are [linearly independent](../../../../../linear-independence.md), so the [conditional-vector product-state criterion](../../../../../conditional-vector-product-state-criterion.md) proves that the output is entangled. Equivalently, in the control [computational basis](../../../../../computational-basis.md) and target eigenbasis its [coefficient matrix](../../../../../coefficient-matrix.md) is $\tfrac12\bigl(\begin{smallmatrix}1&1\\\lambda_0&\lambda_1\end{smallmatrix}\bigr)$, whose determinant is $(\lambda_1-\lambda_0)/4\ne0$. Thus **U is an [entangling gate](../../../../../entangling-gate.md)**. The excluded scalar case would only apply a [phase gate](../../../../../phase-gate.md) to the control and could not entangle the factors; this is the [controlled-unitary entangling criterion](../../../../../controlled-unitary-entangling-criterion.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
