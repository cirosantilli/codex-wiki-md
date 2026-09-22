<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the common constant [mass density](../../../../density.md), the background [hydrostatic pressure](../../../../hydrostatic-pressure.md) satisfies $dp_0/dz=-\rho g$. Define the excess [pressure](../../../../pressure-split.md) $P=p-p_0(z)$. In [Darcy's law](../../../../darcy-law.md), the background [pressure gradient](../../../../pressure-gradient.md) cancels [gravity](../../../../gravity.md):

$$
\mathbf q=-\frac{\Pi_1}{\eta}(\nabla p+\rho g\hat{\mathbf z})
=-\frac{\Pi_1}{\eta}\nabla P,\qquad \nabla^2P=0.
$$

If the source imposes the same excess [pressure](../../../../pressure-split.md) relative to the local [hydrostatic pressure](../../../../hydrostatic-pressure.md) everywhere on its spherical surface, $P(a)=\Delta p$, the [spherical Darcy injection](../../../../spherical-darcy-injection.md) result survives exactly:

$$
\boxed{p(\mathbf x)=p_0(z)+\frac{a\Delta p}{r},\qquad
\mathbf q=\frac{\Pi_1a\Delta p}{\eta r^2}\hat{\mathbf r}.}
$$

It is important to specify what is maintained on the source. A literally uniform absolute [pressure](../../../../pressure-split.md) $p_s=p_0(0)+\Delta p$ on a finite sphere centered at $z=0$ instead gives $P(a,\theta)=\Delta p+\rho ga\cos\theta$, where $\theta$ is measured from the upward vertical. The decaying [harmonic function](../../../../harmonic-function.md) outside the sphere is then

$$
P=\frac{a\Delta p}{r}+\frac{\rho ga^3\cos\theta}{r^2},
$$

and therefore

$$
q_r=\frac{\Pi_1}{\eta}\left(\frac{a\Delta p}{r^2}+\frac{2\rho ga^3\cos\theta}{r^3}\right),\qquad
q_\theta=\frac{\Pi_1\rho ga^3\sin\theta}{\eta r^3}.
$$

This supplies a concrete exception to an unqualified claim that [gravity](../../../../gravity.md) leaves the radial flow unchanged. The additional dipolar contribution has zero net [volumetric flow rate](../../../../volumetric-flow-rate.md), so $Q=4\pi\Pi_1a\Delta p/\eta$ still holds. Equal injected and resident [mass densities](../../../../density.md) are essential to the background cancellation.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
