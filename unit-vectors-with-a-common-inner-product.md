# Unit vectors with a common inner product

↑ **Parent:** [Gram matrix](gram-matrix.md)

For $n\geq2$, the [Gram matrix](gram-matrix.md) of $n$ unit [vectors](vector.md) with common distinct-pair [inner product](inner-product.md) $t$ is $G=(1-t)I+t\mathbf1\mathbf1^T$. Its [eigenvalues](eigenvalue.md) are $1+(n-1)t$ on the all-ones direction and $1-t$ on its orthogonal complement. It is a [positive-definite symmetric matrix](symmetric-positive-definite-matrix.md) exactly when $-1/(n-1)<t<1$, permitting a linearly independent realization in $\mathbb R^n$. An explicit construction takes the columns of

$$
B=\sqrt{1-t}(I-uu^T)+\sqrt{1+(n-1)t}\,uu^T,
\qquad u=\mathbf1/\sqrt n.
$$

The two orthogonal projections have product zero, so $B^TB=G$; positive [eigenvalues](eigenvalue.md) also make $B$ invertible. At either endpoint the corresponding eigenspace becomes a linear dependence.

## ↑ Ancestors (7)

1. [Gram matrix](gram-matrix.md)
2. [Inner product](inner-product.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/8c/iii/solution.md)
