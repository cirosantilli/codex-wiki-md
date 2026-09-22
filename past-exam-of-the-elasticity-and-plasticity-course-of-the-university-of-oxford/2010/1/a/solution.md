<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [displacement](../../../../displacement.md) follows a material point from its reference position to its current position:

$$
\boxed{\mathbf u(\mathbf X,t)=\mathbf x(\mathbf X,t)-\mathbf X.}
$$

The [deformation gradient](../../../../deformation-gradient.md) is the [Jacobian matrix](../../../../jacobian-matrix.md) $F=\partial\mathbf x/\partial\mathbf X=I+\nabla_X\mathbf u$, and the volume Jacobian is

$$
\boxed{J=\det F,\qquad dV=J\,dV_0.}
$$

For an orientation-preserving physical [deformation](../../../../deformation-mechanics.md), $J>0$ measures the local volume expansion factor. [Incompressibility](../../../../incompressible-flow.md) requires $J=1$; [conservation of mass](../../../../mass-conservation.md) gives $\rho(\mathbf x,t)J=\rho_0(\mathbf X)$. For small [displacement](../../../../displacement.md) [gradients](../../../../gradient.md), $J=1+\nabla_X\cdot\mathbf u+O(|\nabla_X\mathbf u|^2)$. If a spatial representation is desired, the same [displacement](../../../../displacement.md) is $\mathbf u(\mathbf x,t)=\mathbf x-\mathbf X(\mathbf x,t)$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
