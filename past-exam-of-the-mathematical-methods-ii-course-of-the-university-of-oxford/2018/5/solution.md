<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $D=y(3y-2)$. [Implicit differentiation](../../../implicit-differentiation.md) of the two constraints gives the [linear system](../../../system-of-linear-equations.md)

$$
D y'-2zz'=-2x,\qquad aD y'+2zz'=-2.
$$

Adding them, then substituting back, gives at regular points

$$
\boxed{\frac{dy}{dx}=-\frac{2(x+1)}{(1+a)y(3y-2)},\qquad
\frac{dz}{dx}=\frac{ax-1}{(1+a)z}.}
$$

The relevant [Jacobian determinant](../../../jacobian-determinant.md) is $2(1+a)yz(3y-2)$. Thus the special parameter value is $\boxed{a=-1}$, assuming the other factors are nonzero. At that parameter, adding the original constraints gives $(x+1)^2=0$: the [intersection curve](../../../intersection-curve.md) lies wholly in the [plane](../../../plane.md) $x=-1$ and cannot be parametrized by $x$ on an interval. Calling its derivatives “infinite” describes a vertical [projection](../../../projection-linear-algebra.md), not a finite-valued differentiable pair $y(x),z(x)$ at $a=-1$; the displayed ratios then have simultaneous zero numerators on the intersection and are undefined.

There are also point-dependent failures when $y=0$, $y=2/3$ or $z=0$. These can produce vertical [tangents](../../../tangent.md) or require a different local parameter, and simultaneous numerator zeros need separate analysis. The [implicit function theorem](../../../implicit-function-theorem.md) guarantees finite $y',z'$ only where the stated [Jacobian determinant](../../../jacobian-determinant.md) is nonzero. This distinction is the geometry of a [singular projection of an implicit curve](../../../singular-projection-of-an-implicit-curve.md).

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2018](../../2018-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
