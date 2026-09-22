<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The sum of the degrees of all [faces](../../../../../../face-of-a-planar-map.md) is $2e$. Each of the $t$ triangular faces contributes three. Because the graph is bridgeless and has no four-cycle, every other face has degree at least five, and therefore

$$
\boxed{2e\ge3t+5(f-t)}.
$$

No edge can border two triangular faces: two distinct triangles sharing that edge would have their other two edges form a four-cycle, while the same triangle on both sides would force the connected bridgeless graph to be that triangle, contrary to $n\ge4$. Thus the $3t$ edge incidences belonging to triangular faces use distinct edges, so

$$
\boxed{e\ge3t}.
$$

Combining the inequalities gives

$$
2e\ge5f-2t\ge5f-\frac{2e}{3},
$$

and hence

$$
\boxed{f\le\frac{8e}{15}}.
$$

The [Euler formula for a connected planar graph](../../../../../../euler-formula-for-a-connected-planar-graph.md) now yields

$$
2=n-e+f
\le n-e+\frac{8e}{15}
=n-\frac{7e}{15},
$$

so the [triangle-pentagon planar edge bound](../../../../../../triangle-pentagon-planar-edge-bound.md) is

$$
\boxed{e\le\frac{15(n-2)}7}.
$$

Equality is possible. Cut each corner of a [dodecahedron](../../../../../../dodecahedron.md) through the midpoints of its incident edges. The resulting [icosidodecahedral graph](../../../../../../icosidodecahedral-graph.md) has

$$
n=30,\qquad e=60,\qquad t=20,\qquad f-t=12,
$$

with every edge incident to one triangular and one pentagonal face. It has no four-cycle, and

$$
60=\frac{15(30-2)}7.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
