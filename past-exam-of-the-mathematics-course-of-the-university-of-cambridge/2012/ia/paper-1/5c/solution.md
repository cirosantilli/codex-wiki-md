<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

For a point $\mathbf x$ on the [plane](../../../../../plane.md), the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $|d|=|\mathbf x\cdot\mathbf n|\leq|\mathbf x|$, because $\mathbf n$ is a [unit vector](../../../../../unit-vector.md). Equality is achieved at $\mathbf x=d\mathbf n$. Thus **the distance from the origin is $|d|$**.

Let $\delta=\mathbf p\cdot\mathbf n-d$ and let $\mathbf q=\mathbf p-\delta\mathbf n$ be the perpendicular projection of the [sphere](../../../../../sphere.md)'s center onto the [plane](../../../../../plane.md). Every point of the [plane](../../../../../plane.md) has form $\mathbf x=\mathbf q+\mathbf u$ with $\mathbf u\cdot\mathbf n=0$. The [Pythagorean theorem](../../../../../pythagorean-theorem.md) gives

$$
|\mathbf x-\mathbf p|^2=|\mathbf u-\delta\mathbf n|^2=|\mathbf u|^2+\delta^2.
$$

If $|\delta|=r$, the [sphere](../../../../../sphere.md) equation therefore forces $\mathbf u=0$. **There is exactly one contact point, $\mathbf q$**; it lies on both surfaces.

Write $\tau=\mathbf a\cdot(\mathbf b\times\mathbf c)>0$. The nonzero [scalar triple product](../../../../../scalar-triple-product.md) proves that $\mathbf a,\mathbf b,\mathbf c$ are [linearly independent](../../../../../linear-independence.md), so they form a positively oriented [basis](../../../../../basis.md) of $\mathbb R^3$ and define a nondegenerate [tetrahedron](../../../../../tetrahedron.md).

For the three faces through the origin, choose the inward [unit vectors](../../../../../unit-vector.md)

$$
\mathbf n_a=\frac{\mathbf b\times\mathbf c}{|\mathbf b\times\mathbf c|},\quad
\mathbf n_b=\frac{\mathbf c\times\mathbf a}{|\mathbf c\times\mathbf a|},\quad
\mathbf n_c=\frac{\mathbf a\times\mathbf b}{|\mathbf a\times\mathbf b|}.
$$

Their signs are correct because each has positive [inner product](../../../../../inner-product.md) with the opposite vertex vector. Write the center as $\mathbf p=\alpha\mathbf a+\beta\mathbf b+\gamma\mathbf c$. It lies on the interior side of every face. Tangency of the interior [sphere](../../../../../sphere.md) therefore means signed distance $r$, not $-r$, from each of those three [planes](../../../../../plane.md). Taking [inner products](../../../../../inner-product.md) gives

$$
\alpha\frac{\tau}{|\mathbf b\times\mathbf c|}=r,\quad
\beta\frac{\tau}{|\mathbf c\times\mathbf a|}=r,\quad
\gamma\frac{\tau}{|\mathbf a\times\mathbf b|}=r.
$$

Solving proves **the center formula**

$$
\boxed{\mathbf p=\frac r\tau\left(|\mathbf b\times\mathbf c|\mathbf a+|\mathbf c\times\mathbf a|\mathbf b+|\mathbf a\times\mathbf b|\mathbf c\right).}
$$

This is the [sphere center from three tetrahedron face distances](../../../../../sphere-center-from-three-tetrahedron-face-distances.md); the interior hypothesis selects these signs rather than an exterior center.

Finally set $\mathbf N=\mathbf a\times\mathbf b+\mathbf b\times\mathbf c+\mathbf c\times\mathbf a$. The [scalar triple product](../../../../../scalar-triple-product.md) identities give $\mathbf N\cdot\mathbf a=\mathbf N\cdot\mathbf b=\mathbf N\cdot\mathbf c=\tau$. In particular $\mathbf N\ne0$, and the [plane](../../../../../plane.md) through the three vertices is

$$
\boxed{\Psi:\ \mathbf N\cdot\mathbf x=\tau,\qquad \operatorname{dist}(O,\Psi)=\frac{\tau}{|\mathbf N|}.}
$$

The second formula follows by normalizing $\mathbf N$ to a [unit vector](../../../../../unit-vector.md) and applying the first distance result.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
