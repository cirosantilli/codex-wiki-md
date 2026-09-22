<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

Use [change of basis](../../../../../change-of-basis.md) matrices whose columns are the respective [basis vectors](../../../../../basis-vector.md) in standard coordinates:

$$
S_B=\begin{pmatrix}1&1\\1&-1\end{pmatrix},\quad
S_C=\begin{pmatrix}1&0&0\\1&1&1\\0&0&1\end{pmatrix},\quad
S_{B'}=\begin{pmatrix}0&2\\2&0\end{pmatrix},\quad
S_{C'}=\begin{pmatrix}1&0&1\\0&1&2\\-1&0&1\end{pmatrix}.
$$

The coordinate relation is $[\Phi(x)]_C=A[x]_B$. Therefore the standard-coordinate [matrix of a linear map](../../../../../matrix-representation-of-a-linear-map.md) is $T=S_CAS_B^{-1}$, and the new coordinate matrix is $A'=S_{C'}^{-1}TS_{B'}$. Multiplying gives

$$
T=\begin{pmatrix}0&1\\2&0\\0&-1\end{pmatrix},\qquad
TS_{B'}=\begin{pmatrix}2&0\\0&4\\-2&0\end{pmatrix},\qquad
\boxed{A'=\begin{pmatrix}2&0\\0&4\\0&0\end{pmatrix}.}
$$

One can also read off the columns: the two new domain [basis vectors](../../../../../basis-vector.md) map to twice the first and four times the second new codomain [basis vector](../../../../../basis-vector.md). All four [change of basis](../../../../../change-of-basis.md) matrices are invertible. In particular the printed codomain vectors are three-dimensional; retaining their third coordinates is essential.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
