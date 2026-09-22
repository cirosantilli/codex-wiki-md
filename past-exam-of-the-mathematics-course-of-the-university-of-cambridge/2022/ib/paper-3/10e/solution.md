<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

Matrices over a [Euclidean domain](../../../../../euclidean-domain.md) are equivalent when $B=PAQ$ for invertible matrices $P,Q$, equivalently when one can pass between them by invertible elementary row and column operations.

For a nonzero matrix, move a nonzero entry to the top left and use Euclidean division and row or column operations to replace it by any nonzero remainder. Repeating terminates with an entry $d_1$ dividing every entry; otherwise adding an offending entry into its row would permit one more strict Euclidean reduction. Clear its row and column, then apply induction to the remaining submatrix. This proves equivalence to a diagonal matrix. It is in [Smith normal form](../../../../../smith-normal-form.md) when, up to units,

$$
d_1\mid d_2\mid\cdots\mid d_r.
$$

Applying these operations over $\mathbb Z$ does not change the isomorphism type of the quotient. If the Smith form of $A$ is $\operatorname{diag}(d_1,\ldots,d_n)$, then

$$
\mathbb Z^n/M\cong\bigoplus_i\mathbb Z/d_i\mathbb Z.
$$

It is finite exactly when every $d_i$ is nonzero, equivalently $\det A\ne0$, and then

$$
\boxed{|\mathbb Z^n/M|=\prod_i|d_i|=|\det A|}.
$$

Both displayed matrices have determinant of absolute value $8$. For $A_1$, the gcds of the entries and of the $2$ by $2$ minors are both $1$, giving Smith invariants

$$
(1,1,8),
\qquad G_1\cong\mathbb Z/8\mathbb Z.
$$

For $A_2$, those gcds are $1$ and $2$, giving

$$
(1,2,4),
\qquad G_2\cong\mathbb Z/2\mathbb Z\oplus\mathbb Z/4\mathbb Z.
$$

The first group has an element of order eight and the second does not, so

$$
\boxed{G_1\not\cong G_2}.
$$

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
