<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the applied [force](../../../../force-split.md) be $\mathbf f=f\hat{\mathbf z}$. A segment with polar angle $\theta$ has energy $-fb\cos\theta$. Independent 3D orientations give the one-link [partition function](../../../../canonical-partition-function.md)

$$
Z_1=\int e^{fb\cos\theta/(k_BT)}d\Omega
=4\pi\frac{\sinh u}{u},\qquad u=\frac{fb}{k_BT},\qquad Z_N=Z_1^N.
$$

Taking the [force](../../../../force-split.md) [derivative](../../../../derivative.md) of $k_BT\ln Z_N$ yields the mean end-to-end projection,

$$
\langle R_z\rangle=Nb\left(\coth u-\frac1u\right).
$$

For $u\ll1$, $\coth u-1/u=u/3+O(u^3)$, so

$$
\boxed{\langle\mathbf R\rangle=\frac{Nb^2}{3k_BT}\mathbf f+O(f^3),\qquad
\mathbf f=\frac{3k_BT}{Nb^2}\langle\mathbf R\rangle.}
$$

[Isotropy](../../../../isotropy.md) supplies the [vector](../../../../vector.md) relation. It is the mean [vector](../../../../vector.md) or its projection, not the mean magnitude of a fluctuating chain; at zero [force](../../../../force-split.md) $\langle\mathbf R\rangle=0$ while $\langle R^2\rangle=Nb^2$ remains positive. The last panel of the model figure in [solution](../../4/b/solution.md) shows the exact orientational response and its weak-[force](../../../../force-split.md) tangent.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
