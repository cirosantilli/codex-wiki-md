<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the same constant [dynamic viscosity](../../../../dynamic-viscosity-split.md) $\mu$ for both incompressible [Stokes flows](../../../../stokes-flow-split.md), and let $\mathbf f^{(a)}$ be [body force](../../../../body-force.md) per unit volume. Their equations and [Newtonian fluid stress tensor](../../../../newtonian-fluid-stress-tensor.md) are

$$
\partial_j\sigma^{(a)}_{ij}+f^{(a)}_i=0,\qquad
\partial_i u^{(a)}_i=0,\qquad
\sigma^{(a)}_{ij}=-p^{(a)}\delta_{ij}+2\mu e^{(a)}_{ij},
$$

where $e^{(a)}_{ij}=(\partial_i u^{(a)}_j+\partial_j u^{(a)}_i)/2$ is the [strain-rate tensor](../../../../strain-rate-tensor.md). Consider the cross-work flux

$$
Q_j=u_i^{(2)}\sigma^{(1)}_{ij}-u_i^{(1)}\sigma^{(2)}_{ij}.
$$

By the product rule,

$$
\partial_jQ_j
=(\partial_j u_i^{(2)})\sigma^{(1)}_{ij}
-(\partial_j u_i^{(1)})\sigma^{(2)}_{ij}
-u_i^{(2)}f_i^{(1)}+u_i^{(1)}f_i^{(2)}.
$$

The pressure terms vanish by [incompressibility](../../../../incompressible-flow.md). Symmetry of the [stress tensor](../../../../cauchy-stress-tensor.md) removes antisymmetric [velocity gradient](../../../../velocity-gradient.md) contributions, leaving $2\mu e^{(1)}:e^{(2)}$ in both cross terms; they cancel. Apply the [divergence theorem](../../../../divergence-theorem.md), with $\mathbf n$ outward from $V$, and rearrange:

$$
\boxed{\begin{aligned}
\int_V\mathbf f^{(1)}\cdot\mathbf u^{(2)}\,dV
+\int_{\partial V}\mathbf u^{(2)}\cdot\boldsymbol\sigma^{(1)}\mathbf n\,dS
={}&\int_V\mathbf f^{(2)}\cdot\mathbf u^{(1)}\,dV\\
&+\int_{\partial V}\mathbf u^{(1)}\cdot\boldsymbol\sigma^{(2)}\mathbf n\,dS.
\end{aligned}}
$$

This is the [Lorentz reciprocal theorem with body forces](../../../../lorentz-reciprocal-theorem-with-body-forces.md). It depends on reciprocal linear viscous response in the same fluid; arbitrary unrelated constitutive laws would not supply the cross-term cancellation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
