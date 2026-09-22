<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The given [permutations](../../../../permutation.md) satisfy $r^4=s^2=1$ and $srs=r^{-1}$. The eight elements $r^j,r^js$ for $0\leq j<4$ are distinct: $s\notin\langle r\rangle$, whose only element of order two is $r^2=(13)(24)$. Thus $H$ is the order-eight [dihedral group](../../../../dihedral-group.md), and we may use the [matrices](../../../../matrix.md)

$$
R=\sigma(r)=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
S=\sigma(s)=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

They obey the same relations and describe a quarter-turn and a [reflection](../../../../reflection-mathematics.md) of a [square](../../../../square.md).

The [eigenvalues](../../../../eigenvalue.md) of $R$ over the [complex numbers](../../../../complex-number.md) are $i$ and $-i$, with respective [eigenlines](../../../../eigenline.md) spanned by $(1,-i)$ and $(1,i)$. Since $S$ interchanges these [eigenlines](../../../../eigenline.md), neither is an [invariant subspace](../../../../invariant-subspace.md) for $H$. Any proper nonzero [subrepresentation](../../../../subrepresentation.md) of this two-dimensional [complex representation](../../../../complex-representation.md) would be a line invariant under both $R$ and $S$, and an $R$-invariant line must be one of those [eigenlines](../../../../eigenline.md). None qualifies, so **$W$ is irreducible**.

For the calculation in part (e), its [character](../../../../character-of-a-representation.md) is

$$
\chi_W(1)=2,\qquad \chi_W(r^2)=-2,\qquad
\chi_W(r)=\chi_W(r^3)=\chi_W(r^js)=0\quad(0\leq j<4).
$$

Indeed $R^2=-I$, while a quarter-turn or a [reflection](../../../../reflection-mathematics.md) has [trace](../../../../matrix-trace.md) zero. The [character inner product](../../../../character-inner-product.md) $(2^2+(-2)^2)/8=1$ provides a second irreducibility check.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to representation theory course of the University of Oxford](../../../split.md)
5. [Introduction to representation theory course of the University of Oxford](../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
