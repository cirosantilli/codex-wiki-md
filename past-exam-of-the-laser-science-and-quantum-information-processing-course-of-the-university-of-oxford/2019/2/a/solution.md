<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [paraxial](../../../../paraxial-approximation.md) [Gaussian beam](../../../../gaussian-beam.md), choose the [complex beam parameter](../../../../complex-beam-parameter.md) with

$$
\frac1q=\frac1{R_b}-i\frac{\lambda}{\pi w^2},\qquad
q=z+iz_R,\quad z_R>0.
$$

Here $R_b$ is the wavefront radius and $w$ the intensity $1/e^2$ radius. The [ABCD law](../../../../abcd-law-for-gaussian-beams.md) is

$$
\boxed{q_{\rm out}=\frac{Aq_{\rm in}+B}{Cq_{\rm in}+D}.}
$$

For a real, lossless round-trip [ray transfer matrix](../../../../ray-transfer-matrix-analysis.md) $M$ in free space, $AD-BC=1$. A reproducing [cavity](../../../../optical-cavity.md) mode requires $q=(Aq+B)/(Cq+D)$, hence

$$
Cq^2+(D-A)q-B=0,\qquad
(D-A)^2+4BC=(A+D)^2-4.
$$

Except for a [scalar identity matrix](../../../../scalar-matrix.md), a finite physical solution requires a [complex-conjugate](../../../../complex-conjugate.md) root pair, one with positive imaginary part. The generic strict stability condition is therefore

$$
\boxed{-2<A+D<2.}
$$

Equivalently, the ray [eigenvalues](../../../../eigenvalue.md) are distinct unit-modulus numbers $e^{\pm i\mu}$, so repeated round trips do not cause unbounded ray excursions. Adequate [mirror](../../../../mirror.md) apertures and longitudinal resonance are also needed for a low-loss resonant mode.

**The strict inequality has a degenerate exception relevant to this paper.** If $M=-I$, then $q'=q$ for every physical $q$ even though $A+D=-2$. A symmetric [confocal resonator](../../../../confocal-optical-resonator.md) has exactly this [matrix](../../../../matrix.md) and supports Gaussian modes; it is not excluded as a physical [cavity](../../../../optical-cavity.md). Thus the printed strict condition should be understood as the generic, nondegenerate stability criterion, not a universal necessary condition covering the confocal case in [c](../c.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
