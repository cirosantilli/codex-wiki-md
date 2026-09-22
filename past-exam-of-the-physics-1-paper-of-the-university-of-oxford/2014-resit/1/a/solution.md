<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the square to have uniform [surface mass density](../../../../projected-surface-mass-density.md) $\sigma=M/a^2$, and put its centre at $x=y=0$. For an in-plane axis through the centre parallel to a side, direct [integration](../../../../integral-split.md) gives

$$
I_x=\frac M{a^2}\int_{-a/2}^{a/2}\int_{-a/2}^{a/2}y^2\,dx\,dy=\frac{Ma^2}{12}.
$$

The same holds for $I_y$, and the mixed [integral](../../../../integral-split.md) $\int xy\,dm$ vanishes by reflection symmetry. The squared perpendicular distance to an axis making angle $\psi$ with the $x$ axis is $(-x\sin\psi+y\cos\psi)^2$. Its [integral](../../../../integral-split.md) therefore gives

$$
I_\psi=\frac{Ma^2}{12}(\sin^2\psi+\cos^2\psi)=\frac{Ma^2}{12}.
$$

Thus a diagonal through opposite corners and its perpendicular **through the centre** have

$$
\boxed{I_{\rm diagonal}=I_{\rm central\ perpendicular}=\frac{Ma^2}{12}.}
$$

This is the [in-plane inertia isotropy of a square plate](../../../../in-plane-inertia-isotropy-of-a-square-plate.md).

**Axis-location qualification:** perpendicularity fixes a direction, not a line's position. If the second axis is instead shifted by distance $d$ from the centre, the [parallel axis theorem](../../../../parallel-axis-theorem.md) gives $I_2=Ma^2/12+Md^2$. A perpendicular through a corner on that diagonal has $d=a/\sqrt2$ and hence $I_2=7Ma^2/12$, a concrete different value satisfying the stated directional description. If “through the corners” means an edge rather than a diagonal, that edge has $I=Ma^2/3$; two adjacent edges both have that value. The general displaced-axis formula and these choices make the location convention explicit rather than silently assigning a unique value to an unspecified second axis.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2014 resit](../../../2014-resit-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
