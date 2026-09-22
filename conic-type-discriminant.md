# Conic type discriminant

↑ **Parent:** [Conic section](conic-section.md)

For a second-degree equation $Ax^2+Bxy+Cy^2+Dx+Ey+F=0$, the number $\Delta_2=B^2-4AC$ is the [discriminant of a binary quadratic form](discriminant-of-a-binary-quadratic-form.md) associated with its quadratic part. For a nonempty, nondegenerate real [conic section](conic-section.md), a negative value gives an [ellipse](ellipse.md), zero a [parabola](parabola.md), and a positive value a [hyperbola](hyperbola.md). It is invariant under a [rotation](rotation-mathematics.md) of orthonormal coordinates.[Precalculus 2e, §10.4, Identifying Conics without Rotating Axes and Using the Discriminant to Identify a Conic](precalculus-2e-by-jay-abramson/10-4-rotation-of-axes.md)

A short explanation uses the [symmetric matrix](symmetric-matrix.md)

$$
H=\begin{pmatrix}A&B/2\\B/2&C\end{pmatrix},\qquad \Delta_2=-4\det H.
$$

An [orthogonal matrix](orthogonal-matrix.md) $R$ changes this matrix to $R^{\mathsf T}HR$, whose [determinant](determinant.md) equals $\det H$. The [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md) then removes the mixed term. Equal-sign, opposite-sign and one-zero [eigenvalues](eigenvalue.md) give the three types after the remaining linear terms and offsets are considered.

The qualification matters. The equations $x^2+y^2=0$, $y^2=0$ and $xy=0$ describe a [point](point-geometry.md), a repeated [straight line](straight-line.md), and two crossing [straight lines](straight-line.md), respectively. Their quadratic discriminants have the signs expected of ellipse, parabola and hyperbola types, but all three are [degenerate conics](degenerate-conic.md). Also, $x^2+y^2=-1$ has an [empty set](empty-set.md) of real solutions despite its negative quadratic discriminant.

## ↑ Ancestors (6)

1. [Conic section](conic-section.md)
2. [Euclidean geometry](euclidean-geometry-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Conic section](conic-section.md)
- [Degenerate conic](degenerate-conic.md)
