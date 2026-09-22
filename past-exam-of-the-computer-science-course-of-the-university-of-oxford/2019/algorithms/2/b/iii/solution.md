<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [point](../../../../../../point-geometry.md) $(1,4)$ satisfies [dual feasibility](../../../../../../dual-feasibility.md) and supplies an upper bound of $13$ by [weak duality](../../../../../../weak-duality.md). Directly, take one copy of the first constraint and four copies of the second:

$$
2x+3y+4z+9w\leq13.
$$

Since $w\geq0$, the original [objective function](../../../../../../objective-function.md) is at most $13-2w\leq13$. The [feasible point](../../../../../../feasible-point.md) $(2,3,0,0)$ attains $13$. Hence

$$
\boxed{\operatorname{OPT}=13,\qquad (x,y,z,w)=(2,3,0,0)\text{ is optimal}.}
$$

There are also nonvertex optima. In terms of the [slack variables](../../../../../../slack-variable.md), the exact [objective function](../../../../../../objective-function.md) identity is

$$
2x+3y+4z+7w=13-s_1-4s_2-2w.
$$

Equality requires $s_1=s_2=w=0$, leaving the entire [optimal face](../../../../../../optimal-face-of-a-linear-program.md)

$$
(x,y,z,w)=(2-t/2,\,3-t,\,t,\,0),\qquad t\geq0.
$$

Negative $x$ or $y$ on this ray are allowed. This illustrates why the single [vertex of a linear polyhedron](../../../../../../vertex-of-a-linear-polyhedron.md) does not imply a unique optimum.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
