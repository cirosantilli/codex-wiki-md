<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For any column vector $v$ and [positive semidefinite](../../../../positive-semidefinite-matrix.md) input $\varrho$, the [Kraus representation](../../../../kraus-representation.md) gives

$$
v^\dagger\mathcal E(\varrho)v=\sum_k(A_k^\dagger v)^\dagger\varrho(A_k^\dagger v)\geq0.
$$

Thus the output is [positive semidefinite](../../../../positive-semidefinite-matrix.md). The [cyclic property of the trace](../../../../cyclic-property-of-the-trace.md) and completeness of the [Kraus operators](../../../../kraus-operator.md) give

$$
\boxed{\operatorname{tr}\mathcal E(\varrho)=\operatorname{tr}\!\left(\varrho\sum_kA_k^\dagger A_k\right)=\operatorname{tr}\varrho.}
$$

More strongly, tensoring with an arbitrary [ancilla](../../../../quantum-ancilla.md) replaces $A_k$ by $A_k\otimes I$, so the same argument proves [complete positivity](../../../../completely-positive-map.md) rather than only positivity on single-system [density matrices](../../../../density-matrix-split.md).

If $\mathcal F$ has [Kraus operators](../../../../kraus-operator.md) $B_j$, the [composition of quantum channels](../../../../composition-of-quantum-channels.md) has

$$
(\mathcal F\circ\mathcal E)(\varrho)=\sum_{j,k}B_jA_k\varrho A_k^\dagger B_j^\dagger,
\qquad
\sum_{j,k}(B_jA_k)^\dagger B_jA_k
=\sum_kA_k^\dagger\!\left(\sum_jB_j^\dagger B_j\right)A_k=I.
$$

This is again a trace-preserving [Kraus representation](../../../../kraus-representation.md). The composition of [completely positive maps](../../../../completely-positive-map.md) is [completely positive](../../../../completely-positive-map.md) even without the trace-preserving assumption; in the general case, the product [Kraus operators](../../../../kraus-operator.md) still establish [complete positivity](../../../../completely-positive-map.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
