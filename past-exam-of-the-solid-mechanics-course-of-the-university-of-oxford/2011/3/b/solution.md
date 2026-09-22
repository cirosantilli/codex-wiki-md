<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the [boundary](../../../../boundary-of-a-set.md) split into a displacement part $\Gamma_D$ and a [traction](../../../../traction.md) part $\Gamma_N$. The linearized stored [elastic energy](../../../../elastic-energy.md) functional is

$$
\boxed{I^{\mathrm{lin}}[u]=\frac12\int_\Omega\mathbb A_{iA jB}u_{i,A}u_{j,B}\,dx.}
$$

Its corresponding total potential subtracts the work of fixed body and surface loads:

$$
\Pi[u]=I^{\mathrm{lin}}[u]-\int_\Omega f\cdot u\,dx-\int_{\Gamma_N}g\cdot u\,dA.
$$

The problem in the [calculus of variations](../../../../calculus-of-variations-split.md) is to minimize $\Pi$ among admissible displacements with $u=u_D$ on $\Gamma_D$. For a stable quadratic [elastic energy](../../../../elastic-energy.md) this is the usual energy minimization formulation. Its stationarity condition suffices to derive equilibrium.

Vary by $u+sv$, with $v=0$ on $\Gamma_D$. Major [symmetry](../../../../symmetry-physics.md) combines the two differentiated quadratic terms, giving

$$
\int_\Omega S^{\mathrm{lin}}:Dv\,dx=\int_\Omega f\cdot v\,dx+\int_{\Gamma_N}g\cdot v\,dA,
\qquad S^{\mathrm{lin}}_{iA}=\mathbb A_{iA jB}u_{j,B}.
$$

[Integration by parts](../../../../integration-by-parts.md), first with test functions compactly supported in the interior, gives $-\operatorname{Div}S^{\mathrm{lin}}=f$. Then arbitrary traces on $\Gamma_N$ give the natural [traction](../../../../traction.md) condition. The complete [boundary value problem](../../../../boundary-value-problem-split.md) is

$$
\boxed{-\operatorname{Div}S^{\mathrm{lin}}=f\text{ in }\Omega,\qquad
S^{\mathrm{lin}}N=g\text{ on }\Gamma_N,\qquad u=u_D\text{ on }\Gamma_D.}
$$

For a [homogeneous hyperelastic material](../../../../homogeneous-hyperelastic-material.md) the [elasticity tensor](../../../../elasticity-tensor.md) is constant. In [isotropic](../../../../isotropy.md) [linear elasticity](../../../../linear-elasticity.md) the [constitutive equation](../../../../constitutive-equation.md) is $S^{\mathrm{lin}}=\lambda\operatorname{div}u\,I+\mu(Du+Du^T)$, giving the familiar [Navier-Cauchy equation](../../../../navier-cauchy-equation.md) $-\mu\Delta u-(\lambda+\mu)\nabla\operatorname{div}u=f$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
