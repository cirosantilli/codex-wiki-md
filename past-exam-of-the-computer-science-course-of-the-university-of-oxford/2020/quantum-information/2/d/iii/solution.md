<h1 id="2/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Extend the normalized [vector](../../../../../../vector.md) $|\phi\rangle$ to an [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|f_j\rangle\}_{j=1}^d$ with $|f_1\rangle=|\phi\rangle$, and extend $|\psi\rangle$ to an [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|e_j\rangle\}_{j=1}^d$ with $|e_1\rangle=|\psi\rangle$. The [Gram-Schmidt process](../../../../../../gram-schmidt-process.md) provides such extensions. Define

$$
U=\sum_{j=1}^d|e_j\rangle\langle f_j|.
$$

Then $U^\dagger U=\sum_j|f_j\rangle\langle f_j|=I$ and $UU^\dagger=I$, so $U$ is unitary and $U|\phi\rangle=|\psi\rangle$. Construct $V$ on the second subsystem in the same way, sending $|\phi'\rangle$ to $|\psi'\rangle$. Consequently

$$
(U\otimes V)(|\phi\rangle\otimes|\phi'\rangle)=|\psi\rangle\otimes|\psi'\rangle.
$$

Thus **any two normalized [product states](../../../../../../product-state.md) on the same pair of subsystem spaces are [local-unitary equivalent](../../../../../../local-unitary-equivalence.md)**. The dimension and [normalization](../../../../../../normalization.md) requirements matter because a unitary preserves both its domain and [vector](../../../../../../vector.md) [norms](../../../../../../norm.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
