<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expand the [matrix trace](../../../../../matrix-trace.md) explicitly:

$$
\mathcal L=\sum_{i,j=1}^N\left[\partial_\mu\Phi_{ij}^*\partial^\mu\Phi_{ij}-m^2\Phi_{ij}^*\Phi_{ij}\right].
$$

Write $\Phi_{ij}=(x_{ij}+iy_{ij})/\sqrt2$ and collect the $2N^2$ real fields into a vector $X$. Then

$$
\mathcal L=\frac12\sum_{A=1}^{2N^2}\left[\partial_\mu X_A\partial^\mu X_A-m^2X_A^2\right].
$$

Both quadratic forms are preserved by every constant [orthogonal matrix](../../../../../orthogonal-matrix.md) $R$, acting as $X\mapsto RX$. Thus the full linear internal symmetry contains $O(2N^2)$, with connected [special orthogonal group](../../../../../special-orthogonal-group.md) $SO(2N^2)$ as requested. The enlargement beyond unitary transformations is possible because the real and imaginary components have identical kinetic and [mass](../../../../../mass.md) terms and no interactions distinguishing them.

For a [Hermitian matrix](../../../../../hermitian-operator.md) $\Phi$, there are $N$ real diagonal entries and $N(N-1)/2$ independent complex off-diagonal entries, hence $N^2$ real fields. Choose an [orthonormal basis](../../../../../orthonormal-basis.md) $T_A$ of [Hermitian matrices](../../../../../hermitian-operator.md) for the [trace inner product](../../../../../frobenius-inner-product.md), $\operatorname{tr}(T_AT_B)=\delta_{AB}$, and put $\Phi=\sum_AX_AT_A/\sqrt2$. The same calculation gives

$$
\boxed{SO(2N^2)\ \text{for a general complex matrix},\qquad SO(N^2)\ \text{for a Hermitian matrix},}
$$

where these are the connected rotation groups; their full orthogonal extensions are $O(2N^2)$ and $O(N^2)$. A purely quadratic theory with $m^2<0$ would have an unstable [scalar potential](../../../../../scalar-potential.md), but this algebraic symmetry statement still holds.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
