<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the first [orthonormal basis](../../../../../../orthonormal-basis.md) [vector](../../../../../../vector.md) to be $\mathbf e_1=\mathbf a$. If $\mathbf b$ is not parallel to $\mathbf a$, choose $\mathbf e_2$ along $\mathbf b-(\mathbf a\cdot\mathbf b)\mathbf a$; otherwise choose any [unit vector](../../../../../../unit-vector.md) [orthogonal](../../../../../../orthogonal-vectors.md) to $\mathbf a$. Complete to an [orthonormal basis](../../../../../../orthonormal-basis.md) with $\mathbf e_3$. The [matrix](../../../../../../matrix.md) with rows $\mathbf e_i^T$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md), and expressing the three [unit vectors](../../../../../../unit-vector.md) in this [basis](../../../../../../basis.md) gives

$$
\mathbf a'=(1,0,0)^T,\qquad \mathbf b'=(x,y,0)^T,\qquad
\mathbf c'=(z,w\cos\theta,w\sin\theta)^T.
$$

The last two components of $\mathbf c'$ have [polar coordinates](../../../../../../polar-coordinates.md) of the displayed form; we may choose $w\geq0$. If they vanish, $\theta$ is arbitrary.

An [orthogonal transformation](../../../../../../orthogonal-transformation.md) preserves [dot products](../../../../../../dot-product.md). Taking [dot products](../../../../../../dot-product.md) with $\mathbf a'$, and then using the unit [Euclidean norms](../../../../../../euclidean-norm.md), gives

$$
\boxed{x=\cos\gamma,\qquad z=\cos\beta,\qquad |y|=\sin\gamma,\qquad |w|=\sin\beta.}
$$

The remaining [dot product](../../../../../../dot-product.md) gives

$$
\cos\alpha=xz+yw\cos\theta.
$$

An [orthogonal matrix](../../../../../../orthogonal-matrix.md) has [determinant](../../../../../../determinant.md) $\pm1$, so it preserves the absolute [scalar triple product](../../../../../../scalar-triple-product.md). In the new [coordinates](../../../../../../coordinate-linear-algebra.md) this [scalar triple product](../../../../../../scalar-triple-product.md) is $yw\sin\theta$. Consequently

$$
\begin{aligned}
| (\mathbf a\wedge\mathbf b)\cdot\mathbf c|^2
&=y^2w^2-(yw\cos\theta)^2\\
&=(1-x^2)(1-z^2)-(\cos\alpha-xz)^2\\
&=1-\cos^2\alpha-\cos^2\beta-\cos^2\gamma
+2\cos\alpha\cos\beta\cos\gamma.
\end{aligned}
$$

Taking the nonnegative [square root](../../../../../../square-root.md) proves

$$
\boxed{|(\mathbf a\wedge\mathbf b)\cdot\mathbf c|
=\sqrt{1-(\mathbf a\cdot\mathbf b)^2-(\mathbf b\cdot\mathbf c)^2-(\mathbf c\cdot\mathbf a)^2+2(\mathbf a\cdot\mathbf b)(\mathbf b\cdot\mathbf c)(\mathbf c\cdot\mathbf a)}.}
$$

No division by $y$ or $w$ was used, so the proof includes parallel [vectors](../../../../../../vector.md). Equivalently, the expression under the [square root](../../../../../../square-root.md) is the [Gram determinant](../../../../../../gram-determinant.md) of the three [unit vectors](../../../../../../unit-vector.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
