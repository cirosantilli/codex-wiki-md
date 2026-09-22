<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

The [row rank](../../../../../row-rank.md) of $A$ is the dimension of the span of its rows in $\mathbb R^n$; its [column rank](../../../../../column-rank.md) is the dimension of the span of its columns in $\mathbb R^m$. [Elementary row operations](../../../../../elementary-row-operation.md) replace rows by invertible [linear combinations](../../../../../linear-combination.md), so preserve their span. They also preserve every column relation: $Ac=0$ if and only if $EAc=0$ for an invertible [elementary matrix](../../../../../elementary-matrix.md) $E$. Reduce $A$ to [row echelon form](../../../../../row-echelon-form.md) $R$, with $r$ nonzero rows. These rows are independent because their leading entries occur in distinct, successively later columns. The $r$ pivot columns are independent by their triangular pivot submatrix, while every column lies in the $r$-dimensional coordinate space supported on the nonzero rows. Thus both ranks of $R$, and hence both ranks of $A$, equal $r$. **[Row rank](../../../../../row-rank.md) equals [column rank](../../../../../column-rank.md).**

[Elementary column operations](../../../../../elementary-column-operation.md) replace columns by invertible [linear combinations](../../../../../linear-combination.md) and preserve their span. Equivalently, right multiplication by an invertible [elementary matrix](../../../../../elementary-matrix.md) $F$ preserves row relations, since $c^TAF=0$ if and only if $c^TA=0$. Therefore either [elementary row operations](../../../../../elementary-row-operation.md) or [elementary column operations](../../../../../elementary-column-operation.md) preserve the [matrix rank](../../../../../matrix-rank.md), and any finite sequence gives $\boxed{\operatorname{rank}(A')=\operatorname{rank}(A)}$.

For the block [matrices](../../../../../matrix.md), put $M=\begin{pmatrix}PQ&0\\Q&QR\end{pmatrix}$. The explicit invertible multiplications

$$
\begin{pmatrix}I&-P\\0&I\end{pmatrix}M\begin{pmatrix}I&-R\\0&I\end{pmatrix}=\begin{pmatrix}0&-PQR\\Q&0\end{pmatrix}
$$

follow by first subtracting $P$ times the lower block row from the upper one and then subtracting the first block column times $R$ from the second. Changing the sign of the upper block row gives $N=\begin{pmatrix}0&PQR\\Q&0\end{pmatrix}$. These operations preserve [matrix rank](../../../../../matrix-rank.md), proving that the two specified block [matrices](../../../../../matrix.md) have equal rank. Their off-diagonal form gives $\operatorname{rank}(N)=\operatorname{rank}(Q)+\operatorname{rank}(PQR)$, since the two image components occupy independent coordinate blocks.

Choose $r_1=\operatorname{rank}(PQ)$ independent columns of $PQ$ and $r_2=\operatorname{rank}(QR)$ independent columns of $QR$. Select the corresponding $r_1$ columns from the first block column of $M$ and $r_2$ from the second. In a [linear relation](../../../../../linear-relation.md) among these selected columns, the upper coordinate block forces every coefficient of the first selection to vanish; the lower block then forces every coefficient of the second to vanish. Consequently $\operatorname{rank}(M)\geq r_1+r_2$. Combining this with the equality of block ranks proves the [Frobenius rank inequality](../../../../../frobenius-rank-inequality.md):

$$
\boxed{\operatorname{rank}(PQ)+\operatorname{rank}(QR)\leq\operatorname{rank}(Q)+\operatorname{rank}(PQR).}
$$

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
