<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**First method: substitute the trajectory.** Along the [parametric curve](../../../parametric-curve.md), the [temperature](../../../temperature-split.md) is $T(t)=20e^{-\cos^2t}-(1+\sin t)^3$. The [chain rule](../../../chain-rule.md) gives

$$
\boxed{\frac{dT}{dt}
=40\sin t\cos t\,e^{-\cos^2t}-3(1+\sin t)^2\cos t.}
$$

**Second method: use the spatial derivatives.** The [partial derivatives](../../../partial-derivative.md) of the [scalar field](../../../scalar-field.md) are $T_x=-40xe^{-x^2}$ and $T_z=-3(z+1)^2$, while the [velocity](../../../velocity.md) components are $\dot x=-\sin t$ and $\dot z=\cos t$. The [multivariable chain rule](../../../multivariable-chain-rule.md) therefore gives

$$
\frac{dT}{dt}=T_x\dot x+T_z\dot z
=(-40\cos t\,e^{-\cos^2t})(-\sin t)-3(1+\sin t)^2\cos t,
$$

which agrees with the first calculation. This is the [gradient](../../../gradient.md) dotted with the [velocity](../../../velocity.md), rather than a [partial derivative](../../../partial-derivative.md) at a fixed position.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
