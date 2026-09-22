<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The columns of $P$ are the coordinates of the vectors $\mathbf f_j$, so they form a basis exactly when

$$
\boxed{\det P\ne0}.
$$

For a [linear transformation](../../../../../linear-map.md) $\alpha$, define its [matrix representation](../../../../../matrix-representation.md) in the standard basis by

$$
[\alpha(\mathbf v)]_{\mathbf e}=A[\mathbf v]_{\mathbf e},
\qquad A_{ij}=[\alpha(\mathbf e_j)]_i.
$$

The [change-of-basis matrix](../../../../../change-of-basis-matrix.md) satisfies $[\mathbf v]_{\mathbf e}=P[\mathbf v]_{\mathbf f}$. Therefore

$$
P[\alpha(\mathbf v)]_{\mathbf f}
=A P[\mathbf v]_{\mathbf f},
$$

and multiplication by $P^{-1}$ gives the [similar matrix](../../../../../matrix-similarity.md) relation

$$
\boxed{\widetilde A=P^{-1}AP}.
$$

The characteristic polynomial of the displayed $A$ is

$$
(\lambda-1)(\lambda-2)^2.
$$

Eigenvectors $(2,-1,2)^T$, $(1,0,0)^T$, and $(0,-1,3)^T$ give

$$
P=\begin{pmatrix}2&1&0\\-1&0&-1\\2&0&3\end{pmatrix},
\qquad
B=\begin{pmatrix}1&0&0\\0&2&0\\0&0&2\end{pmatrix}.
$$

Indeed, $\det P=1$ and

$$
AP=\begin{pmatrix}2&2&0\\-1&0&-2\\2&0&6\end{pmatrix}=PB,
$$

so $P^{-1}AP=B$. Finally, the [diagonalization of a matrix](../../../../../diagonalization-of-a-matrix.md) gives

$$
A^nP=PB^n
=\boxed{\begin{pmatrix}
2&2^n&0\\
-1&0&-2^n\\
2&0&3\,2^n
\end{pmatrix}}.
$$

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
