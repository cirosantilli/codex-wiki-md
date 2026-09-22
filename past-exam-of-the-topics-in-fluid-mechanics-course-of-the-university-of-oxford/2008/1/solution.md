<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The four dimensional equations express [mass conservation](../../../mass-conservation.md), [momentum balance](../../../momentum-conservation.md) with [pressure](../../../pressure-split.md), [gravity](../../../gravity.md) and [viscous stress](../../../viscous-stress-tensor.md), heat advection and conduction, and a linear thermal-expansion [equation of state](../../../equation-of-state.md). For heating from below, suitable plate conditions are $\mathbf u=0$ and $T=T_0+\Delta T$ at $z=0$, and $\mathbf u=0$, $T=T_0$ at $z=d$. [No slip](../../../no-slip-boundary-condition.md) and [thermal insulation](../../../thermal-insulation.md) on the sidewall provide one suitable lateral completion; prescribed lateral [temperatures](../../../temperature-split.md) would be another specified thermal setup.

Let $\kappa=k/(\rho_0c_p)$ be [thermal diffusivity](../../../thermal-diffusivity.md) and $\nu=\mu/\rho_0$ [kinematic viscosity](../../../kinematic-viscosity.md). Use $d$, $d^2/\kappa$, $\kappa/d$ and $\Delta T$ as length, time, [velocity](../../../velocity.md) and [temperature](../../../temperature-split.md) scales. Subtract the static reference [pressure](../../../pressure-split.md) $p_H$ with $\nabla p_H=-\rho_0g\mathbf k$ and scale its remainder by $\mu\kappa/d^2$. Then

$$
\boxed{B=\alpha\Delta T,\qquad Pr=\nu/\kappa,\qquad Ra=\frac{g\alpha\Delta T d^3}{\nu\kappa}.}
$$

[Density](../../../density.md) becomes $\rho_0(1-BT)$. Substitution and division by the corresponding diffusion/viscous scales give

$$
-BT_t+\nabla\cdot[(1-BT)\mathbf u]=0,\qquad
Pr^{-1}(1-BT)(\mathbf u_t+\mathbf u\cdot\nabla\mathbf u)=-\nabla p+Ra\,T\mathbf k+\Delta\mathbf u,
$$



$$
(1-BT)(T_t+\mathbf u\cdot\nabla T)=\Delta T.
$$

In the Boussinesq small-[density](../../../density.md)-contrast limit retain [buoyancy](../../../buoyancy.md) while neglecting the other $B$ factors. At infinite [Prandtl number](../../../prandtl-number.md), after any fast initial adjustment, the equations are

$$
\boxed{\nabla\cdot\mathbf u=0,\qquad0=-\nabla p+Ra\,T\mathbf k+\Delta\mathbf u,\qquad T_t+\mathbf u\cdot\nabla T=\Delta T.}
$$

The [velocity](../../../velocity.md) is instantaneously constrained by a viscous elliptic balance; the [temperature](../../../temperature-split.md) still evolves.

Take the [divergence](../../../divergence.md) of the [vector Poisson equation](../../../poisson-s-equation.md). Derivatives commute, and [divergence](../../../divergence.md) of a [curl](../../../curl.md) is zero, so $\Delta(\nabla\cdot\mathbf A)=0$. Its boundary value is zero, hence the [maximum principle](../../../maximum-principle.md) gives $\nabla\cdot\mathbf A=0$ throughout $D$. The vector identity now gives $\operatorname{curl}\operatorname{curl}\mathbf A=\operatorname{curl}\mathbf u$, or

$$
\operatorname{curl}(\operatorname{curl}\mathbf A-\mathbf u)=0.
$$

The layer domain is [simply connected](../../../simply-connected-space.md) because its horizontal section is [simply connected](../../../simply-connected-space.md). For a [curl](../../../curl.md)-free field on such a domain, define $\chi(x)$ as its [line integral](../../../line-integral.md) from a fixed base point to $x$. Contractibility of loops and [Stokes theorem](../../../stokes-theorem.md) make the [integral](../../../integral-split.md) [path independent](../../../path-independence.md), and differentiation gives its [gradient](../../../gradient.md) equal to the field. Thus $\operatorname{curl}\mathbf A-\mathbf u=\nabla\chi$.

[Incompressibility](../../../incompressible-flow.md) then gives $\Delta\chi=0$, while the prescribed normal [curl](../../../curl.md) gives $\partial_n\chi=0$. [Green's identity](../../../green-s-first-identity.md) yields

$$
\int_D|\nabla\chi|^2\,dV=\int_{\partial D}\chi\partial_n\chi\,dS-\int_D\chi\Delta\chi\,dV=0.
$$

Hence $\chi$ is constant on the connected domain and $\boxed{\operatorname{curl}\mathbf A=\mathbf u}$. The extra condition $\mathbf A\cdot\mathbf n=0$ belongs to the stated potential boundary problem; the reconstruction argument above uses the [divergence](../../../divergence.md) and normal-[curl](../../../curl.md) conditions. On a multiply connected domain a [curl](../../../curl.md)-free field need not be a globally single-valued [gradient](../../../gradient.md).

Finally $\operatorname{curl}(T\mathbf k)=(T_y,-T_x,0)$. Taking the [curl](../../../curl.md) of the infinite-Prandtl [momentum balance](../../../momentum-conservation.md) and using $\operatorname{curl}\mathbf u=-\Delta\mathbf A$ gives

$$
0=Ra(T_y\mathbf i-T_x\mathbf j)-\Delta^2\mathbf A,\qquad
\boxed{\nabla^4\mathbf A+Ra(T_x\mathbf j-T_y\mathbf i)=0.}
$$

The derivation is an instance of [velocity reconstruction from a mixed-boundary vector Poisson problem](../../../velocity-reconstruction-from-a-mixed-boundary-vector-poisson-problem.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2008](../../2008-split.md)
3. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../split.md)
4. [Topics in fluid mechanics course of the University of Oxford](../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
