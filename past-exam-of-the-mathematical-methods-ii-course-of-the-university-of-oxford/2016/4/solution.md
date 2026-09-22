<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [divergence theorem](../../../divergence-theorem.md) includes every part of the closed boundary, including the two vertical cut faces. Its volume integrand simplifies because the terms linear in $x$ cancel:

$$
\nabla\cdot\mathbf F=3x^2+(3y^2+2x)-2x=3(x^2+y^2).
$$

In [cylindrical coordinates](../../../cylindrical-coordinate-system.md), the remaining [integration region](../../../domain-of-integration.md) is $0\leq r\leq1$, $0\leq z\leq1-r^2$, $\pi/2\leq\theta\leq2\pi$. With the [Jacobian determinant](../../../jacobian-determinant.md) $r$, the outward [flux](../../../flux.md) is

$$
\boxed{\int_{\partial V}\mathbf F\cdot d\mathbf S=\int_{\pi/2}^{2\pi}\int_0^1\int_0^{1-r^2}3r^3\,dz\,dr\,d\theta=\frac{9\pi}{2}\left(\frac14-\frac16\right)=\frac{3\pi}{8}.}
$$

The angular range is three quarters of a full revolution. The volume calculation already accounts for the base and cut faces, so no additional surface terms should be appended.

## ↑ Ancestors (11)

1. [4](../4.md)
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
