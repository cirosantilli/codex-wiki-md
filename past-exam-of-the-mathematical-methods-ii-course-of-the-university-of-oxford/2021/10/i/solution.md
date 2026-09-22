<h1 id="10/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathbf F=(F_x,F_y,F_z)$ be continuously differentiable near $P$. Take a small axis-aligned rectangular volume around $P$, with side lengths $\Delta x,\Delta y,\Delta z$ shrinking with bounded aspect ratios. The outward [flux](../../../../flux.md) through its two $x$ faces is, to leading order,

$$
\bigl[F_x(x+\Delta x/2,y,z)-F_x(x-\Delta x/2,y,z)\bigr]\Delta y\Delta z
=\frac{\partial F_x}{\partial x}(P)\,\Delta x\Delta y\Delta z+o(\Delta V),
$$

where $\Delta V=\Delta x\Delta y\Delta z$. The analogous face pairs give $\partial F_y/\partial y$ and $\partial F_z/\partial z$. Dividing total [flux](../../../../flux.md) by $\Delta V$ and taking the limit gives

$$
\boxed{\nabla\cdot\mathbf F=\frac{\partial F_x}{\partial x}+\frac{\partial F_y}{\partial y}+\frac{\partial F_z}{\partial z}.}
$$

The [divergence](../../../../divergence.md) is thus the local outward [flux](../../../../flux.md) per unit volume; the symbols on the right are Cartesian [partial derivatives](../../../../partial-derivative.md).

For a bounded volume $V$ with piecewise smooth closed boundary $S$, subdivide into small cells. Each internal face occurs twice with opposite [normal vectors](../../../../normal-vector.md), so its [flux](../../../../flux.md) cancels. The remaining sum is the exterior [surface integral](../../../../surface-integral.md); the cell sums of $(\nabla\cdot\mathbf F)\Delta V$ converge to the [volume integral](../../../../volume-integral.md). Assuming continuous first [partial derivatives](../../../../partial-derivative.md) on a neighborhood of the closure of $V$, this proves the [divergence theorem](../../../../divergence-theorem.md):

$$
\boxed{\oiint_S\mathbf F\cdot\mathbf n\,dS=\iiint_V\nabla\cdot\mathbf F\,dV.}
$$

The unit [normal vector](../../../../normal-vector.md) $\mathbf n$ points out of $V$. Multiple boundary components are allowed; at a cavity wall it points into the cavity.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [10](../../10.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
