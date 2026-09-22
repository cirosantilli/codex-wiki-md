# Vertex of a linear polyhedron

↑ **Parent:** [Linear polyhedron](linear-polyhedron.md)

For a [linear polyhedron](linear-polyhedron.md) $P=\{x\in\mathbb R^n:Ax\leq b\}$, a [vertex of a linear polyhedron](vertex-of-a-linear-polyhedron.md) is a [feasible point](feasible-point.md) $p$ at which the normals of the [active constraints](active-constraint.md) span $\mathbb R^n$. Equivalently, $n$ [linearly independent](linear-independence.md) [active constraints](active-constraint.md) uniquely determine $p$. A [linear polyhedron](linear-polyhedron.md) may be unbounded or lower-dimensional; the definition applies in those cases as well as to a [convex polytope](convex-polytope.md).

Such a [point](point-geometry.md) is an [extreme point](extreme-point.md). Indeed, if $p=\lambda u+(1-\lambda)v$ with $u,v\in P$ and $0<\lambda<1$, every [active constraint](active-constraint.md) at $p$ must also be an equality at $u$ and $v$. Selecting $n$ independent active rows forces $u=v=p$. Conversely, if the active normals do not span $\mathbb R^n$, take a nonzero [vector](vector.md) $h$ annihilated by all active rows. The finitely many inactive inequalities have positive slack, so both $p+\varepsilon h$ and $p-\varepsilon h$ remain feasible for sufficiently small $\varepsilon>0$. Their [midpoint](midpoint.md) is $p$, so $p$ is not an [extreme point](extreme-point.md). Thus these notions coincide for a [linear polyhedron](linear-polyhedron.md).

## ↑ Ancestors (6)

1. [Linear polyhedron](linear-polyhedron.md)
2. [Linear programming](linear-programming-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/3/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/2/a/ii/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/2/a/iii/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/2/a/iv/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/2/b/i/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/2/b/iii/solution.md)
- [Vertex of a linear polyhedron](vertex-of-a-linear-polyhedron.md)
