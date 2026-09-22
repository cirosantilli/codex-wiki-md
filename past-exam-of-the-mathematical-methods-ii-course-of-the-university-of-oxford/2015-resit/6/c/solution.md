<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The enclosed volume lies above $z=0$ and below $z=4-x^2-y^2$. In [cylindrical coordinates](../../../../cylindrical-coordinate-system.md), its limits are $0\le r\le2$, $0\le\theta\le2\pi$, $0\le z\le4-r^2$, with volume element $r\,dz\,dr\,d\theta$. The [divergence theorem](../../../../divergence-theorem.md) gives

$$
\oiint\mathbf F\cdot d\mathbf S=2\int_0^{2\pi}\int_0^2\int_0^{4-r^2}r\,dz\,dr\,d\theta=4\pi\int_0^2(4r-r^3)\,dr.
$$

Thus the volume is $8\pi$, and the outward [flux](../../../../flux.md) is $\boxed{16\pi}$.

A direct check separates the boundary into its cap and base. On the base, $\mathbf F\cdot(-\hat{\mathbf z})=0$. On the graph $z=4-x^2-y^2$, the upward vector area element is $(2x,2y,1)\,dx\,dy$, so the cap flux is $\iint_{x^2+y^2\le4}2(x^2+y^2)\,dx\,dy=16\pi$, in agreement with the volume calculation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
