# Incremental three-dimensional convex hull algorithm

↑ **Parent:** [Convex hull](convex-hull.md)

Start from a nondegenerate [tetrahedron](tetrahedron.md) and insert remaining [points](point-geometry.md) one at a time. Discard a [point](point-geometry.md) inside the current [convex polyhedron](convex-polyhedron.md); otherwise replace faces visible from it by the cone from that [point](point-geometry.md) to the [horizon of a convex polyhedron](horizon-of-a-convex-polyhedron.md). Scanning every current face gives $O(n^2)$ worst-case [time complexity](time-complexity.md) and $O(n)$ current-hull storage in three dimensions. Coplanar input requires a separate degeneracy policy.

## ↑ Ancestors (6)

1. [Convex hull](convex-hull.md)
2. [Convex set](convex-set-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Geometric Modelling examination paper by the University of Oxford (2015)](geometric-modelling-examination-paper-by-the-university-of-oxford-2015.md)
- [Horizon of a convex polyhedron](horizon-of-a-convex-polyhedron.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/geometric-modelling/3/e/solution.md)
