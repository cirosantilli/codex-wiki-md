<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The printed point is not on the printed surface, so the requested tangent plane does not exist.** At $(2,-2,9)$, the left side of the defining equation is $x^2y=-8$, whereas the right side is $4ze^{x+y}-11=25$. This is a direct counterexample to the premise that the stated point belongs to the [surface](../../../topological-surface-split.md).

To make the obstruction precise, set $G(x,y,z)=x^2y-4ze^{x+y}+11$. The specified [surface](../../../topological-surface-split.md) is the [level set](../../../level-set.md) $G=0$, but $G(2,-2,9)=-33$. Although $\nabla G(2,-2,9)=(-44,-32,-4)$, the resulting plane $11x+8y+z=15$ is tangent to the different [level set](../../../level-set.md) $G=-33$ through that point. It is not an answer for the printed [surface](../../../topological-surface-split.md). A [tangent plane requires the point to lie on the surface](../../../tangent-plane-requires-the-point-to-lie-on-the-surface.md).

If the intended correction preserves $x=2,y=-2$, the surface equation instead forces $z=3/4$. At the corrected point $p_*=(2,-2,3/4)$,

$$
\nabla G(p_*)=(-11,1,-4).
$$

The corresponding conditional [tangent plane](../../../tangent-plane.md) is

$$
\boxed{11x-y+4z=27\qquad\text{at the corrected point }(2,-2,3/4).}
$$

This conditional calculation identifies a possible repair; it does not silently replace the source's coordinate $9$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
