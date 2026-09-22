<h1 id="b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

About a specified axis, the [moment of inertia](../../../../moment-of-inertia.md) is $I=\int r_\perp^2\,dm$, giving [rotational kinetic energy](../../../../rotational-kinetic-energy.md) $I\omega^2/2$ for fixed-axis rotation. With square coordinates centred on the plate,

$$
I_x=\frac{M}{l^2}\int_{-l/2}^{l/2}\int_{-l/2}^{l/2}y^2\,dx\,dy
=\boxed{\frac{Ml^2}{12}}.
$$

The [in-plane inertia isotropy of a square plate](../../../../in-plane-inertia-isotropy-of-a-square-plate.md) follows using the [perpendicular axis theorem](../../../../perpendicular-axis-theorem.md), which gives $I_z=I_x+I_y=Ml^2/6$. For any in-plane central axis at angle $\phi$, the perpendicular in-plane axis has the same inertia by the square's $90^\circ$ rotational symmetry. Their sum is $I_z$, so **every such in-plane axis has $I=Ml^2/12$**.

The [parallel axis theorem](../../../../parallel-axis-theorem.md) gives hinge inertia $I_H=Ml^2/3$. During the short [impulse](../../../../impulse.md) [gravity](../../../../gravity.md) is negligible, and the hinge [impulse](../../../../impulse.md) has no moment about the hinge. Therefore

$$
I_H\omega=K(l/2+a),\qquad
\boxed{v=\frac{\omega l}{2}=\frac{3K}{4M}\left(1+\frac{2a}{l}\right).}
$$

The [hinge impulse of an edge-pivoted square plate](../../../../hinge-impulse-of-an-edge-pivoted-square-plate.md) follows from [linear momentum](../../../../momentum-split.md): $J_H=Mv-K$. Taking its positive direction to be that of the applied [impulse](../../../../impulse.md),

$$
\boxed{J_H=K\left(\frac{3a}{2l}-\frac14\right),\qquad
N=|J_H|.}
$$

Generally $K$ alone does not supply the centre-of-mass [momentum](../../../../momentum-split.md) compatible with rotation about the fixed hinge, so the hinge supplies the difference. Its [impulse](../../../../impulse.md) vanishes at the [centre of percussion](../../../../centre-of-percussion.md),

$$
\boxed{a=l/6.}
$$

## ↑ Ancestors (12)

1. [B9](../b9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
