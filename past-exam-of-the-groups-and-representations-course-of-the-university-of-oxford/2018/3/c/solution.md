<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the following [Pauli matrix](../../../../pauli-matrices.md) realization, with its spinor [basis](../../../../basis.md) fixed for the later [Dirac adjoint](../../../../dirac-adjoint.md):

$$
\boxed{r(K_1)=\frac{\sigma_3}{2}=\frac12\begin{pmatrix}1&0\\0&-1\end{pmatrix},\quad
r(K_2)=-\frac{\sigma_2}{2}=\frac12\begin{pmatrix}0&i\\-i&0\end{pmatrix},\quad
r(J)=-\frac{i\sigma_1}{2}=\frac12\begin{pmatrix}0&-i\\-i&0\end{pmatrix}.}
$$

The [Pauli matrix](../../../../pauli-matrices.md) multiplication rule verifies

$$
[r(J),r(K_1)]=r(K_2),\qquad
[r(J),r(K_2)]=-r(K_1),\qquad
[r(K_1),r(K_2)]=-r(J).
$$

Extending linearly therefore gives a two-dimensional [Lie algebra representation](../../../../lie-algebra-representation.md). For an [irreducible representation](../../../../irreducible-representation.md), it suffices to rule out an invariant line. Any such line would have to be an [eigenline](../../../../eigenline.md) of $r(K_1)$, whose two [eigenvalues](../../../../eigenvalue.md) are distinct. Those two coordinate lines are interchanged by $r(K_2)$, so neither is invariant. There is no proper nonzero [invariant subspace](../../../../invariant-subspace.md).

This is a spinorial [representation](../../../../group-representation.md) rather than a single-valued two-dimensional [representation](../../../../group-representation.md) of the identity component of the specified orthogonal [group](../../../../group-split.md):

$$
 e^{2\pi J}=I_3,\qquad e^{2\pi r(J)}=-I_2.
$$

The mismatch explicitly exhibits the need for the spin double cover. It causes no obstruction to the requested infinitesimal construction.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
