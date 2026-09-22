<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For any normalized vector $|u\rangle$, the [Born rule](../../../../born-rule.md) assigns the [probability](../../../../probability.md) $\langle u|\rho|u\rangle$ to the corresponding rank-one [orthogonal projection](../../../../orthogonal-projection.md). This must be nonnegative for every $u$, which is exactly [positive semidefiniteness](../../../../positive-semidefinite-matrix.md). For any complete [orthonormal basis](../../../../orthonormal-basis.md) $\{|j\rangle\}$, the outcome [probabilities](../../../../probability.md) must sum to one:

$$
\sum_j\langle j|\rho|j\rangle=\operatorname{Tr}\rho=1.
$$

Thus a [Hermitian matrix](../../../../hermitian-operator.md) represents a physical [density matrix](../../../../density-matrix-split.md) only if

$$
\boxed{\rho\geq0,\qquad\operatorname{Tr}\rho=1.}
$$

These conditions are also sufficient in finite dimension. The [spectral theorem](../../../../spectral-theorem.md) writes $\rho=\sum_jp_j|u_j\rangle\langle u_j|$ with $p_j\geq0$ and $\sum_jp_j=1$, describing a [quantum state ensemble](../../../../quantum-state-ensemble.md) of [pure states](../../../../pure-state.md) with valid mixing [probabilities](../../../../probability.md). A [Hermitian matrix](../../../../hermitian-operator.md) alone could have negative [eigenvalues](../../../../eigenvalue.md), hence negative measurement [probabilities](../../../../probability.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
