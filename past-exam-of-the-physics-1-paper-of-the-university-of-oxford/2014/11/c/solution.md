<h1 id="11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [fixed-speed orbital launch-direction error](../../../../fixed-speed-orbital-launch-direction-error.md), the initial radius and [speed](../../../../speed.md) are correct, so the specific [orbital energy](../../../../orbital-energy.md) is still $\varepsilon=-GM/(2R)$ and the new [semi-major axis](../../../../semi-major-axis.md) is still $a=R$. Resolve the launch [velocity](../../../../velocity.md) into radial and tangential components, taking $\alpha$ as the in-plane deviation from the intended tangent:

$$
v_r=\sqrt{\frac{GM}{R}}\sin\alpha,\qquad v_\phi=\sqrt{\frac{GM}{R}}\cos\alpha,\qquad j=\sqrt{GMR}\cos\alpha.
$$

For a nondegenerate orbit $\cos\alpha\ne0$, the [orbital eccentricity](../../../../orbital-eccentricity.md) follows from $j^2=GMa(1-e^2)$:

$$
e=|\sin\alpha|,\qquad r_{\min}=R(1-|\sin\alpha|),\qquad r_{\max}=R(1+|\sin\alpha|).
$$

The intended circular orbit has radius $R$ everywhere, so the largest radial distance between the orbit curves occurs at either apsis:

$$
\boxed{\Delta r_{\max}=R|\sin\alpha|\simeq R|\alpha|\quad\text{for small }|\alpha|\text{ in radians}.}
$$

This is the geometric separation of the two orbit curves, not the distance between two satellites compared at equal elapsed times. The latter also depends on orbital phase. A purely radial launch is a degenerate zero-angular-momentum trajectory through the central body and requires separate treatment of the collision.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [11](../../11.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
