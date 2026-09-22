<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

A [bounding volume hierarchy](../../../../../bounding-volume-hierarchy.md) is a [tree](../../../../../tree-graph-theory-split.md) whose leaves contain geometric primitives, here [triangles](../../../../../triangle.md), and whose internal nodes store cheap-to-test [bounding volumes](../../../../../bounding-volume.md) containing all descendant geometry. A [bounding volume](../../../../../bounding-volume.md) may be an [axis-aligned bounding box](../../../../../axis-aligned-bounding-box.md) or a [sphere](../../../../../sphere.md). The key containment guarantee is

$$
\boxed{\text{ray misses a node's bounding volume}\Rightarrow\text{ray misses every triangle below that node}.}
$$

Traverse from the root. Reject a whole subtree when its [bounding volume](../../../../../bounding-volume.md) is missed; otherwise visit its children and perform the full [ray-triangle intersection](../../../../../ray-triangle-intersection.md) test only at surviving leaves. Hitting a [bounding volume](../../../../../bounding-volume.md) is only permission to investigate, not evidence of hitting an enclosed [triangle](../../../../../triangle.md).

For nearest-hit queries, visit the nearer child first and keep the current nearest parameter. A second child whose volume begins farther away than this parameter can be pruned. For a [shadow ray](../../../../../shadow-ray.md), restrict the traversal to the segment before the source and terminate at any blocker.

A flat list of $N$ [triangles](../../../../../triangle.md) needs up to $N$ detailed tests per primary [ray](../../../../../ray-geometry.md) or [shadow ray](../../../../../shadow-ray.md). A well-built [bounding volume hierarchy](../../../../../bounding-volume-hierarchy.md) can reject large groups with a few cheap tests and substantially reduce the average work. A balanced, well-separated scene often gives traversal resembling a short root-to-leaf search, but balance alone does not guarantee logarithmic query time: extensive overlap or an unfortunate [ray](../../../../../ray-geometry.md) can force examination of most or all leaves. Its advantage is spatial rejection, not a universal worst-case bound.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
