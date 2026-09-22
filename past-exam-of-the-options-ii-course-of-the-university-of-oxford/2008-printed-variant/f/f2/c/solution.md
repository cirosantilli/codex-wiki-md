<h1 id="f/f2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Lagrange multiplier](../../../../../lagrange-multiplier.md) condition says that at a constrained local extremum of a continuously differentiable objective on a regular surface $h=0$, its [gradient](../../../../../gradient.md) is normal to the tangent plane: $\nabla f=\lambda\nabla h$ for some scalar multiplier.

First the box must be centred at zero. If the two face coordinates in one direction are $u_i,v_i$, subtracting the [ellipsoid](../../../../../ellipsoid.md) equations for two vertices differing only in that coordinate gives $u_i^2=v_i^2$. A nondegenerate box has $u_i\ne v_i$, hence $u_i=-v_i$. Its positive half-sides $x,y,z$ therefore satisfy $x^2/a^2+y^2/b^2+z^2/c^2=1$ and its volume is $8xyz$.

The feasible closed octant is [compact](../../../../../compact-space.md), the boundary gives zero volume, and some interior box has positive volume, so the maximum is interior. Apply multipliers to $\log(xyz)$ there:

$$
1/x=2\lambda x/a^2,\quad1/y=2\lambda y/b^2,\quad1/z=2\lambda z/c^2.
$$

Thus the three squared scaled coordinates are equal and sum to one. The unique positive solution gives

$$
\boxed{\text{side lengths }2a/\sqrt3,\ 2b/\sqrt3,\ 2c/\sqrt3;\qquad V_{\max}=\frac{8abc}{3\sqrt3}}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2008 printed variant](../../../../2008-printed-variant-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
