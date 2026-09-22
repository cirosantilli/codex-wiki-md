<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the centre position as $\mathbf x$ and the bead positions as $\mathbf r_{1,2}=\mathbf x\mp\mathbf R/2$. In the [affine velocity field](../../../../affine-velocity-field.md), $\mathbf u(\mathbf r_{1,2})=\mathbf u(\mathbf x)\mp K\mathbf R/2$. The midpoint follows the flow, so its two slip [velocities](../../../../velocity.md) are

$$
\dot{\mathbf r}_{1,2}-\mathbf u(\mathbf r_{1,2})=\mp\frac12(\dot{\mathbf R}-K\mathbf R).
$$

Each bead loses mechanical power $\zeta$ times its squared slip [speed](../../../../speed.md). Adding the two powers proves the [drag dissipation of a bead-spring pair](../../../../drag-dissipation-of-a-bead-spring-pair.md):

$$
\boxed{D_{\rm pair}=\zeta\left|\frac{\dot{\mathbf R}-K\mathbf R}{2}\right|^2+\zeta\left|\frac{\dot{\mathbf R}-K\mathbf R}{2}\right|^2=\frac\zeta2|\dot{\mathbf R}-K\mathbf R|^2.}
$$

The factor one half comes from two equal-and-opposite bead slips, not from assigning only one bead a drag force.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
