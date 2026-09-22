<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\mathbf1$ for the [trivial representation](../../../../trivial-representation.md), $\varepsilon$ for the [sign representation](../../../../sign-representation.md), and $\mathbf2$ for the given two-dimensional [group representation](../../../../group-representation.md). Their [matrix representations](../../../../matrix-representation.md) on the [generators of a group](../../../../generator-of-a-group.md) are

$$
\begin{array}{c|cc}
 &r&s\\\hline
\mathbf1&1&1\\
\varepsilon&1&-1\\
\mathbf2&\operatorname{diag}(\alpha,\alpha^{-1})&\begin{pmatrix}0&1\\1&0\end{pmatrix}
\end{array}
$$

with $\alpha=e^{2\pi i/3}$. The two [eigenvalues](../../../../eigenvalue.md) of $r$ in $\mathbf2$ are distinct, and $s$ exchanges its two [eigenlines](../../../../eigenline.md); no line is invariant under both. Thus $\mathbf2$ is an [irreducible representation](../../../../irreducible-representation.md). The dimensions already exhaust the [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md), so this is the complete list.

Since $\alpha+\alpha^{-1}=-1$, the [character table](../../../../character-table.md) is

$$
\boxed{
\begin{array}{c|rrr}
\text{class}&I&\{r,r^2\}&\{s,rs,r^2s\}\\
\text{class size}&1&2&3\\\hline
\chi_{\mathbf1}&1&1&1\\
\chi_{\varepsilon}&1&1&-1\\
\chi_{\mathbf2}&2&-1&0
\end{array}.}
$$

Multiplying [characters](../../../../character-of-a-representation.md) and using [character orthogonality](../../../../character-orthogonality.md) gives every [tensor product of group representations](../../../../tensor-product-of-group-representations.md):

$$
\boxed{
\begin{array}{c|ccc}
\otimes&\mathbf1&\varepsilon&\mathbf2\\\hline
\mathbf1&\mathbf1&\varepsilon&\mathbf2\\
\varepsilon&\varepsilon&\mathbf1&\mathbf2\\
\mathbf2&\mathbf2&\mathbf2&\mathbf1\oplus\varepsilon\oplus\mathbf2
\end{array}.}
$$

For example $\chi_{\mathbf2}^2=(4,1,0)=\chi_{\mathbf1}+\chi_\varepsilon+\chi_{\mathbf2}$. Explicit [Clebsch-Gordan coefficients](../../../../clebsch-gordan-coefficients.md) can be read from two doublets $x=(x_1,x_2)^T$, $y=(y_1,y_2)^T$:

$$
\mathbf1:\ x_1y_2+x_2y_1,\qquad
\varepsilon:\ x_1y_2-x_2y_1,\qquad
\mathbf2:\ \begin{pmatrix}x_2y_2\\x_1y_1\end{pmatrix}.
$$

The first two combinations are invariant under $r$ and respectively even and odd under $s$; the last transforms by the displayed doublet [matrices](../../../../matrix.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
