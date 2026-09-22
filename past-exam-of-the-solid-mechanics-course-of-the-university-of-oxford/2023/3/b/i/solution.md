<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Restore the particle label suppressed in the question, writing the static family as $\mathbf x_0(\mathbf X;\tau)$. At each fixed $\tau$, its [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) satisfies

$$
\operatorname{div}\mathbf T_0(\tau)+\rho\mathbf b=\mathbf0.
$$

This [dynamic continuation of a static incompressible elastic deformation](../../../../../dynamic-continuation-of-a-static-incompressible-elastic-deformation.md) sets $\tau=t$ to form a motion. At every time its [deformation gradient](../../../../../deformation-gradient.md) is the same as that of the corresponding static member. For an elastic material the elastic part of the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) depends on that [deformation gradient](../../../../../deformation-gradient.md), while [incompressibility](../../../../../incompressible-flow.md) leaves an arbitrary scalar [constraint reaction in hyperelastic stress](../../../../../constraint-reaction-in-hyperelastic-stress.md). Therefore write

$$
\mathbf T_0=\mathbf S(\mathbf F)-p_0\mathbf1,\qquad
\mathbf T=\mathbf S(\mathbf F)-p\mathbf1,
\qquad
\mathbf T-\mathbf T_0=(p_0-p)\mathbf1.
$$

Here $\mathbf1$ is the [identity matrix](../../../../../identity-matrix.md). Subtracting static [balance of linear momentum](../../../../../balance-of-linear-momentum.md) from dynamic [balance of linear momentum](../../../../../balance-of-linear-momentum.md) gives

$$
\rho\ddot{\mathbf x}_0=\nabla(p_0-p).
$$

Since the homogeneous incompressible material has constant [mass density](../../../../../density.md), define $\xi=(p-p_0)/\rho$. Necessarily

$$
\boxed{\ddot{\mathbf x}_0(\mathbf X,t)
=-\nabla\xi(\mathbf x_0(\mathbf X,t),t).}
$$

Conversely, suppose this [acceleration potential](../../../../../acceleration-potential.md) exists. Choose $p=p_0+\rho\xi$. Then

$$
\operatorname{div}\mathbf T+\rho\mathbf b
=\operatorname{div}\mathbf T_0+\rho\mathbf b-\rho\nabla\xi
=\rho\ddot{\mathbf x}_0.
$$

The added isotropic [stress](../../../../../stress.md) is symmetric, so [angular momentum conservation](../../../../../conservation-of-angular-momentum.md) remains satisfied. This proves both directions for the field equations and the elastic [constitutive equation](../../../../../constitutive-equation.md). The surface [tractions](../../../../../traction.md) for the motion are those of the adjusted [stress](../../../../../stress.md); identical prescribed static [tractions](../../../../../traction.md) would impose an additional boundary restriction on $\xi$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the solid mechanics course of the University of Oxford](../../../../split.md)
6. [Solid mechanics course of the University of Oxford](../../../../../solid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
