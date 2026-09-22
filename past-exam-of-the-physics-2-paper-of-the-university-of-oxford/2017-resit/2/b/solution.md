<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [uniform space charge in a grounded spherical cavity](../../../../uniform-space-charge-in-a-grounded-spherical-cavity.md), [grounding](../../../../grounding.md) sets the metal's [electric potential](../../../../electric-potential.md) to zero. With no external sources and zero [electric potential](../../../../electric-potential.md) at infinity, the exterior [electric potential](../../../../electric-potential.md) is also zero by the [uniqueness theorem for the electrostatic potential](../../../../uniqueness-theorem-for-the-electrostatic-potential.md). The original shell [electric charge](../../../../electric-charge-split.md) is no longer fixed: [electric charge](../../../../electric-charge-split.md) can flow to or from earth.

Inside the cavity, [Gauss's law](../../../../gauss-s-law.md) gives $\mathbf E=\rho r\hat{\mathbf r}/(3\epsilon_0)$. Integrating the [electric field](../../../../electric-field-split.md) inward from the zero boundary [electric potential](../../../../electric-potential.md) gives

$$
V(r)=\int_r^{r_1}\frac{\rho s}{3\epsilon_0}\,ds
=\frac{\rho(r_1^2-r^2)}{6\epsilon_0},\qquad
\boxed{V(0)=\frac{\rho r_1^2}{6\epsilon_0}.}
$$

The inner surface carries $-Q_\rho$, where $Q_\rho=4\pi\rho r_1^3/3$, and the outer surface carries zero net [electric charge](../../../../electric-charge-split.md). Only the cavity contributes to the final [electrostatic energy](../../../../electrostatic-energy.md):

$$
U=\frac{\epsilon_0}{2}\int |\mathbf E|^2\,d^3r
=\frac{\epsilon_0}{2}4\pi\int_0^{r_1}\left(\frac{\rho r}{3\epsilon_0}\right)^2r^2\,dr,
\qquad
\boxed{U=\frac{2\pi\rho^2r_1^5}{45\epsilon_0}
=\frac{Q_\rho^2}{40\pi\epsilon_0r_1}.}
$$

The same result follows from $U=\tfrac12\int\rho V\,d^3r$; the conductor's [surface charge](../../../../surface-charge.md) contributes zero because its [electric potential](../../../../electric-potential.md) is zero. This is the final stored [electrostatic energy](../../../../electrostatic-energy.md), not the change from the earlier central-charge configuration, whose ideal [point charge](../../../../point-charge.md) has divergent self-energy.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
