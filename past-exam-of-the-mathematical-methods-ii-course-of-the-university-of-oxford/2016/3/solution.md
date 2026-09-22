<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [implicit differentiation](../../../implicit-differentiation.md) while holding $x$ fixed. Writing $y_z=(\partial y/\partial z)_x$, the constraint gives

$$
2xyy_z+z^2y_z+2yz=0,\qquad y_z=-\frac{2yz}{2xy+z^2}.
$$

The [chain rule](../../../chain-rule.md) applied to $v=xy^3$ now yields

$$
\boxed{\left(\frac{\partial v}{\partial z}\right)_x=3xy^2y_z=-\frac{6xy^3z}{2xy+z^2},\qquad \left(\frac{\partial v}{\partial z}\right)_{x,(1,1,1)}=-2.}
$$

This local formula requires $2xy+z^2\ne0$, as in the [implicit function theorem](../../../implicit-function-theorem.md); that denominator equals $3$ at the specified point.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2016](../../2016-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
