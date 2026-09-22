<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Conjugation by one [Pauli matrix](../../../../pauli-matrices.md) fixes that same matrix and reverses the other two. For example, $X X X=X$, $Y X Y=-X$, and $Z X Z=-X$. Applying this to each component of the [Bloch vector](../../../../bloch-vector.md) gives

$$
\sum_{j=x,y,z}\sigma_j\varrho\sigma_j
=\frac12(3I-\mathbf s\cdot\boldsymbol\sigma).
$$

Hence the [quantum depolarizing channel](../../../../quantum-depolarizing-channel.md) is

$$
\mathcal E_p(\varrho)
=\frac12\left[I+\left(1-\frac{4p}{3}\right)\mathbf s\cdot\boldsymbol\sigma\right],
\qquad
\boxed{\mathbf s'=\frac{3-4p}{3}\mathbf s.}
$$

The [Kraus operators](../../../../kraus-operator.md) $\sqrt{1-p}\,I$ and $\sqrt{p/3}\,\sigma_j$ establish [complete positivity](../../../../completely-positive-map.md) for $0\leq p\leq1$. At $p=3/4$ every state becomes [maximally mixed](../../../../maximally-mixed-state.md). For $p>3/4$ the factor is negative: it reverses the vector as well as reducing its length. Its most negative value is $-1/3$, consistent with the complete-positivity range of the [isotropic qubit map](../../../../isotropic-qubit-map.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
