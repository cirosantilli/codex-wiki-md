<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Let $D$ be the disk $x^2+y^2\le3$. The upper boundary is the graph $z=3-x^2-y^2$, with outward vector [vector surface element](../../../vector-area-element.md) $(2x,2y,1)\,dx\,dy$. Thus its [flux](../../../flux.md) is

$$
\iint_D(2x^2+2y^2)\,dx\,dy
=\int_0^{2\pi}\int_0^{\sqrt3}2r^3\,dr\,d\theta=9\pi.
$$

The lower disk has outward [normal vector](../../../normal-vector.md) $-\mathbf e_z$ and zero [flux](../../../flux.md), since $F_z=0$. The total outward [surface integral](../../../surface-integral.md) is therefore $9\pi$.

Independently, $\nabla\cdot\mathbf F=2$ and the enclosed [volume](../../../volume.md) is

$$
V=\int_0^{2\pi}\int_0^{\sqrt3}(3-r^2)r\,dr\,d\theta=\frac{9\pi}{2}.
$$

Consequently $\iiint_V\nabla\cdot\mathbf F\,dV=2V=\boxed{9\pi}$, agreeing with the [divergence theorem](../../../divergence-theorem.md). Both the orientation of the cap and inclusion of the closing disk have been accounted for.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2016 resit](../../2016-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
