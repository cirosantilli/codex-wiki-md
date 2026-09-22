<h1 id="p/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a complex [matrix](../../../../matrix.md) $C=(c_{ij})$, Gershgorin's theorem puts every [eigenvalue](../../../../eigenvalue.md) in the union of the row discs $D_i=\{z:|z-c_{ii}|\leq R_i\}$, where $R_i=\sum_{j\ne i}|c_{ij}|$. To prove it, choose an [eigenvector](../../../../eigenvector.md) $v$ for an [eigenvalue](../../../../eigenvalue.md) $\lambda$ and an index $i$ maximizing $|v_i|>0$. Its $i$th equation gives

$$
|\lambda-c_{ii}|\,|v_i|\leq\sum_{j\ne i}|c_{ij}|\,|v_j|\leq R_i|v_i|.
$$

Division proves $\lambda\in D_i$.

The usual counting refinement says that a connected component made of $k$ discs contains exactly $k$ [eigenvalues](../../../../eigenvalue.md), with [algebraic multiplicity](../../../../algebraic-multiplicity.md). For completeness, deform the [matrix](../../../../matrix.md) from its diagonal part to the original by multiplying all off-diagonal entries by $t\in[0,1]$. Its discs have radii $tR_i$ and stay inside the original discs. Continuous variation of the roots of the [characteristic polynomial](../../../../characteristic-polynomial.md) keeps the number inside any contour separating one original component from the others constant. At $t=0$, the diagonal entries give exactly $k$ roots there, proving the refinement.

For the application put $s=-\mu>0$. The [matrix](../../../../matrix.md) is

$$
A+sB=\begin{pmatrix}2+2s&-2&0\\-3&5+2s&s\\1&2+s&3+2s\end{pmatrix}.
$$

Its three row discs have positive real centres and leftmost real coordinates

$$
(2+2s)-2=2s,\qquad(5+2s)-(3+s)=2+s,\qquad(3+2s)-(3+s)=s.
$$

All are strictly positive, so zero lies in none of the discs. It cannot be an [eigenvalue](../../../../eigenvalue.md). Thus **$A-\mu B$ is nonsingular for every real $\mu<0$**.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [P](../../p.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
