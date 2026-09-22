<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a continuously differentiable [vector field](../../../vector-field.md) on a volume $V$ with piecewise smooth boundary $S$, the [divergence theorem](../../../divergence-theorem.md) states

$$
\oiint_S\mathbf A\cdot\hat{\mathbf n}\,dS=\iiint_V\nabla\cdot\mathbf A\,dV,
$$

where $\hat{\mathbf n}$ is the **outward** unit normal. For the polynomial field here,

$$
\nabla\cdot\mathbf A=\partial_x(4xz)+\partial_y(-y^2)+\partial_z(yz)=4z-y.
$$

Therefore the outward [flux](../../../flux.md) through the unit cube is

$$
I=\int_0^1\int_0^1\int_0^1(4z-y)\,dx\,dy\,dz=2-\frac12=\boxed{\frac32}.
$$

As a direct boundary check, the $x=1$ face contributes $2$, the $y=1$ face contributes $-1$, and the $z=1$ face contributes $1/2$. All three opposite faces contribute zero, reproducing the result and fixing the orientation sign.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2015](../../2015-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
