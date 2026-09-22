<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Segre embedding](../../../../segre-embedding.md) is

$$
\boxed{\sigma_{n,m}([x_0:\cdots:x_n],[y_0:\cdots:y_m])=[x_iy_j]_{0\leq i\leq n,\ 0\leq j\leq m}.}
$$

Rescaling the two representatives multiplies every target coordinate by the same scalar, and at least one [product](../../../../product-of-numbers.md) is nonzero, so the map is well defined. In affine source charts its coordinate ratios are regular [products](../../../../product-of-numbers.md), so it is a [morphism](../../../../morphism-of-algebraic-varieties.md).

Arrange target coordinates into a [matrix](../../../../matrix.md) $Z=(z_{ij})$. Every [image](../../../../image-of-a-function.md) [matrix](../../../../matrix.md) has [rank](../../../../rank-one-quadratic-form.md) one and satisfies all homogeneous equations

$$
z_{ij}z_{k\ell}-z_{i\ell}z_{kj}=0.
$$

Conversely, a nonzero [matrix](../../../../matrix.md) satisfying these equations has [rank](../../../../rank-one-quadratic-form.md) one. Choose $z_{i_0j_0}\neq0$ and [set](../../../../set-split.md) $x_i=z_{ij_0}$, $y_j=z_{i_0j}/z_{i_0j_0}$. The [minors](../../../../minor-linear-algebra.md) imply $z_{ij}=x_iy_j$. Therefore

$$
\boxed{\operatorname{im}\sigma_{n,m}=V(\text{all }2\times2\text{ minors}),}
$$

a [projective variety](../../../../projective-variety.md). The two projective factors are uniquely recoverable from a nonzero column and row. This also shows [injectivity](../../../../injective-function.md) and supplies the local inverse formulas used in the next part.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebraic Geometry course of the University of Oxford](../../../split.md)
5. [Algebraic Geometry course of the University of Oxford](../../../../algebraic-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
