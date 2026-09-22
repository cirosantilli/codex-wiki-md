<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [local Hamiltonian](../../../../../../../local-hamiltonian.md) as $H=\sum_{j=1}^mh_j$. Since its terms commute, their [matrix exponentials](../../../../../../../matrix-exponential.md) factor exactly:

$$
e^{-iHt}=\prod_{j=1}^me^{-ih_jt}.
$$

Each factor acts on at most two qubits and can be compiled over a fixed [universal quantum gate set](../../../../../../../universal-quantum-gate-set.md) to [operator norm](../../../../../../../operator-norm.md) error at most $\varepsilon/m$. The [telescoping bound for products of operators](../../../../../../../telescoping-bound-for-products-of-operators.md) then bounds the total error by the sum of the factor errors, at most $\varepsilon$. Because $m$ is polynomial in $n$ and the [Solovay--Kitaev theorem](../../../../../../../solovay-kitaev-theorem.md) gives gate count polynomial in $\log(m/\varepsilon)$ for each fixed-dimensional factor, this is an efficient [commuting local Hamiltonian simulation](../../../../../../../commuting-local-hamiltonian-simulation.md). Finally, the [eigenvalue equation](../../../../../../../eigenvalue-equation.md) $H|\Psi\rangle=\lambda|\Psi\rangle$ implies

$$
U(t)|\Psi\rangle=e^{-i\lambda t}|\Psi\rangle,
$$

so $|\Psi\rangle$ remains an [eigenstate](../../../../../../../eigenstate.md) and its eigenvalue is $e^{-i\lambda t}$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
