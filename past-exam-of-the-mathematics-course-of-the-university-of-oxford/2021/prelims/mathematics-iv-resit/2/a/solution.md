<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First find the fixed [axis of rotation](../../../../../../axis-of-rotation.md) by solving $(M-I)\mathbf n=0$. After removing a nonzero common factor, the [linear equations](../../../../../../linear-equation.md) are

$$
-2n_1+n_2-3n_3=0,\qquad -3n_1-2n_2-n_3=0,\qquad n_1+3n_2-2n_3=0.
$$

They give $n_2=n_3=-n_1$. Choose the following [unit vectors](../../../../../../unit-vector.md):

$$
\mathbf p_1=\frac1{\sqrt3}(1,-1,-1)^T,\quad \mathbf p_2=\frac1{\sqrt2}(1,1,0)^T,\quad \mathbf p_3=\mathbf p_1\times\mathbf p_2=\frac1{\sqrt6}(1,-1,2)^T.
$$

Their [dot products](../../../../../../dot-product.md) show that they form an [orthonormal basis](../../../../../../orthonormal-basis.md); hence $P=(\mathbf p_1\ \mathbf p_2\ \mathbf p_3)$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md). Since $M$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md) fixing $\mathbf p_1$, it preserves the [orthogonal complement](../../../../../../orthogonal-complement.md) of $\mathbf p_1$. Its restriction there has [determinant](../../../../../../determinant.md) $1$, so it is a [planar rotation](../../../../../../planar-rotation.md).

The [trace](../../../../../../matrix-trace.md) gives $1+2\cos\theta=\operatorname{tr}M=9/7$, so $\cos\theta=1/7$. To determine the sign of the [sine](../../../../../../sine.md), rather than just its magnitude, calculate

$$
M\mathbf p_2=\frac1{7\sqrt2}(5,-3,8)^T,\qquad \mathbf p_3^TM\mathbf p_2=\frac{24}{7\sqrt{12}}=\frac{4\sqrt3}{7}>0.
$$

Thus a suitable [angle](../../../../../../angle.md) and [change of basis](../../../../../../change-of-basis.md) are

$$
\boxed{\theta=\arccos(1/7),\qquad P=\begin{pmatrix}1/\sqrt3&1/\sqrt2&1/\sqrt6\\-1/\sqrt3&1/\sqrt2&-1/\sqrt6\\-1/\sqrt3&0&2/\sqrt6\end{pmatrix}.}
$$

In fact direct [matrix multiplication](../../../../../../matrix-multiplication.md) gives

$$
P^TMP=\begin{pmatrix}1&0&0\\0&1/7&-4\sqrt3/7\\0&4\sqrt3/7&1/7\end{pmatrix}=\operatorname{diag}(1,R_\theta).
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
