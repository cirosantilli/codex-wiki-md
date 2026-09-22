<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The [matrix rank](../../../../../matrix-rank.md) $r$ is the [dimension](../../../../../dimension-vector-space.md) of its [column space](../../../../../column-space.md), equivalently the dimension of the image of the corresponding [linear map](../../../../../linear-map.md). The equation is solvable precisely when $\mathbf b\in\operatorname{col}A$, equivalently when the augmented matrix has the same rank as $A$. If $\mathbf x_0$ is one solution, every solution is $\mathbf x_0+\mathbf u$ with $\mathbf u\in\ker A$, since subtracting any two solutions gives a kernel element. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives $\dim\ker A=3-r$.

Consequently, for rank three there is one solution for every $\mathbf b$, namely $A^{-1}\mathbf b$. For rank two there are no solutions outside the column plane, and an [affine solution space of a linear equation](../../../../../affine-solution-space-of-a-linear-equation.md) of dimension one when consistent. For rank one, consistency requires $\mathbf b$ to lie on the column line and the solution set is an affine plane of dimension two. For rank zero, $A=0$: the solution set is all of $\mathbb R^3$ if $\mathbf b=0$, and empty otherwise. These descriptions include homogeneous systems, whose solution spaces pass through the origin.

The [sphere](../../../../../sphere.md) has normal $\nabla(x_1^2+x_2^2+x_3^2)=(0,2,2)$ at the specified point, so its [tangent plane](../../../../../tangent-plane.md) is

$$
\boxed{x_2+x_3=2.}
$$

A general [straight line](../../../../../straight-line.md) through the origin is $\mathbf x=t\mathbf d$, $t\in\mathbb R$, for a fixed nonzero direction $\mathbf d=(d_1,d_2,d_3)$. To express the intersection using a $3\times3$ [matrix](../../../../../matrix.md), choose independent [vectors](../../../../../vector.md) $\mathbf u,\mathbf v$ spanning $\mathbf d^\perp$. The line is exactly the intersection of $\mathbf u\cdot\mathbf x=0$ and $\mathbf v\cdot\mathbf x=0$, hence

$$
\boxed{\begin{pmatrix}u_1&u_2&u_3\\v_1&v_2&v_3\\0&1&1\end{pmatrix}\mathbf x=\begin{pmatrix}0\\0\\2\end{pmatrix}.}
$$

The first two rows have rank two. The third is independent of them exactly when $(0,1,1)\cdot\mathbf d=d_2+d_3\ne0$. In that case the rank is three and the unique intersection is

$$
\boxed{\mathbf x=\frac{2\mathbf d}{d_2+d_3}.}
$$

Geometrically the line crosses the tangent plane transversely. If $d_2+d_3=0$, the matrix rank is two: its third row is a linear combination of the first two, but the corresponding right-hand-side combination would be zero rather than two. The system is inconsistent and **there is no intersection**. The line is parallel to the tangent plane and cannot lie in it, since it contains the origin while the plane does not. Thus no choice of a genuine direction produces an infinite intersection in this particular problem.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
