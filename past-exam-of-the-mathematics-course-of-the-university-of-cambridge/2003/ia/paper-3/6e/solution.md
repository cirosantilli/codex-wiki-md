<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

Write the row components as $E_{ai}=(e_a)_i$. Expanding the [cross product](../../../../../cross-product.md) in components,

$$
(e_1\times e_2)\cdot e_3=\epsilon_{ijk}(e_1)_i(e_2)_j(e_3)_k
$$

equals the alternating six-term expansion of the [determinant](../../../../../determinant.md) of $E$. Therefore **$(e_1\times e_2)\cdot e_3=\det E$**.

Geometrically, $|e_1\times e_2|$ is the area of the parallelogram spanned by $e_1,e_2$, and its direction is perpendicular to that plane. A nonzero [scalar triple product](../../../../../scalar-triple-product.md) means both that this area is nonzero and that $e_3$ has a nonzero component normal to the plane. Thus the vectors are [linearly independent](../../../../../linear-independence.md) and form a [basis](../../../../../basis.md) of $\mathbb R^3$, without needing to be orthogonal. Equivalently, their parallelepiped has nonzero volume.

The entries of $E\hat E^T$ are $e_a\cdot\hat e_b$, so the required duality is exactly $E\hat E^T=I$. Since $E$ is invertible, this has the unique solution

$$
\boxed{\hat E^T=E^{-1},\qquad \hat E=E^{-T}}.
$$

Its [determinant](../../../../../determinant.md) is $1/\det E\ne0$, so its rows are again a [basis](../../../../../basis.md). Put $\Delta=(e_1\times e_2)\cdot e_3$. The [cross product](../../../../../cross-product.md) $e_2\times e_3$ is perpendicular to $e_2,e_3$, and its [dot product](../../../../../dot-product.md) with $e_1$ is $\Delta$. Consequently the [reciprocal basis](../../../../../reciprocal-basis.md) is

$$
\boxed{\hat e_1=\frac{e_2\times e_3}{\Delta},\qquad \hat e_2=\frac{e_3\times e_1}{\Delta},\qquad \hat e_3=\frac{e_1\times e_2}{\Delta}}.
$$

These vectors have precisely the required [dot products](../../../../../dot-product.md), so uniqueness identifies them with the rows of $E^{-T}$.

For the final request, an [orthonormal basis](../../../../../orthonormal-basis.md) of rows gives $EE^T=I$. If instead the reciprocal rows are [orthonormal](../../../../../orthonormal-set.md), then $\hat E\hat E^T=I$ and substitution of $\hat E=E^{-T}$ gives $E^{-T}E^{-1}=I$, again implying $EE^T=I$. Thus in either case **$E$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md)** and $\hat E=E$.

The further printed claim that $E$ must be a [rotation matrix](../../../../../rotation-matrix.md) is false without an orientation assumption. The [matrix](../../../../../matrix.md) $E=\operatorname{diag}(1,1,-1)$ has orthonormal rows and is its own [reciprocal basis](../../../../../reciprocal-basis.md) [matrix](../../../../../matrix.md), but $\det E=-1$: it is a [reflection](../../../../../reflection-mathematics.md). By the [orientation of an orthonormal reciprocal basis](../../../../../orientation-of-an-orthonormal-reciprocal-basis.md), the corrected conclusion is

$$
\boxed{E\in O(3),\qquad E\text{ is a rotation matrix if and only if }\det E=+1.}
$$

A right-handed original ordered [basis](../../../../../basis.md) supplies exactly this missing condition.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
