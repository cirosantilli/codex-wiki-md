<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) and use the assumed independence of $\varphi$ and $z$. In each material region, the zero [curl](../../../../../curl.md) of the static [electric field](../../../../../electric-field-split.md) gives

$$
\frac{dE_z}{d\rho}=0,\qquad
\frac{d(\rho E_\varphi)}{d\rho}=0.
$$

The tangential [electric field](../../../../../electric-field-split.md) is zero at a [perfect conductor](../../../../../perfect-conductor.md). The [dielectric-interface boundary conditions](../../../../../dielectric-interface-boundary-conditions.md) make its tangential components continuous at each material interface, so $E_z=E_\varphi=0$ throughout the gap. They also vanish in the empty interior and exterior for the regular solution with no applied external [electric field](../../../../../electric-field-split.md). Hence

$$
\boxed{\mathbf E=E_\rho(\rho)\mathbf e_\rho.}
$$

This specifies an axis of direction: the sign of $E_\rho$ depends on the sign of $V$.

For the static [magnetic field](../../../../../magnetic-field-split.md), [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md) implies

$$
\frac1\rho\frac{d(\rho B_\rho)}{d\rho}=0.
$$

Thus $\rho B_\rho$ is constant in each layer. Continuity of the normal [magnetic field](../../../../../magnetic-field-split.md) across every interface makes that constant global, and regularity at the axis makes it zero. Next use $\nabla\times\mathbf H=0$ away from the conducting surfaces. Its $\varphi$ component gives $dH_z/d\rho=0$. There is no azimuthal [surface current density](../../../../../surface-current-density.md), so $H_z$ is continuous across the conducting surfaces and the material interface. The decay of the exterior [magnetic field](../../../../../magnetic-field-split.md) at infinity therefore forces this global constant to zero. The only remaining component is

$$
\boxed{\mathbf B=B_\varphi(\rho)\mathbf e_\varphi.}
$$

The [magnetostatic Ampère law](../../../../../magnetostatic-ampere-law.md) fixes its sign: positive inner [electric current](../../../../../electric-current.md) in the $+z$ direction produces positive $B_\varphi$ for positive [magnetic permeability](../../../../../permeability-electromagnetism.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
