<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the negative [gradient](../../../../gradient.md) to the leading far-field [electric potential](../../../../electric-potential.md). In [spherical coordinates](../../../../spherical-coordinate-system.md),

$$
E_r=-\frac{\partial V}{\partial r}=\frac{2\alpha\cos\theta}{r^3},\qquad E_\theta=-\frac1r\frac{\partial V}{\partial\theta}=\frac{\alpha\sin\theta}{r^3},\qquad E_\phi=-\frac1{r\sin\theta}\frac{\partial V}{\partial\phi}=0.
$$

The [electric field](../../../../electric-field-split.md) therefore has the coordinate-independent form

$$
\boxed{\mathbf E=\frac{3(\mathbf p\cdot\hat{\mathbf r})\hat{\mathbf r}-\mathbf p}{4\pi\epsilon_0r^3}.}
$$

For the [electric dipole](../../../../electric-dipole.md) along $z$, use $V=\alpha z/(x^2+y^2+z^2)^{3/2}$. Direct [partial differentiation](../../../../partial-derivative.md) gives the [vector components](../../../../coordinate-linear-algebra.md)

$$
\boxed{E_x=\frac{3\alpha xz}{r^5},\qquad E_y=\frac{3\alpha yz}{r^5},\qquad E_z=\frac{\alpha(3z^2-r^2)}{r^5},\quad r^2=x^2+y^2+z^2.}
$$

On the positive axis the [electric field](../../../../electric-field-split.md) points along the [electric dipole moment](../../../../electric-dipole-moment.md); in the equatorial plane it points oppositely, providing a useful sign check.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
