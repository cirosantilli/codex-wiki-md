<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First choose the same orthonormal [basis](../../../../basis.md) for the left and right copies of the two-dimensional [unitary representation](../../../../unitary-representation.md) $D$. Then the family [representation](../../../../group-representation.md) is $F=D\oplus\varepsilon$. Because the barred [fermion](../../../../fermion.md) transforms with $F(g)^\dagger$ and the [scalar field](../../../../scalar-field.md) $H$ is a [trivial representation](../../../../trivial-representation.md), invariance of the [Yukawa interaction](../../../../yukawa-interaction.md) requires

$$
F(g)^\dagger\lambda F(g)=\lambda,
\quad\text{equivalently}\quad \lambda F(g)=F(g)\lambda
\qquad(g\in S_3).
$$

Write $\lambda$ in a $2+1$ block form. The off-diagonal blocks would be [intertwiners](../../../../intertwiner.md) between inequivalent [irreducible representations](../../../../irreducible-representation.md) $D$ and $\varepsilon$, so the [Schur lemma](../../../../schur-s-lemma.md) makes them zero. The doublet block must be a scalar [matrix](../../../../matrix.md), while the singlet block is arbitrary. Therefore

$$
\boxed{\lambda=\begin{pmatrix}a&0&0\\0&a&0\\0&0&b\end{pmatrix},\qquad a,b\in\mathbb C.}
$$

Equivalently, the allowed [Yukawa interaction](../../../../yukawa-interaction.md) is $H[a(\bar\psi_L^1\psi_R^1+\bar\psi_L^2\psi_R^2)+b\bar\psi_L^3\psi_R^3]$, together with its [Hermitian conjugate](../../../../hermitian-conjugation.md) when constructing a real [Lagrangian](../../../../lagrangian.md). The [tensor product](../../../../tensor-product.md) rules explain the two free parameters: both $D^*\otimes D$ and $\varepsilon^*\otimes\varepsilon$ contain one [trivial representation](../../../../trivial-representation.md), while the mixed products contain none.

There is a useful [basis](../../../../basis.md) qualification. The [basis](../../../../basis.md) used in [solution](../c/solution.md) is not orthonormal: its [Gram matrix](../../../../gram-matrix.md) is $K=\begin{pmatrix}2&1\\1&2\end{pmatrix}$, and $D(g)^\dagger KD(g)=K$. If the fields are expressed in exactly those coordinates, with the barred components defined by ordinary conjugate transpose, the invariant doublet coefficient is $aK$, rather than $aI_2$. Canonically normalizing the [kinetic term](../../../../kinetic-term.md) returns the boxed form. Independently chosen left and right orthonormal [bases](../../../../basis.md) replace $aI_2$ by $aS$, where $S$ is their fixed unitary [intertwiner](../../../../intertwiner.md); the physical degeneracy is unchanged.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
