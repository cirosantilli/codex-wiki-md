<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At the first step of [Gaussian elimination](../../../../../../gaussian-elimination.md), the first column of a nonsingular [matrix](../../../../../../matrix.md) cannot be zero. Choose a nonzero pivot there using a row interchange and eliminate below it. The resulting [matrix](../../../../../../matrix.md) has block form

$$
\begin{pmatrix}p&r\\0&B\end{pmatrix},\qquad p\ne0.
$$

Elementary elimination and row [permutations](../../../../../../permutation.md) preserve nonsingularity, so $p\det B\ne0$ and the trailing [matrix](../../../../../../matrix.md) $B$ is nonsingular. Its first column again has a nonzero entry. Repeating this argument inductively provides a nonzero pivot at every step and produces an upper-triangular factor. The recorded elimination multipliers, with previous entries permuted when necessary, form the unit lower-triangular factor. **Every nonsingular square [matrix](../../../../../../matrix.md) admits $PA=LU$ under [columnwise partial pivoting](../../../../../../columnwise-partial-pivoting.md).**

For the column-interchange convention from part (a), use the same induction with a nonzero entry in the first row of each nonsingular trailing [matrix](../../../../../../matrix.md). Column interchanges put it in the pivot position, and elimination gives $AQ=LU$. These existence statements are in exact arithmetic; they do not assert that all choices have equally good numerical stability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
