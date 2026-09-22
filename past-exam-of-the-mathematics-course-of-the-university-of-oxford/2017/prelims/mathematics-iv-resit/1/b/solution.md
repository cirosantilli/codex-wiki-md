<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A real square [matrix](../../../../../../matrix.md) $A$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md) when

$$
\boxed{A^TA=I.}
$$

Here $A^T$ is the [transpose](../../../../../../transpose.md) and $I$ the [identity matrix](../../../../../../identity-matrix.md); equivalently, its columns form an [orthonormal basis](../../../../../../orthonormal-basis.md). If this holds, the squared [Euclidean norm](../../../../../../euclidean-norm.md) obeys

$$
|A\mathbf v|^2=\mathbf v^TA^TA\mathbf v=\mathbf v^T\mathbf v=|\mathbf v|^2,
$$

so the [linear transformation](../../../../../../linear-map.md) preserves length.

Conversely, suppose $|A\mathbf v|=|\mathbf v|$ for every [vector](../../../../../../vector.md) $\mathbf v$. Put $B=A^TA-I$, a [symmetric matrix](../../../../../../symmetric-matrix.md). Then $\mathbf v^TB\mathbf v=0$ for every [vector](../../../../../../vector.md). Taking $\mathbf v=\mathbf e_i$, the standard [basis vectors](../../../../../../basis-vector.md), gives $B_{ii}=0$. Taking $\mathbf v=\mathbf e_i+\mathbf e_j$ for $i\ne j$ gives $2B_{ij}=0$. Thus $B=0$, proving that **the [linear transformation](../../../../../../linear-map.md) preserves length if and only if $A$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md).**

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
