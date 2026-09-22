<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use separate moving [orthonormal bases](../../../../orthonormal-basis.md) in the reference and current [cylindrical coordinate systems](../../../../cylindrical-coordinate-system.md). For [pure torsion of an incompressible cylinder](../../../../pure-torsion-of-an-incompressible-cylinder.md), the [deformation map](../../../../deformation-map.md) is

$$
\mathbf x(R,\Theta,Z)=R\mathbf e_r(\Theta+\tau Z)+Z\mathbf e_z.
$$

The [unit vectors](../../../../unit-vector.md) depend on the angle: $\partial_\theta\mathbf e_r=\mathbf e_\theta$ and $\partial_\theta\mathbf e_\theta=-\mathbf e_r$. Consequently

$$
\partial_R\mathbf x=\mathbf e_r,\qquad
\partial_\Theta\mathbf x=R\mathbf e_\theta,\qquad
\partial_Z\mathbf x=\tau R\mathbf e_\theta+\mathbf e_z.
$$

In particular, the last derivative includes the rotation of $\mathbf e_r$ along the cylinder. The material [gradient](../../../../gradient.md) has the reference coordinate scale factor $1/R$:

$$
\begin{aligned}
\mathbf F
&=(\partial_R\mathbf x)\otimes\mathbf E_R
+\frac1R(\partial_\Theta\mathbf x)\otimes\mathbf E_\Theta
+(\partial_Z\mathbf x)\otimes\mathbf E_Z\\
&=\mathbf e_r\otimes\mathbf E_R
+\mathbf e_\theta\otimes\mathbf E_\Theta
+(\tau r\mathbf e_\theta+\mathbf e_z)\otimes\mathbf E_Z.
\end{aligned}
$$

The [outer products](../../../../outer-product.md) specify the images of the three reference [unit vectors](../../../../unit-vector.md). Thus, with current basis vectors indexing rows and reference basis vectors indexing columns,

$$
\boxed{\mathbf F=\begin{pmatrix}1&0&0\\0&1&\tau r\\0&0&1\end{pmatrix}.}
$$

Its [determinant](../../../../determinant.md) is one, checking [incompressibility](../../../../incompressible-flow.md). The radius is unchanged, so the current outer radius in part (d) is $a=A$. The formula at the coordinate axis is understood by continuity in [Cartesian coordinates](../../../../cartesian-coordinate-system.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
