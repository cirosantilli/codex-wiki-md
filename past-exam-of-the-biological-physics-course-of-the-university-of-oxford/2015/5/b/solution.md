<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conservation of total [probability](../../../../probability.md) gives $A(t)=1-B(t)$. The two-state [master equation](../../../../master-equation.md) is therefore

$$
\dot B=k_f(1-B)-k_bB=k_f-(k_f+k_b)B,\qquad B(0)=0.
$$

Solving this linear [ordinary differential equation](../../../../ordinary-differential-equation.md) gives

$$
\boxed{B(t)=\frac{k_f}{k_f+k_b}\left(1-e^{-(k_f+k_b)t}\right).}
$$

The middle panel in [d](../../2/d.md) sketches this solution for the explicitly illustrative ratio $k_f/(k_f+k_b)=0.6$. The curve starts at zero with slope $k_f$, is increasing and concave down, and approaches the horizontal limit $B_\infty=k_f/(k_f+k_b)$ on [time constant](../../../../time-constant.md) $(k_f+k_b)^{-1}$. Its initial tangent meets the asymptote at that [time constant](../../../../time-constant.md). The complementary limit is $A_\infty=k_b/(k_f+k_b)$, so $B_\infty/A_\infty=k_f/k_b=e^{-\Delta G_{AB}/(k_BT)}$, the [Boltzmann distribution](../../../../boltzmann-distribution.md) ratio. These are occupancy [probabilities](../../../../probability.md); $B(t)$ is not the cumulative first-passage probability when reverse transitions remain possible.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
