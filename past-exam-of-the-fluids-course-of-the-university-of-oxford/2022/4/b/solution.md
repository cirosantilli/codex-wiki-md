<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an axisymmetric field without azimuthal motion, the [divergence](../../../../divergence.md) in [spherical coordinates](../../../../spherical-coordinate-system.md) is

$$
\nabla\cdot\mathbf v=\frac1{r^2}\partial_r(r^2v_r)
+\frac1{r\sin\theta}\partial_\theta(\sin\theta v_\theta).
$$

Substituting the given axisymmetric [stream function](../../../../stream-function.md) representation gives

$$
\nabla\cdot\mathbf v
=\frac1{r^2\sin\theta}\left(\partial_r\partial_\theta\Psi
-\partial_\theta\partial_r\Psi\right)=0.
$$

Thus [incompressible flow](../../../../incompressible-flow.md) is automatic.

The [velocity](../../../../velocity.md) components are laboratory-frame components resolved about the instantaneous bubble center. The center itself translates with $U\hat{\mathbf z}=U\cos\theta\hat{\mathbf r}-U\sin\theta\hat{\boldsymbol\theta}$. The [kinematic boundary condition](../../../../kinematic-boundary-condition.md) for a spherical interface gives

$$
\boxed{v_r(a,\theta)=U\cos\theta.}
$$

For negligible internal [dynamic viscosity](../../../../dynamic-viscosity-split.md), continuity of tangential [traction](../../../../traction.md) imposes zero tangential [shear stress](../../../../shear-stress.md), rather than a prescribed tangential [velocity](../../../../velocity.md). In terms of the [strain-rate tensor](../../../../strain-rate-tensor.md),

$$
\boxed{e_{r\theta}(a,\theta)=0,\qquad
\left[\partial_rv_\theta-\frac{v_\theta}{r}
+\frac1r\partial_\theta v_r\right]_{r=a}=0.}
$$

Equivalently, $\partial_rv_\theta(a)=v_\theta(a)/a+U\sin\theta/a$. Axisymmetry gives $v_\phi=0$, and the far-field [boundary condition](../../../../boundary-condition.md) is $\mathbf v\to0$. There is no [no-slip boundary condition](../../../../no-slip-boundary-condition.md) $v_\theta=-U\sin\theta$ on a clean bubble; the liquid can slip tangentially relative to the translating interface.

These are the conditions of the prescribed-sphere [clean-bubble Stokes drag](../../../../clean-bubble-stokes-drag.md) model. A genuinely free bubble also requires a [normal stress](../../../../normal-stress.md) balance. If one additionally insists on spatially uniform gas [pressure](../../../../pressure-split.md), while removing both [surface tension](../../../../surface-tension-split.md) and the variation of [hydrostatic pressure](../../../../hydrostatic-pressure.md), that extra condition is incompatible with the translating spherical solution in part (c). The approximation must therefore be understood as computing drag on an imposed spherical interface, or as retaining the normal balancing effects when checking a free bubble.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
