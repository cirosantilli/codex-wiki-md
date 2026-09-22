<h1 id="5a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two displacement [vectors](../../../../../../vector.md) $\mathbf b-\mathbf a$ and $\mathbf c-\mathbf a$ lie in the required [plane](../../../../../../plane.md). Because the three points are non-collinear, their [cross product](../../../../../../cross-product.md)

$$
\mathbf N=(\mathbf b-\mathbf a)\times(\mathbf c-\mathbf a)
$$

is nonzero and is a [normal vector](../../../../../../normal-vector.md) to that plane. A point with position vector $\mathbf r$ lies in the plane exactly when

$$
(\mathbf r-\mathbf a)\cdot\mathbf N=0.
$$

Expanding the [cross product](../../../../../../cross-product.md) gives

$$
\mathbf N=\mathbf a\times\mathbf b+\mathbf b\times\mathbf c+\mathbf c\times\mathbf a.
$$

The terms $\mathbf a\cdot(\mathbf a\times\mathbf b)$ and $\mathbf a\cdot(\mathbf c\times\mathbf a)$ vanish, so the [equation of a plane through three points](../../../../../../equation-of-a-plane-through-three-points.md) becomes

$$
\boxed{\mathbf r\cdot
(\mathbf a\times\mathbf b+\mathbf b\times\mathbf c+\mathbf c\times\mathbf a)
=\mathbf a\cdot(\mathbf b\times\mathbf c).}
$$

Non-collinearity is important: it ensures this is a genuine plane equation with nonzero normal, rather than the vacuous equality $0=0$.

For the specified coordinates,

$$
\mathbf a\times\mathbf b=(-4,0,8),\qquad
\mathbf b\times\mathbf c=(8,0,-4),\qquad
\mathbf c\times\mathbf a=(-1,3,2).
$$

Their sum is $(3,3,6)$, with [Euclidean norm](../../../../../../euclidean-norm.md) $3\sqrt6$. Consequently either orientation of the [unit normal](../../../../../../unit-normal.md) is valid:

$$
\boxed{\mathbf n=\pm\frac{(1,1,2)}{\sqrt6}.}
$$

As a check, the [scalar triple product](../../../../../../scalar-triple-product.md) is $12$, so the plane equation simplifies to $x+y+2z=4$, which all three supplied points satisfy. **The normal direction is $(1,1,2)$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5A](../../5a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
