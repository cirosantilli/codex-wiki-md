<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [free-draining approximation](../../../../free-draining-approximation.md): neglect the [hydrodynamic interaction](../../../../hydrodynamic-interaction.md) between the widely separated spheres and neglect the connector's viscous drag. [Stokes law](../../../../stokes-s-law.md) gives $\mathbf f_i=-6\pi\mu a_i\mathbf U$ for each sphere. Their resultant is

$$
\mathbf F=\mathbf f_1+\mathbf f_2=-6\pi\mu(a_1+a_2)\mathbf U,
\qquad\boxed{A\simeq6\pi\mu(a_1+a_2)I.}
$$

This is the leading two-sphere approximation, not an exact finite-separation [hydrodynamic resistance matrix](../../../../hydrodynamic-resistance-matrix.md). Writing $d=|\mathbf r_2-\mathbf r_1|$ and $\mathbf n=(\mathbf r_2-\mathbf r_1)/d$, the first [Stokeslet](../../../../stokeslet.md) reflection gives, if the connector remains negligible,

$$
A=6\pi\mu(a_1+a_2)I-\frac{9\pi\mu a_1a_2}{d}(I+\mathbf n\mathbf n^T)+O\!\left(\mu\frac{(a_1+a_2)^3}{d^2}\right).
$$

The negative correction expresses reduced drag from fluid entrainment by the other sphere. A very thin but arbitrarily long rod need not have negligible total drag: its typical transverse drag scales as $\mu d/\log(d/b)$ for rod radius $b$. Thus the simple boxed result uses the intended negligibly dragging connector limit as well as $a_i/d\ll1$; the two printed size inequalities alone do not specify a uniform limit in which rod drag vanishes.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
