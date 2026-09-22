<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

For the standard basis vector $e_j$, matrix multiplication selects the $j$th column, so

$$
Me_j=c_j.
$$

Consequently

$$
(PM)e_j=P(Me_j)=Pc_j,
$$

and the columns of $PM$ are $Pc_1,\ldots,Pc_n$.

Suppose first that $v,Av,\ldots,A^{n-1}v$ are linearly independent, and define

$$
S=\begin{pmatrix}v&Av&\cdots&A^{n-1}v\end{pmatrix}.
$$

Then $S$ is invertible. The first $n-1$ columns of $AS$ are the last $n-1$ columns of $S$. By the [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md),

$$
A^nv=-a_0v-a_1Av-\cdots-a_{n-1}A^{n-1}v.
$$

This is exactly the last-column rule for the [companion matrix](../../../../../companion-matrix.md) $C$, so

$$
AS=SC,\qquad S^{-1}AS=C.
$$

Conversely, suppose $S^{-1}AS=C$, or $AS=SC$, and write the columns of $S$ as $s_1,\ldots,s_n$. Comparing the first $n-1$ columns gives

$$
As_j=s_{j+1}\qquad(1\leq j<n).
$$

Hence

$$
s_j=A^{j-1}s_1.
$$

Since $S$ is invertible, its columns are linearly independent. Taking $v=s_1$ therefore makes

$$
v,Av,\ldots,A^{n-1}v
$$

linearly independent. Thus $A$ is similar to $C$ exactly when it has the stated [cyclic vector](../../../../../cyclic-vector.md).

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
