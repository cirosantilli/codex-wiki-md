# Rank-one matrix update

↑ **Parent:** [Linear algebra](linear-algebra-split.md)

A [rank-one matrix update](rank-one-matrix-update.md) changes a [matrix](matrix.md) $A$ by an [outer product](outer-product.md) $uv^T$. For real [vectors](vector.md) $u,v\in\mathbb R^n$, its action on an input [vector](vector.md) $x$ is

$$
(A+uv^T)x=Ax+u(v^Tx).
$$

The [dot product](dot-product.md) $v^Tx$ reads one [scalar](scalar.md) from the input, and the correction moves the output along $u$. All correction outputs therefore lie in one [linear span](linear-span.md). If either [vector](vector.md) is zero, the update is zero; otherwise the correction is a [rank-one matrix](rank-one-matrix.md). The full updated [matrix](matrix.md) need not have rank one.

For example, choose

$$
u=\begin{pmatrix}1\\2\end{pmatrix},\qquad
v=\begin{pmatrix}3\\-1\end{pmatrix},\qquad
uv^T=\begin{pmatrix}3&-1\\6&-2\end{pmatrix}.
$$

The update sends $x=(x_1,x_2)^T$ to the correction $(3x_1-x_2)(1,2)^T$. Although all four entries change, there is only one direction of correction. Adding it to the [identity matrix](identity-matrix.md) gives $B=\begin{pmatrix}4&-1\\6&-1\end{pmatrix}$.

This special structure allows existing work to be reused. The [matrix determinant lemma](matrix-determinant-lemma.md) updates the [determinant](determinant.md) using one [scalar](scalar.md), and the [Sherman–Morrison formula](sherman-morrison-formula.md) updates the [matrix inverse](matrix-inverse.md) using an [outer product](outer-product.md). Such formulas are useful when a [linear system](system-of-linear-equations.md) changes slightly after a new observation or a parameter adjustment: the unchanged part can retain its [LU decomposition](lu-decomposition.md). The term rank-one describes the rank of the _correction_, not the size of the entry changes. [Gilbert Strang, MIT 18.065, Lecture 14: Low Rank Changes in A and Its Inverse](https://ocw.mit.edu/courses/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/988b4c05680f40a5a4b3be7004a32500_XhSk_Lw2X_U.pdf).

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Matrix determinant lemma](matrix-determinant-lemma.md)
- [Rank-one matrix update](rank-one-matrix-update.md)
- [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)
- [Sherman–Morrison formula](sherman-morrison-formula.md)
