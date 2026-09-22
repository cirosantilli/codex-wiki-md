<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent a paraxial ray by its height and forward slope $(x,\theta)^{\mathsf T}$, with $\theta=dx/dz$. Free-space propagation leaves the slope unchanged and increases height by $L\theta$, giving

$$
\boxed{P(L)=\begin{pmatrix}1&L\\0&1\end{pmatrix}.}
$$

A [thin lens](../../../../thin-lens.md) leaves the ray height unchanged. A parallel incident ray at height $x$ must emerge toward the focal point, so its slope changes by $-x/f$. By linearity, the same increment applies to any paraxial incident slope:

$$
\boxed{F(f)=\begin{pmatrix}1&0\\-1/f&1\end{pmatrix}.}
$$

These [ray transfer matrices](../../../../ray-transfer-matrix-analysis.md) have determinant one in air and compose in reverse [matrix](../../../../matrix.md) order to the physical order of traversal.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
