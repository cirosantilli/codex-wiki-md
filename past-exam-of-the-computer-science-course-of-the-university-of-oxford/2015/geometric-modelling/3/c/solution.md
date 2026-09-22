<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [boundary representation](../../../../../boundary-representation.md) separates geometry, which supplies locations and supporting [planes](../../../../../plane.md), from topology, which specifies incidence and orientation. A practical [winged-edge data structure](../../../../../winged-edge.md) uses three related record types:

- A [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md) record holds its three [coordinates](../../../../../coordinate-linear-algebra.md) and a reference to one incident edge, sufficient to begin traversing the local fan.
- A face record holds its supporting [plane](../../../../../plane.md), an outward [normal vector](../../../../../normal-vector.md) or equivalent orientation, and a reference to a boundary edge. Faces with holes need one entry per boundary loop.
- An edge record holds its two endpoint [vertices of a polyhedron](../../../../../vertex-of-a-polyhedron.md), its left and right incident faces, and predecessor and successor edges around each of those faces: four “wing” references. “Left” and “right” refer to a chosen orientation of the edge and compatible face traversal conventions.

This explicitly stores adjacency rather than recovering it by searching all faces. A [half-edge data structure](../../../../../doubly-connected-edge-list.md) expresses much the same information with two oppositely directed records per undirected edge: each has an origin [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md), an incident face, its next boundary record and its opposite record; a previous record is often stored as well. The destination can be obtained from the opposite record's origin. This mesh record is distinct from a dangling [half-edge of a graph](../../../../../half-edge-of-a-graph.md).

The compact implementation answer is

$$
\boxed{\text{vertex geometry + oriented face loops + explicit edge/face/vertex incidence}.}
$$

There is deliberate redundancy: the same adjacency can be reached from both an edge and a face, a stored previous edge is recoverable by walking the loop, and a face [normal vector](../../../../../normal-vector.md) can be computed from its ordered noncollinear [vertices of a polyhedron](../../../../../vertex-of-a-polyhedron.md). These copies make neighbourhood queries and local edits cheap, and cached [plane](../../../../../plane.md) equations speed geometric tests. They impose consistency obligations: an edit must update reciprocal references, loops, orientations and affected geometric caches together. A [half-edge data structure](../../../../../doubly-connected-edge-list.md) should share the undirected edge's geometry or keep its paired records synchronized.

## ↑ Ancestors (11)

1. [C](../c.md)
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
