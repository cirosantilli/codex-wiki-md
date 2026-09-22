<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We construct both the required [triangulation](../../../../../triangulation.md) and its [polygonal schema](../../../../../polygonal-schema.md). Subdivide the [square](../../../../../square.md) $Q=[0,1]^2$ into a $4\times4$ grid. Insert the centre of each small square and join it by [line segments](../../../../../line-segment.md) to its four corners, making four triangles per small square. Identify opposite sides of $Q$ by translations: $(0,t)\sim(1,t)$ and $(t,0)\sim(t,1)$. This is the standard [quotient space](../../../../../quotient-topological-space.md) presentation of the [torus](../../../../../torus.md).

The grid and centre vertices, with these identifications, define an abstract [simplicial complex](../../../../../simplicial-complex.md) $K_1$. Every triangle contains its own small-square centre and two consecutive grid vertices, so no triangle has identified vertices and no distinct triangles acquire the same vertex set. Only intended common sides or vertices are shared. Thus this is a genuine finite [triangulation](../../../../../triangulation.md), whose [geometric realization](../../../../../geometric-realization-of-a-simplicial-complex.md) is [homeomorphic](../../../../../homeomorphism.md) to $T^2$. There are $32$ vertices, $96$ edges and $64$ triangles, giving [Euler characteristic](../../../../../euler-characteristic.md) zero.

Choose the [simplex](../../../../../simplex.md) $\tau$ represented in the interior of $Q$ by the triangle with vertices

$$
(1/4,1/4),\qquad(1/2,1/4),\qquad(3/8,3/8).
$$

Remove its [relative interior](../../../../../relative-interior.md). Before identifying the square's sides, the remainder is a [closed disc](../../../../../closed-disc.md) with a triangular hole, hence an [annulus](../../../../../annulus-mathematics.md). Cut this [annulus](../../../../../annulus-mathematics.md) along the [line segment](../../../../../line-segment.md) from $(0,0)$ to $(1/4,1/4)$, treating the two banks as distinct boundary arcs. The cut space is a [closed disc](../../../../../closed-disc.md); traversing its boundary follows the four outer edges, one bank, the three inner edges, and the other bank. It therefore has nine marked boundary sides.

A [homeomorphism](../../../../../homeomorphism.md) from this cut disc to a convex nine-sided [polygon](../../../../../polygon.md) can be chosen to carry its nine marked sides to the nine polygon sides. One justification is to choose a boundary [homeomorphism](../../../../../homeomorphism.md) with the prescribed marked vertices and extend it over the disc by radial extension after disc parametrizations. Transport the identifications to this [convex polygon](../../../../../convex-polygon.md). With labels recording traversal direction, its boundary word is

$$
\boxed{a\,b\,a^{-1}\,b^{-1}\,c\,d\,e\,f\,c^{-1}}.
$$

Identify equally labelled sides in their arrow directions: the two $a$ sides and two $b$ sides restore the torus pairings, while the two $c$ sides undo the cut. Leave $d,e,f$ unpaired. Their union is the triangular boundary of the removed [simplex](../../../../../simplex.md). The resulting [quotient space](../../../../../quotient-topological-space.md) is exactly

$$
X=|K_1|\setminus\operatorname{inside}(\tau).
$$

This is the [polygonal presentation of a punctured surface](../../../../../polygonal-presentation-of-a-punctured-surface.md). The word supplies all nine sides and every gluing; inverse exponents reverse the boundary traversal direction.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
