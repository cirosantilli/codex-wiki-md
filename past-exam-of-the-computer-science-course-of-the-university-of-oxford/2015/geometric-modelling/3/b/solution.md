<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an ordinary closed manifold [boundary representation](../../../../../boundary-representation.md), three requirements are:

- **Valid embedded faces.** Each face is planar and bounded by simple closed edge loops with nonzero area; distinct face interiors do not cross, and faces meet only in their declared common edges or [vertices of a polyhedron](../../../../../vertex-of-a-polyhedron.md). A quadrilateral with four noncoplanar [vertices of a polyhedron](../../../../../vertex-of-a-polyhedron.md) is not one planar face; a bow-tie loop does not bound a simple face. Holes, when allowed, need separate correctly oriented loops.
- **Closed manifold incidence.** Exactly two faces meet at each edge, and the incident faces around each [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md) form one cyclic fan. A single missing face leaves edges incident with only one face. Three faces sharing an edge, or two closed shells touching only at one [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md), violate the local surface condition. The second example shows why the edge count alone is insufficient.
- **Consistent orientation.** Adjacent oriented faces traverse their common edge in opposite directions, giving compatible outward [normal vectors](../../../../../normal-vector.md). Reversing just one face of a [tetrahedron](../../../../../tetrahedron.md) breaks this condition. For a cavity, the material's outward [normal vector](../../../../../normal-vector.md) points into the cavity, so shell orientation must also respect which region is solid.

Together these support the answer

$$
\boxed{\text{embedded planar faces; closed manifold incidence; consistent outward orientation}.}
$$

For a connected orientable closed boundary of genus $g$, the [Euler characteristic](../../../../../euler-characteristic.md) provides an additional check, $V-E+F=2-2g$, when faces are disk-like. The familiar value $2$ applies to a sphere-like shell; it must not be imposed blindly on every [polyhedron](../../../../../polyhedron.md). Correct counts alone do not exclude intersections or invalid local incidence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
