<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the source's [Gaussian units](../../../../gaussian-units.md) and neglect the [displacement current](../../../../displacement-current.md), as in nonrelativistic [magnetohydrodynamics](../../../../magnetohydrodynamics-split.md). Write $\Delta p=p_\perp-p_\parallel$ for the [pressure anisotropy](../../../../pressure-anisotropy.md). The [pressure tensor](../../../../pressure-tensor.md) is $\mathsf P=p_\perp\mathsf I-\Delta p\,\mathbf b\mathbf b$, so its [force density](../../../../force-density.md) is

$$
-\nabla\cdot\mathsf P=-\nabla p_\perp+\nabla\cdot(\Delta p\,\mathbf b\mathbf b).
$$

[Ampère's law](../../../../ampere-s-circuital-law.md) and the [solenoidal magnetic-field constraint](../../../../solenoidal-magnetic-field-constraint.md) give the [Lorentz force](../../../../lorentz-force.md) decomposition

$$
\frac{\mathbf j\times\mathbf B}{c}
=\frac{(\nabla\times\mathbf B)\times\mathbf B}{4\pi}
=-\nabla\frac{B^2}{8\pi}+\frac{(\mathbf B\cdot\nabla)\mathbf B}{4\pi}
=-\nabla\frac{B^2}{8\pi}+\nabla\cdot\frac{\mathbf B\mathbf B}{4\pi}.
$$

Adding these two [force densities](../../../../force-density.md) and using $\mathbf B\mathbf B=B^2\mathbf b\mathbf b$ yields

$$
\boxed{\rho\frac{D\mathbf u}{Dt}=-\nabla\left(p_\perp+\frac{B^2}{8\pi}\right)+\nabla\cdot\left[\left(\Delta p+\frac{B^2}{4\pi}\right)\mathbf b\mathbf b\right].}
$$

The first term is the [gradient](../../../../gradient.md) of the modified [magnetohydrodynamic total pressure](../../../../magnetohydrodynamic-total-pressure.md); the second is the anisotropic [Maxwell stress tensor](../../../../maxwell-stress-tensor.md) contribution together with the directional [pressure force](../../../../pressure-force.md). Their effective coefficient is the [pressure-anisotropy-modified magnetic tension](../../../../pressure-anisotropy-modified-magnetic-tension.md), $\mathcal T=B^2/(4\pi)+\Delta p$. At fixed [magnetic field](../../../../magnetic-field-split.md), positive [pressure anisotropy](../../../../pressure-anisotropy.md) increases resistance to bending, while negative [pressure anisotropy](../../../../pressure-anisotropy.md) reduces it. When $\mathcal T$ becomes negative, bending experiences an amplifying [force](../../../../force-split.md) rather than a restoring [force](../../../../force-split.md). Gradients of $\Delta p$ can also drive motion, so the curvature interpretation refers specifically to the bending contribution.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
