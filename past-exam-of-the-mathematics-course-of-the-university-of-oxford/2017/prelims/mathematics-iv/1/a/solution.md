<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

For [vectors](../../../../../../vector.md) $\mathbf a,\mathbf b,\mathbf c\in\mathbb R^3$, the [scalar product](../../../../../../dot-product.md), [cross product](../../../../../../cross-product.md) and [scalar triple product](../../../../../../scalar-triple-product.md) are respectively

$$
\begin{aligned}
\mathbf a\cdot\mathbf b&=a_1b_1+a_2b_2+a_3b_3,\\
\mathbf a\wedge\mathbf b&=(a_2b_3-a_3b_2,\ a_3b_1-a_1b_3,\ a_1b_2-a_2b_1),\\
(\mathbf a\wedge\mathbf b)\cdot\mathbf c&=\det\begin{pmatrix}a_1&a_2&a_3\\b_1&b_2&b_3\\c_1&c_2&c_3\end{pmatrix}.
\end{aligned}
$$

Expanding the [dot product](../../../../../../dot-product.md) gives

$$
(\mathbf a\wedge\mathbf b)\cdot\mathbf a
=a_1a_2b_3-a_1a_3b_2+a_2a_3b_1-a_1a_2b_3+a_1a_3b_2-a_2a_3b_1=0.
$$

Interchanging $\mathbf a$ and $\mathbf b$ changes the sign of their [cross product](../../../../../../cross-product.md), so its [dot product](../../../../../../dot-product.md) with $\mathbf b$ is also zero. Thus the [cross product](../../../../../../cross-product.md) is [orthogonal](../../../../../../orthogonal-vectors.md) to both [vectors](../../../../../../vector.md), including when it is the [zero vector](../../../../../../zero-vector.md).

The displayed [scalar triple product](../../../../../../scalar-triple-product.md) is a [determinant](../../../../../../determinant.md). A square [matrix](../../../../../../matrix.md) has nonzero [determinant](../../../../../../determinant.md) exactly when its rows are [linearly independent](../../../../../../linear-independence.md). Hence

$$
\boxed{(\mathbf a\wedge\mathbf b)\cdot\mathbf c\ne0\iff\mathbf a,\mathbf b,\mathbf c\text{ are linearly independent}.}
$$

## ↑ Ancestors (12)

1. [a](../a.md)
2. [1](../../1.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
