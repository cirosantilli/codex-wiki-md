<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the two complementary [projection operators](../../../../projection-linear-algebra.md)

$$
P_+=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix},\qquad
P_-=\frac12\begin{pmatrix}1&-1\\-1&1\end{pmatrix}.
$$

They obey $P_++P_-=I_2$, $P_+P_-=0$ and $P_\pm^2=P_\pm$. The given [matrix](../../../../matrix.md) is $A=P_++\alpha P_-$, and consequently

$$
A^g=P_++\alpha^gP_-,\qquad A^3=I_2.
$$

It follows that multiplication of these [matrices](../../../../matrix.md) respects addition modulo three:

$$
R(g)R(h)=A^{g+h}=R(g+h\bmod3),\qquad R(0)=I_2.
$$

Thus this is a [group representation](../../../../group-representation.md). The [eigenvectors](../../../../eigenvector.md) $(1,1)^T$ and $(1,-1)^T$ have [eigenvalues](../../../../eigenvalue.md) $1$ and $\alpha$, respectively. They span invariant lines carrying $\chi_0$ and $\chi_1$ in the convention of [c](../c.md), so

$$
\boxed{R\cong\rho_0\oplus\rho_1,\qquad \chi_R=(2,1+\alpha,1+\alpha^2).}
$$

The other nontrivial [irreducible representation](../../../../irreducible-representation.md), $\rho_2$, is absent.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
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
