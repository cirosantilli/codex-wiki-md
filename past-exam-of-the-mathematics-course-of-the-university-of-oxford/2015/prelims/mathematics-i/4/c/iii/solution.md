<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**$A$ is not an [orthogonal matrix](../../../../../../../orthogonal-matrix.md).** Its first column has squared [Euclidean norm](../../../../../../../euclidean-norm.md)

$$
(-\sqrt2)^2+0^2+(3/\sqrt2)^2=\frac{13}{2}\ne1,
$$

so $A^TA\ne I$. The reason this is compatible with [ii](../ii.md) is that $1,x,x^2$ is not an [orthonormal basis](../../../../../../../orthonormal-basis.md) for the given [inner product](../../../../../../../inner-product-split.md). Its [Gram matrix](../../../../../../../gram-matrix.md) is

$$
G=\begin{pmatrix}1&0&2/3\\0&2/3&0\\2/3&0&2/3\end{pmatrix},\qquad
\langle u,v\rangle=[u]^TG[v].
$$

The correct condition on this [matrix representation of a linear map](../../../../../../../matrix-representation-of-a-linear-map.md) is

$$
\boxed{A^TGA=G,}
$$

which follows either by direct multiplication or by the [inner product](../../../../../../../inner-product-split.md) preservation just proved. This is the rule for an [orthogonal transformation in a nonorthonormal basis](../../../../../../../orthogonal-transformation-in-a-nonorthonormal-basis.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
