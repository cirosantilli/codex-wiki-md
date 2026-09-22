<h1 id="section-b/6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Farther than a few [edge](../../../../../edge-of-a-graph.md) lengths from the root, replace the radial coordinate $r$ by a physical coordinate $x=ar$ and smooth the [master equation](../../../../../master-equation.md). It has the same constant-coefficient [Fokker-Planck equation](../../../../../fokker-planck-equation.md) as in (b). Under the conventional first-time-derivative truncation,

$$
D_0=\frac{a^2}{2\tau},\qquad
\boxed{C=\frac{a(2-z)}{z\tau}<0\quad\text{for }z>2.}
$$

The radial drift $v=-C=a(z-2)/(z\tau)$ is outward. For $z=2$ the tree is the infinite line, its radial distance is an unbiased reflected walk, and $C=0$.

The root cannot absorb [probability](../../../../../probability.md) or allow negative radial distance. Write the equation as a [continuity equation](../../../../../continuity-equation.md), using the [Fokker-Planck probability current](../../../../../fokker-planck-probability-current.md)

$$
\partial_tP=-\partial_xj,\qquad j=-D\partial_xP-CP.
$$

The appropriate continuum [boundary condition](../../../../../boundary-condition.md) is reflecting, or zero flux:

$$
\boxed{j(0,t)=0\quad\Longleftrightarrow\quad D\partial_xP(0,t)+CP(0,t)=0.}
$$

It is not generally $\partial_xP(0,t)=0$: that simpler condition is correct only when $C=0$. With the finite-bias fixed-step Gaussian convention from (b), use $D=D_{\rm fixed}=2a^2(z-1)/(z^2\tau)$ instead; the drift sign and zero-current [boundary condition](../../../../../boundary-condition.md) are unchanged. A continuum [boundary condition](../../../../../boundary-condition.md) represents the microscopic root region after coarse-graining, rather than reproducing each discrete root [probability](../../../../../probability.md) at individual step times.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
