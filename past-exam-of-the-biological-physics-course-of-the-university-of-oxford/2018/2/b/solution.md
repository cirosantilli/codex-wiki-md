<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let a segment of fixed length $b$ make angle $\theta$ with an applied [force](../../../../force-split.md) $\mathbf f=f\hat{\mathbf z}$. Its [energy](../../../../energy-split.md) contribution is $-fb\cos\theta$. Independent freely jointed orientations give the single-segment [partition function](../../../../canonical-partition-function.md) and chain [partition function](../../../../canonical-partition-function.md)

$$
Z_1=\int e^{u\cos\theta}d\Omega=4\pi\frac{\sinh u}{u},\qquad
u=\frac{fb}{k_BT},\qquad Z_N=Z_1^N.
$$

The mean end-to-end projection is the [force](../../../../force-split.md) [derivative](../../../../derivative.md) of $k_BT\ln Z_N$:

$$
\langle R_z\rangle=Nb\left(\coth u-\frac1u\right).
$$

For $|u|\ll1$, the [Langevin function](../../../../langevin-function.md) is $u/3+O(u^3)$. [Isotropy](../../../../isotropy.md) therefore gives the vector response

$$
\boxed{\langle\mathbf R\rangle=\frac{Nb^2}{3k_BT}\mathbf f+O(f^3),\qquad
\mathbf f=\frac{3k_BT}{Nb^2}\langle\mathbf R\rangle\quad\text{to linear order}.}
$$

The [covariance](../../../../covariance.md) at zero [force](../../../../force-split.md) provides an independent route: $\langle R_iR_j\rangle_0=Nb^2\delta_{ij}/3$, and the [Boltzmann weight](../../../../boltzmann-factor.md)'s first-order term yields $\langle R_i\rangle=f_j\langle R_iR_j\rangle_0/(k_BT)$. This is a relation for the [mean vector](../../../../mean-vector.md) or its projection. The zero-[force](../../../../force-split.md) [mean vector](../../../../mean-vector.md) vanishes even though the chain has finite [root mean square](../../../../root-mean-square.md) size $b\sqrt N$.

The controlled weak-[force](../../../../force-split.md) condition is $fb\ll k_BT$, not merely that a short part of a measured curve looks straight. With the supplied $b$, $k_BT/b\simeq10.3\,\mathrm{pN}$ at $25^\circ\mathrm C$. A raw [force](../../../../force-split.md) near $30\,\mathrm{pN}$, as in the figure's labelled low-extension portion, would give $u\simeq2.9$ and is not asymptotically weak for those literal segment parameters. A [force](../../../../force-split.md) offset or different effective model might change that interpretation, but no such correction should be invented from the plot.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
