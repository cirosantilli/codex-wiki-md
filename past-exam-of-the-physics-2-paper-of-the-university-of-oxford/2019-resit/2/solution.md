<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Interpret the coordinates as a plane in ordinary three-dimensional [electrostatics](../../../electrostatics-split.md). Set $k_e=1/(4\pi\epsilon_0)$, where $\epsilon_0$ is the [vacuum permittivity](../../../vacuum-permittivity.md). The work required to bring the second [point charge](../../../point-charge.md) in quasistatically is its [electric charge](../../../electric-charge-split.md) times the first charge's [electric potential](../../../electric-potential.md):

$$
\boxed{U=-\frac{k_eQ^2}{d}.}
$$

The individual point-charge self-energies are excluded; this is the [electrostatic potential energy of point charges](../../../electrostatic-potential-energy-of-point-charges.md) relative to infinite separation.

By the [superposition principle](../../../superposition-principle.md), for $\mathbf r=(x,y)$ and $\mathbf d=(d,0)$ the [electric field](../../../electric-field-split.md) is

$$
\mathbf E(\mathbf r)=k_eQ\left(\frac{\mathbf r}{|\mathbf r|^3}-\frac{\mathbf r-\mathbf d}{|\mathbf r-\mathbf d|^3}\right).
$$

At the first position both contributions point toward positive $x$, whereas at the second they oppose one another. Thus

$$
\boxed{\mathbf E(d/3,0)=\frac{45k_eQ}{4d^2}\,\hat{\mathbf x},\qquad
\mathbf E(-d/3,0)=-\frac{135k_eQ}{16d^2}\,\hat{\mathbf x}.}
$$

At $(d/2,d)$ the two distances are $\sqrt5d/2$. The vertical [electric field](../../../electric-field-split.md) components cancel and the horizontal components add:

$$
\boxed{\mathbf E(d/2,d)=\frac{8k_eQ}{5\sqrt5\,d^2}\,\hat{\mathbf x}.}
$$

**Dimensional convention.** The source's description of space as two-dimensional cannot literally mean two-dimensional [electrostatics](../../../electrostatics-split.md) with the same inverse-square formula. In a genuinely two-dimensional [Gauss's law](../../../gauss-s-law.md), the circumference grows as $r$, giving an [electric field](../../../electric-field-split.md) proportional to $1/r$ and a logarithmic [electric potential](../../../electric-potential.md). For example, integrating $1/r$ from $d$ to infinity diverges, so the same finite reference [potential energy](../../../potential-energy.md) at infinite separation does not exist. The displayed results use the conventional three-dimensional [Coulomb's law](../../../coulomb-s-law.md) restricted to the stated plane.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
