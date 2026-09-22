<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Only $z,w$ have printed nonnegativity restrictions; $x,y$ are unrestricted. In four-dimensional space, a [vertex of a linear polyhedron](../../../../../../vertex-of-a-linear-polyhedron.md) needs four independent [active constraints](../../../../../../active-constraint.md). There are exactly four available constraints, so all must be active. Solving them gives

$$
z=w=0,\qquad y=3,\qquad 2x-y=1,
$$

and therefore the only possible [vertex of a linear polyhedron](../../../../../../vertex-of-a-linear-polyhedron.md) is **$(x,y,z,w)=(2,3,0,0)$**. It is feasible, and its four active normals are independent, so it is indeed a [vertex of a linear polyhedron](../../../../../../vertex-of-a-linear-polyhedron.md).

One can also see uniqueness geometrically from the [slack variables](../../../../../../slack-variable.md) $s_1=1-2x+y-5w$ and $s_2=3-y-z-w$. The [feasible region](../../../../../../feasible-region.md) is in affine bijection with the [nonnegative orthant](../../../../../../nonnegative-orthant.md) in $(s_1,s_2,z,w)$:

$$
y=3-s_2-z-w,\qquad x=2-\tfrac12s_1-\tfrac12s_2-\tfrac12z-3w.
$$

That [orthant](../../../../../../orthant.md) has only the origin as an [extreme point](../../../../../../extreme-point.md), giving the same unique [vertex of a linear polyhedron](../../../../../../vertex-of-a-linear-polyhedron.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Algorithms](../../../../algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
