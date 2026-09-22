<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a planar [incompressible flow](../../../../../incompressible-flow.md), the [divergence](../../../../../divergence.md) of the [velocity field](../../../../../velocity-field.md) must vanish. Here

$$
\nabla\cdot\mathbf u=\frac{\partial u}{\partial x}+\frac{\partial v}{\partial y}=-1+1=0.
$$

Equivalently, the [Jacobian determinant](../../../../../jacobian-determinant.md) of the [deformation map](../../../../../deformation-map.md) is

$$
\det\frac{\partial(x,y)}{\partial(X,Y)}
=e^{-t}e^t(\cos^2\Omega t+\sin^2\Omega t)=1,
$$

so every material area is preserved. However, the out-of-plane [vorticity](../../../../../vorticity-split.md) is

$$
\boxed{\omega_z=\frac{\partial v}{\partial x}-\frac{\partial u}{\partial y}
=-\Omega(e^{2t}+e^{-2t})=-2\Omega\cosh(2t)}.
$$

Since $\Omega>0$, this [vorticity](../../../../../vorticity-split.md) never vanishes. The motion is an [incompressible flow](../../../../../incompressible-flow.md) but is not an [irrotational flow](../../../../../irrotational-flow.md); its local spin is clockwise.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
