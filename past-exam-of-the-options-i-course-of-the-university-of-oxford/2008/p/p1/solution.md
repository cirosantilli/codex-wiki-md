<h1 id="p/p1/solution">Solution</h1>

↑ **Parent:** [P1](../p1.md)

Use [Gaussian elimination with partial pivoting](../../../../gaussian-elimination.md), choosing a largest absolute entry in the uneliminated part of each pivot column. The first pivot is two in row one, with multipliers $1/2,1/2,1/5$ for rows two, three and four. The second-column candidates are then $-1,0,-2/5$, so row two stays as pivot and the remaining nonzero multiplier is $2/5$ for row four. The augmented matrix at this stage is

$$
\left(\begin{array}{rrrr|r}2&-1&4&2&3\\0&-1&3&2&1\\0&0&-3/4&-3/2&0\\0&0&3&-2&0\end{array}\right).
$$

The third pivot is three, so swap rows three and four. The final multiplier is $-1/4$, leaving last pivot $-2$. Carrying that swap through the previously stored multipliers gives

$$
P=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&0&0&1\\0&0&1&0\end{pmatrix},\qquad
L=\begin{pmatrix}1&0&0&0\\1/2&1&0&0\\1/5&2/5&1&0\\1/2&0&-1/4&1\end{pmatrix},
$$



$$
\boxed{U=\begin{pmatrix}2&-1&4&2\\0&-1&3&2\\0&0&3&-2\\0&0&0&-2\end{pmatrix},\qquad PA=LU}.
$$

The transformed right side is $(3,1,0,0)^T$. Back substitution gives $z=0$, $y=0$, $x=-1$ and $w=1$, hence $\boxed{(w,x,y,z)=(1,-1,0,0)}$.

For the [eigenvalue](../../../../eigenvalue.md) claim, put $S=P^TL$. It is invertible because a [permutation matrix](../../../../permutation-matrix.md) and a unit [lower triangular matrix](../../../../lower-triangular-matrix.md) are invertible. The factorization gives $A=SU$, so

$$
\boxed{S^{-1}AS=US=UP^TL=B}.
$$

Similar matrices have the same [characteristic polynomial](../../../../characteristic-polynomial.md) and therefore the same eigenvalues with algebraic multiplicities. This proves the claim without changing the prescribed elimination method.

## ↑ Ancestors (12)

1. [P1](../p1.md)
2. [P](../../p.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
