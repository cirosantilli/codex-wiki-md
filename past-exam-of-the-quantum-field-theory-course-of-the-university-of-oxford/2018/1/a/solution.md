<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Divide the infinitesimal [variation](../../../../variation.md) by its constant parameter $\alpha$, so the transformation generator is $(\delta\phi_1,\delta\phi_2)=(\phi_2,-\phi_1)$. The variation of the [kinetic term](../../../../kinetic-term.md) is

$$
\partial_\mu\phi_1\partial^\mu\phi_2-\partial_\mu\phi_2\partial^\mu\phi_1=0,
$$

and that of $\phi_1^2+\phi_2^2$ is $2\phi_1\phi_2-2\phi_2\phi_1=0$. Thus the [Lagrangian density](../../../../lagrangian-density.md) is invariant pointwise, without a nonzero boundary current. The finite transformation is a rotation of the two [real scalar fields](../../../../real-scalar-field.md), giving an [SO(2)](../../../../special-orthogonal-group-in-two-dimensions.md) [global symmetry in field theory](../../../../global-symmetry-in-field-theory.md).

[Noether's theorem](../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) supplies the parameter-independent [Noether current](../../../../noether-current.md)

$$
\boxed{j^\mu=\phi_2\partial^\mu\phi_1-\phi_1\partial^\mu\phi_2.}
$$

Its [divergence](../../../../divergence.md) is $\partial_\mu j^\mu=\phi_2\Box\phi_1-\phi_1\Box\phi_2$, since the first-derivative terms cancel. Both fields obey the same [Klein-Gordon equation](../../../../klein-gordon-equation.md), so this vanishes on solutions. With spatial boundary conditions giving zero flux at infinity, the [Noether charge](../../../../noether-charge.md) is

$$
\boxed{Q=\int d^3x\,(\phi_2\dot\phi_1-\phi_1\dot\phi_2),\qquad \dot Q=0.}
$$

A finite box with periodic [boundary conditions](../../../../boundary-condition.md) works as well. The spatial integral is conserved because the local [continuity equation](../../../../continuity-equation.md) converts its time derivative into a boundary flux; neither vanishing local current nor constant individual fields is required. Equivalently, $\Phi=(\phi_1+i\phi_2)/\sqrt2$ transforms as $\Phi\mapsto e^{-i\alpha}\Phi$, exhibiting the equivalent [global U(1) symmetry](../../../../global-u-1-symmetry.md) and fixing the sign of the generator.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
