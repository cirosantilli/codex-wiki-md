# Cartesian basis

↑ **Parent:** [Linear algebra](linear-algebra-split.md)

A [Cartesian basis](cartesian-basis.md) is an [ordered basis](ordered-basis.md) of [unit vectors](unit-vector.md) along the mutually perpendicular axes of a [Cartesian coordinate system](cartesian-coordinate-system.md). It is an [orthonormal basis](orthonormal-basis.md) of a real [Euclidean space](euclidean-norm.md): $e_i\cdot e_j=\delta_{ij}$, with $\delta_{ij}$ the [Kronecker delta](kronecker-delta.md). In the plane, the familiar [standard basis](standard-basis.md) is $e_1=(1,0)^T$, $e_2=(0,1)^T$; the [vector](vector.md) $p=(2,1)^T$ is $2e_1+e_2$. A rotated pair of perpendicular [unit vectors](unit-vector.md) is also a [Cartesian basis](cartesian-basis.md), even though its [basis vectors](basis-vector.md) have different [standard basis](standard-basis.md) entries.

The advantage is that [coordinates](coordinate-linear-algebra.md) can be measured separately by [dot products](dot-product.md), and the squared [norm](norm.md) is the sum of their squares:

$$
p=\sum_i(p\cdot e_i)e_i,\qquad [p]_{\mathcal E}=(p\cdot e_1,\ldots,p\cdot e_n)^T,\qquad \|p\|^2=\sum_i(p\cdot e_i)^2.
$$

These are the real [Euclidean space](euclidean-norm.md) instances of the [orthonormal basis](orthonormal-basis.md) expansion.[§6B, Definition 6.27, printed p. 199, and Theorem 6.30(a–b), printed p. 200](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

An [orthogonal basis](orthogonal-basis.md) only requires perpendicular [basis vectors](basis-vector.md); their lengths need not be one. For example, $(2,0)^T,(0,3)^T$ are [orthogonal](orthogonal-vectors.md), but $p=(2,1)^T$ has [coordinates](coordinate-linear-algebra.md) $(1,1/3)^T$, while its [dot products](dot-product.md) with them are $4,3$. For an [orthogonal basis](orthogonal-basis.md) $(a_i)$, the [coordinate](coordinate-linear-algebra.md) along $a_i$ is $(p\cdot a_i)/(a_i\cdot a_i)$. Dividing each nonzero [basis vector](basis-vector.md) by its [norm](norm.md) makes it a [unit vector](unit-vector.md) without changing its direction. Unit length alone does not imply [orthogonality](orthogonal-vectors.md): $(1,0)^T$ and $(1,1)^T/\sqrt2$ are both [unit vectors](unit-vector.md) but have [dot product](dot-product.md) $1/\sqrt2$.

The examples below show why these distinctions matter: rotating a [Cartesian basis](cartesian-basis.md) changes the [coordinate vector](coordinate-vector.md) while keeping lengths easy to compute; using nonperpendicular [basis vectors](basis-vector.md) still gives unique [coordinates](coordinate-linear-algebra.md), but requires the [dual basis](dual-basis.md) or a [matrix inverse](matrix-inverse-split.md) to extract them.

**Table of contents**

- [Cartesian basis under rotation](cartesian-basis-under-rotation.md)
- [Cartesian and oblique coordinate reconstruction](cartesian-and-oblique-coordinate-reconstruction.md)
- [Cartesian frame](cartesian-frame.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Active planar rotation](active-planar-rotation.md)
- [Cartesian basis](cartesian-basis.md)
- [Cartesian basis under rotation](cartesian-basis-under-rotation.md)
- [Cartesian frame](cartesian-frame.md)
- [Change of basis](change-of-basis.md)
- [Dot product](dot-product.md)
- [Householder reflection sending a vector to a coordinate axis](householder-reflection-sending-a-vector-to-a-coordinate-axis.md)
- [Noncommuting rotations about fixed axes](noncommuting-rotations-about-fixed-axes.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4/11c/i/solution.md)
- [Rotation matrix](rotation-matrix.md)
