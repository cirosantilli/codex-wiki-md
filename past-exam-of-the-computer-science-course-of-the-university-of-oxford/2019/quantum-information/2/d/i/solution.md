<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider one normalized measurement [vector](../../../../../../vector.md) $|u\rangle=a|0\rangle+b|1\rangle$ on C. The unnormalized [partial inner product](../../../../../../partial-inner-product.md) on AB is

$$
|\chi_u\rangle=(I_{AB}\otimes\langle u|)|W\rangle=\frac1{\sqrt3}\bigl(\overline b|00\rangle+\overline a|01\rangle+\overline a|10\rangle\bigr).
$$

Its [tensor-product coefficient matrix](../../../../../../tensor-product-coefficient-matrix.md) and determinant are

$$
C_u=\frac1{\sqrt3}\begin{pmatrix}\overline b&\overline a\\\overline a&0\end{pmatrix},\qquad \det C_u=-\frac{\overline a^{\,2}}3.
$$

The [two-qubit product-state determinant criterion](../../../../../../two-qubit-product-state-determinant-criterion.md) therefore says that this branch is entangled whenever $a\ne0$. Its [probability](../../../../../../probability.md) is $(|b|^2+2|a|^2)/3>0$, so such a branch is physically possible and can be normalized without changing whether its determinant vanishes.

For an [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|u_0\rangle,|u_1\rangle\}$, completeness gives $|\langle0|u_0\rangle|^2+|\langle0|u_1\rangle|^2=1$. At least one [vector](../../../../../../vector.md) has $a\ne0$. Hence **at least one nonzero-probability outcome leaves AB entangled**, proving [conditional entanglement of the three-qubit W state](../../../../../../conditional-entanglement-of-the-three-qubit-w-state.md). Some bases give two entangled branches; the [computational basis](../../../../../../computational-basis.md) gives one entangled and one product branch. The claim is not that every outcome must entangle AB.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
