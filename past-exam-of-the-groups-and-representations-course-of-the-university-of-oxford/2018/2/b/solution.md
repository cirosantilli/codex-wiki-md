<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a one-dimensional [representation](../../../../group-representation.md), the relation $srs=r^{-1}$ implies $\rho(r)=\rho(r)^{-1}$, so $\rho(r)=\delta\in\{\pm1\}$. Independently $\rho(s)=\epsilon\in\{\pm1\}$. These give four [irreducible representations](../../../../irreducible-representation.md)

$$
\chi_{\epsilon,\delta}(r^ks^\ell)=\delta^k\epsilon^\ell.
$$

A two-dimensional [representation](../../../../group-representation.md) $E$ is obtained by restricting the given [matrices](../../../../matrix.md) to the $yz$ plane:

$$
E(r)=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad
E(s)=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

The [eigenvalues](../../../../eigenvalue.md) of $E(r)$ are $i$ and $-i$. Its two [eigenlines](../../../../eigenline.md) are interchanged by $E(s)$, so neither is invariant under the whole [group](../../../../group-split.md). Thus $E$ is a complex [irreducible representation](../../../../irreducible-representation.md).

Taking [traces](../../../../matrix-trace.md) gives the [character table](../../../../character-table.md), with class sizes included for the [character inner product](../../../../character-inner-product.md):

$$
\boxed{\begin{array}{c|rrrrr}
 &C_0&C_1&C_2&C_3&C_4\\
|C_j|&1&1&2&2&2\\\hline
\chi_{+,+}&1&1&1&1&1\\
\chi_{+,-}&1&1&1&-1&-1\\
\chi_{-,+}&1&1&-1&1&-1\\
\chi_{-,-}&1&1&-1&-1&1\\
\chi_E&2&-2&0&0&0
\end{array}.}
$$

For example $\langle\chi_E,\chi_E\rangle=(4+4)/8=1$, and its inner product with each one-dimensional row is $(2-2)/8=0$. The four one-dimensional rows are mutually orthonormal by direct weighted summation. Their squared [dimensions](../../../../dimension-vector-space.md) sum to $4\cdot1^2+2^2=8=|G|$, and there are five rows for five [conjugacy classes](../../../../conjugacy-class.md). This proves completeness of the list.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
