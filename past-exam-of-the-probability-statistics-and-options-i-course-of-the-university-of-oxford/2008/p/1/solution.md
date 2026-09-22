<h1 id="p/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [Gaussian elimination](../../../../gaussian-elimination.md) with [partial pivoting](../../../../columnwise-partial-pivoting.md), choosing the largest absolute available entry in the current pivot column. The first pivot is 2, with multipliers $1/2,1/2,1/5$. After eliminating that column, the augmented system is

$$
\left(\begin{array}{rrrr|r}
2&-1&4&2&3\\0&-1&3&2&1\\
0&0&-3/4&-3/2&0\\0&-2/5&21/5&-6/5&2/5
\end{array}\right).
$$

The second pivot is $-1$, already largest in its remaining column. Its multipliers are zero and $2/5$, giving row four $(0,0,3,-2\mid0)$. In column three, partial pivoting now requires exchanging rows three and four, since $3>3/4$. The final elimination multiplier is $-1/4$. Thus

$$
U=\begin{pmatrix}
2&-1&4&2\\0&-1&3&2\\0&0&3&-2\\0&0&0&-2
\end{pmatrix},\qquad
b_{\rm elim}=(3,1,0,0)^T.
$$

Back substitution gives $\boxed{(w,x,y,z)=(1,-1,0,0)}$.

The permutation and recorded multipliers, with the earlier multiplier rows swapped at the third pivot, are

$$
P=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&0&0&1\\0&0&1&0\end{pmatrix},\qquad
L=\begin{pmatrix}
1&0&0&0\\1/2&1&0&0\\1/5&2/5&1&0\\1/2&0&-1/4&1
\end{pmatrix}.
$$

Direct multiplication verifies $PA=LU$. Since $U$ is invertible and $A=P^TLU$,

$$
UP^TL=UAU^{-1}.
$$

The two matrices are similar, and similar matrices have the same characteristic polynomial and eigenvalues.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [P](../../p.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
