<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the straightforward [incremental three-dimensional convex hull algorithm](../../../../../incremental-three-dimensional-convex-hull-algorithm.md). Assume distinct input [points](../../../../../point-geometry.md), at least four noncoplanar [points](../../../../../point-geometry.md), and general position with no four coplanar. Use exact orientation decisions, or robust predicates that certify the same signs. These assumptions avoid the separate bookkeeping for flat faces, points on the boundary and lower-dimensional initial data.

1. Select four [points](../../../../../point-geometry.md) forming a nondegenerate [tetrahedron](../../../../../tetrahedron.md). Store its four triangular faces with outward [normal vectors](../../../../../normal-vector.md) and consistent adjacency.
1. For the next [point](../../../../../point-geometry.md) $p$, evaluate every current oriented face $f=(a,b,c)$ using$$
   \sigma_f(p)=((b-a)\times(c-a))\cdot(p-a).
   $$

   The current hull lies in $\sigma_f\le0$. Thus a face is visible from $p$ exactly when $\sigma_f(p)>0$.
1. If no face is visible, discard $p$: it lies in the current [convex hull](../../../../../convex-hull.md). Otherwise identify the [horizon of a convex polyhedron](../../../../../horizon-of-a-convex-polyhedron.md) seen from $p$, namely the edges incident with exactly one visible and one retained face.
1. Delete the visible faces and cone the ordered [horizon of a convex polyhedron](../../../../../horizon-of-a-convex-polyhedron.md) to $p$, adding one [triangle](../../../../../triangle.md) per horizon edge. Orient each new face consistently outward and continue with the next [point](../../../../../point-geometry.md).

The [determinant](../../../../../determinant.md) $\sigma_f$ is six times the oriented volume of the [tetrahedron](../../../../../tetrahedron.md) $abcp$; only its sign matters. A zero value needs a declared degeneracy policy if the general-position assumption is relaxed.

The [data structure](../../../../../data-structure-split.md) update is a separate local operation. Mark visible faces and walk their adjacency to collect the horizon cycle before deleting anything. Remove edges with two visible incident faces; retain horizon edges and their retained-face links. Insert a [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md) record for $p$ and a new edge from $p$ to each horizon [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md). Add one face per horizon edge, connect its other two edges to its neighbours in the cone, and replace the deleted face reference on each horizon edge. Restore the cyclic boundary references and each retained [vertex of a polyhedron](../../../../../vertex-of-a-polyhedron.md)'s incident-edge reference; remove any old [vertices of a polyhedron](../../../../../vertex-of-a-polyhedron.md) left without incident faces.

For an outward visible face with boundary edge $a\to b$ on the horizon, the new outward face can be ordered $(a,b,p)$. Its retained neighbour already traverses that edge as $b\to a$. As an independent orientation check, an interior [point](../../../../../point-geometry.md) of the old hull must evaluate negatively against the new face.

The correctness step is geometric: the nonvisible part of a [convex polyhedron](../../../../../convex-polyhedron.md) remains supporting, while sight lines from $p$ to the horizon create precisely the new supporting faces. Replacing the visible cap by its cone therefore gives

$$
\boxed{H_{i+1}=\operatorname{conv}(H_i\cup\{p\}).}
$$

Induction from the initial [tetrahedron](../../../../../tetrahedron.md) yields the [convex hull](../../../../../convex-hull.md) of all input [points](../../../../../point-geometry.md).

## ↑ Ancestors (11)

1. [E](../e.md)
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
