<h1 id="12g/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Suppose an open hyperbolic disc centred at $X$ is contained in a [hyperbolic triangle](../../../../../../hyperbolic-triangle.md). Move $X$ to zero by an [isometry](../../../../../../isometry.md). Extend the radial geodesics from zero through the three vertices to ideal points $P_1,P_2,P_3$. Because zero lies inside the original triangle, the three vertex directions are not contained in a semicircle. The [ideal hyperbolic triangle](../../../../../../ideal-triangle.md) with those endpoints therefore contains zero: otherwise a separating geodesic through zero would put all three endpoints in one semicircle. It also contains each finite vertex, which lies on the segment from zero to the corresponding ideal endpoint. Geodesic convexity then makes it contain the original triangle.

The three angular gaps between successive ideal endpoints sum to $2\pi$, and each is at most $\pi$. One has size at least $2\pi/3$, so its half-angle $\alpha$ is at least $\pi/3$. The distance in part (iii) decreases as $\alpha$ increases. Thus the corresponding side of the ideal triangle is at distance at most

$$
2\operatorname{artanh}\!\left(\frac{1-\sin(\pi/3)}{\cos(\pi/3)}\right)=2\operatorname{artanh}(2-\sqrt3)=\frac12\log3
$$

from zero. If the disc radius exceeds this distance, it contains a point on that side and points beyond it, and cannot be contained in the ideal triangle, hence cannot be contained in the original one. This proves the [hyperbolic triangle inradius bound](../../../../../../hyperbolic-triangle-inradius-bound.md):

$$
\boxed{a>2\operatorname{artanh}(2-\sqrt3)\ \Longrightarrow\ \text{no hyperbolic triangle contains an open disc of radius }a.}
$$

The symmetric ideal triangle has equality, explaining the constant. Finite triangles have strictly smaller inradius.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [12G](../../12g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
