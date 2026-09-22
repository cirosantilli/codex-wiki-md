<h1 id="5a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The chosen [unit normal](../../../../../../unit-normal.md) points toward the plane from the origin, so the plane equation is

$$
\boxed{\mathbf n\cdot\mathbf r=d.}
$$

To locate the circle centre, project $\mathbf p$ onto this [plane](../../../../../../plane.md). Put

$$
\gamma=d-\mathbf n\cdot\mathbf p,\qquad
\mathbf h=\mathbf p+\gamma\mathbf n.
$$

Then $\mathbf n\cdot\mathbf h=d$, so $\mathbf h$ lies in the plane. For any other point $\mathbf r$ of the plane, $\mathbf r-\mathbf h$ is perpendicular to $\mathbf n$. The [Pythagorean theorem](../../../../../../pythagorean-theorem.md) therefore gives

$$
|\mathbf r-\mathbf p|^2
=|\mathbf r-\mathbf h|^2+\gamma^2.
$$

Restricting the sphere equation to the plane consequently gives a circle centred at $\mathbf h$. Thus $\mathbf m=\mathbf h$, proving that the displacement of its centre is purely normal:

$$
\boxed{\mathbf m-\mathbf p=\gamma\mathbf n,\qquad
\gamma=d-\mathbf n\cdot\mathbf p.}
$$

The same [Pythagorean theorem](../../../../../../pythagorean-theorem.md) gives $q^2=\rho^2+\gamma^2$, and hence

$$
\boxed{\gamma^2=q^2-\rho^2,\qquad
\gamma=\pm\sqrt{q^2-\rho^2}.}
$$

**The sign of $\gamma$ is fixed by which side of the plane contains $\mathbf p$; $q$ and $\rho$ alone determine only its magnitude.** Substituting the signed offset yields the [sphere-plane intersection](../../../../../../sphere-plane-intersection.md) radius

$$
\boxed{\rho=\sqrt{q^2-(d-\mathbf n\cdot\mathbf p)^2}.}
$$

A genuine circle requires $|d-\mathbf n\cdot\mathbf p|<q$; equality gives tangency and $\rho=0$, while a larger distance gives no intersection. The [signed distance from a point to a plane](../../../../../../signed-distance-from-a-point-to-a-plane.md) in the direction $\mathbf n$ is $\mathbf n\cdot\mathbf p-d=-\gamma$; the ordinary [distance from a point to a plane](../../../../../../distance-from-a-point-to-a-plane.md) is its absolute value.

## ↑ Ancestors (11)

1. [C](../c.md)
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
