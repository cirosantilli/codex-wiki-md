# Reduced column echelon form

↑ **Parent:** [Elementary column operation](elementary-column-operation.md)

The reduced column echelon form of a [matrix](matrix.md) $A$ is defined by taking its [transpose](transpose.md), forming the [reduced row echelon form](reduced-row-echelon-form.md), and transposing back:

$$
\operatorname{rcef}(A)=\bigl(\operatorname{rref}(A^T)\bigr)^T.
$$

It is obtained from $A$ by [elementary column operations](elementary-column-operation.md). Its nonzero columns precede its zero columns, the topmost nonzero entry of each nonzero column is $1$, these leading entries move strictly downward as the column number increases, and each leading entry is the only nonzero entry in its row.

Every [elementary column operation](elementary-column-operation.md) preserves the [column space](column-space.md), because it and its inverse express each new column as a [linear combination](linear-combination.md) of the old columns. Thus the nonzero columns of the reduced form give a [basis](basis.md) of the original [column space](column-space.md). In contrast, [elementary row operations](elementary-row-operation.md) preserve the [row space](row-space.md). There is no general identity $\operatorname{rcef}(A)=\operatorname{rref}(A)^T$: the definition requires reducing $A^T$, not $A$.

For an [invertible matrix](invertible-matrix.md) of size $n$, both reduced forms are $I_n$. A singular example showing the distinction is

$$
A=\begin{pmatrix}1&2\\0&0\end{pmatrix},\qquad
\operatorname{rref}(A)=\begin{pmatrix}1&2\\0&0\end{pmatrix},\qquad
\operatorname{rcef}(A)=\begin{pmatrix}1&0\\0&0\end{pmatrix}.
$$

## ↑ Ancestors (9)

1. [Elementary column operation](elementary-column-operation.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/2/c/ii/c/solution.md)
