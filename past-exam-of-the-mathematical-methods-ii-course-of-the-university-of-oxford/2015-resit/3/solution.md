<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work on a domain with $x\ne0$, and suppose $f$ is differentiable at $u=y/x$. The multivariable [chain rule](../../../chain-rule.md) gives

$$
\frac{\partial w}{\partial x}=f'(u)\frac{\partial u}{\partial x}=-\frac{y}{x^2}f'(u),\qquad\frac{\partial w}{\partial y}=f'(u)\frac{\partial u}{\partial y}=\frac1x f'(u).
$$

Multiplying the first equation by $x$ and the second by $y$ cancels their common terms:

$$
\boxed{x\frac{\partial w}{\partial x}+y\frac{\partial w}{\partial y}=0}.
$$

The geometry is that $y/x$ stays fixed along a radial dilation $(x,y)\mapsto(\lambda x,\lambda y)$. Thus $w$ is constant along each admissible radial ray, and the differential operator $x\partial_x+y\partial_y$ differentiates along that ray. This is the degree-zero case of [Euler homogeneous function theorem](../../../euler-theorem-for-homogeneous-functions.md). The displayed quotient does not define a function at $x=0$ without additional extension data.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
