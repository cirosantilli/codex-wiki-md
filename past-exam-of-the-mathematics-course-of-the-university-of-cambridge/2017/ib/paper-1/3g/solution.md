<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

In the curvature $-1$ normalization, the [hyperbolic triangle area](../../../../../hyperbolic-triangle-area.md) is its angle defect:

$$
\boxed{\operatorname{area}(T)=\pi-\alpha-\beta-\gamma}.
$$

Join one vertex of a convex geodesic polygon to its nonadjacent vertices. This gives $n-2$ [hyperbolic triangles](../../../../../hyperbolic-triangle.md) with disjoint interiors. Their angles at every polygon vertex sum to that vertex's interior angle. Adding the [hyperbolic triangle areas](../../../../../hyperbolic-triangle-area.md) therefore gives the [hyperbolic polygon area](../../../../../hyperbolic-polygon-area.md)

$$
\boxed{A=(n-2)\pi-\sum_{j=1}^n\alpha_j}.
$$

For a [regular hyperbolic polygon with prescribed area](../../../../../regular-hyperbolic-polygon-with-prescribed-area.md), place $n$ equally spaced vertices on a [hyperbolic circle](../../../../../hyperbolic-circle.md) of radius $R>0$ and join consecutive vertices by [geodesics](../../../../../geodesic.md). Rotations through $2\pi/n$ and reflections in radial lines show that this is a convex regular polygon. The triangle from its centre to a vertex and the midpoint of an adjacent side is right angled, with angles $\pi/n$, $\alpha(R)/2$, and $\pi/2$, and hypotenuse $R$. The angle form of the [hyperbolic law of cosines](../../../../../hyperbolic-law-of-cosines.md) gives

$$
\cosh R=\cot(\pi/n)\cot(\alpha(R)/2),\qquad \alpha(R)=2\arctan\!\left(\frac{\cot(\pi/n)}{\cosh R}\right).
$$

Consequently $A(R)=(n-2)\pi-n\alpha(R)$ is continuous and strictly increasing. As $R\downarrow0$, $\alpha(R)\to\pi-2\pi/n$, so $A(R)\to0$; as $R\to\infty$, $\alpha(R)\to0$, so $A(R)\to(n-2)\pi$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) proves existence for every permitted $A$. Indeed the required radius is

$$
\boxed{R=\operatorname{arcosh}\!\left[\frac{\cot(\pi/n)}{\tan(((n-2)\pi-A)/(2n))}\right]}.
$$

The argument also proves uniqueness of the radius in this construction; neither endpoint area is attained by a nondegenerate finite-radius polygon.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
