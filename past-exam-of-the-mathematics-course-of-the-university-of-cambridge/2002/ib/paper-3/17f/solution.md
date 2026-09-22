<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

Over a commutative field, define the [determinant](../../../../../determinant.md) by the signed permutation sum

$$
\boxed{\det A=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_{i=1}^n a_{i,\sigma(i)}}.
$$

It is linear in each row separately. Swapping two rows reindexes the permutations by a transposition and reverses the sign; thus a [matrix](../../../../../matrix.md) with two equal rows has [determinant](../../../../../determinant.md) zero. Adding $c$ times row $i$ to a different row $j$ consequently gives

$$
\det A'=\det A+c\det(\text{matrix with row }j\text{ replaced by row }i)=\det A.
$$

These are immediate consequences of the definition, not assumptions about elementary row operations.

For the block upper-triangular [matrix](../../../../../matrix.md), a nonzero permutation term must assign every bottom row to one of the last $n$ columns, because its first $n$ entries are zero. Those rows use all the last columns; the top rows must use all the first columns. The sign and products factor into two independent $n$-permutations, giving

$$
\boxed{\det\begin{pmatrix}A&B\\0&C\end{pmatrix}=\det A\det C}.
$$

In particular $X_0=\begin{pmatrix}B&I\\0&A\end{pmatrix}$ has [determinant](../../../../../determinant.md) $\det B\det A$. For each bottom row $n+i$, subtract $a_{ij}$ times top row $j$ for $j=1,\ldots,n$. The top rows remain unchanged, so these additions produce

$$
X_1=\begin{pmatrix}B&I\\-AB&0\end{pmatrix}
$$

without changing the [determinant](../../../../../determinant.md). Exchange its first and last blocks of $n$ columns; the permutation has sign $(-1)^{n^2}$ and gives $\begin{pmatrix}I&B\\0&-AB\end{pmatrix}$. Hence

$$
(-1)^{n^2}\det X_1=\det(-AB)=(-1)^n\det(AB).
$$

Since $n^2$ and $n$ have the same parity, $\det X_1=\det(AB)$. Combining the two evaluations proves

$$
\boxed{\det(AB)=\det A\det B}.
$$

No invertibility of $A$ or $B$ was used, so the proof includes singular [matrices](../../../../../matrix.md).

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
