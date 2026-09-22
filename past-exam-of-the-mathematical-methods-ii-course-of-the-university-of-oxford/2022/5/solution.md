<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose the normal pointing away from the origin, equivalently the outward normal of the first-octant tetrahedron. Parametrize the face by $\mathbf r=(x,y,2-x/2-y/2)$ on $D=\{x,y\ge0:x+y\le4\}$. Its oriented area element is

$$
\mathbf r_x\times\mathbf r_y\,dx\,dy=(1/2,1/2,1)\,dx\,dy.
$$

Thus the [surface integral](../../../surface-integral.md) is

$$
\iint_D\left(-\frac x2+\frac y2+2-\frac x2-\frac y2\right)dx\,dy
=\int_0^4(2-x)(4-x)\,dx
=\boxed{\frac{16}{3}}.
$$

The [divergence theorem](../../../divergence-theorem.md) checks this result: $\nabla\cdot\mathbf F=1$, the tetrahedron's [volume](../../../volume.md) is $4\cdot4\cdot2/6=16/3$, and each coordinate-plane face has zero [flux](../../../flux.md). The opposite orientation gives $-16/3$; a signed [flux](../../../flux.md) requires an orientation.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2022](../../2022-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
