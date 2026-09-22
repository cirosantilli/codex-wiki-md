<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The temporal [integration by parts](../../../../../../integration-by-parts.md) terms are

$$
-[\,(\mathbf u^\dagger,\delta\mathbf u)+(\theta^\dagger,\delta\theta)\,]_0^T
-(\mathbf u_0^\dagger,\delta\mathbf u(0)-\delta\mathbf u_0)
+2(\Theta(T),\delta\theta(T)).
$$

The terminal states are free and the objective has no explicit terminal-[velocity](../../../../../../velocity.md) dependence. Therefore

$$
\boxed{\mathbf u^\dagger(T)=\mathbf0,\qquad
\theta^\dagger(T)=2\Theta(T).}
$$

The factor two follows from the displayed objective without a $1/2$ prefactor. The initial [scalar field](../../../../../../scalar-field.md) perturbation is fixed, so $\delta\theta(0)=0$ and there is no independently prescribed adjoint-scalar condition at $t=0$. Its value there is obtained by backward integration. Independent variation of the initial [velocity](../../../../../../velocity.md) state gives $\mathbf u^\dagger(0)=\mathbf u_0^\dagger$.

Variation of the candidate $\mathbf u_0$ in the energy-augmented functional gives the [fixed-energy initial-condition optimality](../../../../../../fixed-energy-initial-condition-optimality.md) condition. For the usual divergence-free no-slip control space $H$, write $P_H$ for its [orthogonal projection](../../../../../../orthogonal-projection.md), the [Leray-Helmholtz projection](../../../../../../leray-helmholtz-projection.md) in the usual incompressible [velocity](../../../../../../velocity.md) space. This is the standard formal control condition when [pressure](../../../../../../pressure.md) is determined by [incompressible flow](../../../../../../incompressible-flow.md) and normal momentum. If the independently imposed direct [pressure](../../../../../../pressure.md) flux is retained as an additional constraint, the admissible control variations must also satisfy its compatibility conditions along the trajectory; they need not fill the usual space $H$. The standard projection formula alone does not prove stationarity for that more restricted problem. Then

$$
\boxed{P_H\mathbf u^\dagger(0)=\lambda\mathbf u_0,\qquad
\frac12\|\mathbf u_0\|^2=E_0.}
$$

For the natural solenoidal adjoint space, $P_H\mathbf u^\dagger(0)=\mathbf u^\dagger(0)$. Equivalently, its component tangent to the [sphere in a normed vector space](../../../../../../sphere-in-a-normed-vector-space.md) of fixed [kinetic energy](../../../../../../kinetic-energy.md) vanishes:

$$
g_{\mathrm{tan}}=P_H\mathbf u^\dagger(0)
-\frac{(P_H\mathbf u^\dagger(0),\mathbf u_0)}{2E_0}\mathbf u_0=0.
$$

Here $E_0>0$ is needed for the [sphere in a normed vector space](../../../../../../sphere-in-a-normed-vector-space.md) to be regular and for division by $2E_0$. The multiplier is real and can have either sign; normalizing the initial adjoint with a prescribed positive sign is not a general necessary condition for minimization. If $E_0=0$, the only feasible initial [velocity](../../../../../../velocity.md) is zero and this tangent formula for the [sphere in a normed vector space](../../../../../../sphere-in-a-normed-vector-space.md) is inapplicable. First-order stationarity alone also allows maxima or saddles; a local minimum requires the appropriate nonnegative constrained second variation.

The spatial boundary terms vanish with periodic adjoints in $x,z$, homogeneous [no-slip boundary conditions](../../../../../../no-slip-boundary-condition.md) $\mathbf u^\dagger=0$ at $y=\pm1$, and $\partial_y\theta^\dagger=0$ there. To see this, [velocity](../../../../../../velocity.md) variations vanish at the wall while their normal [derivatives](../../../../../../derivative.md) need not, so the viscous boundary term forces the adjoint [velocity](../../../../../../velocity.md) to vanish. Scalar variations have zero normal [derivative](../../../../../../derivative.md) but free values, forcing the adjoint scalar's normal [derivative](../../../../../../derivative.md) to vanish. Pressure variation gives adjoint [incompressible flow](../../../../../../incompressible-flow.md); no independent terminal or initial datum is assigned to $p^\dagger$. Its additive time-dependent constant may be fixed by a zero spatial mean.

In particular, a homogeneous Neumann condition for the direct [pressure](../../../../../../pressure.md) does not by variational transposition require $\partial_yp^\dagger=0$. For a smooth adjoint solution, the wall-normal adjoint momentum equation instead supplies

$$
\partial_yp^\dagger=-\nu\Delta u_y^\dagger
$$

at the flat walls, because the direct scalar normal [derivative](../../../../../../derivative.md) is zero there. A zero adjoint-[pressure](../../../../../../pressure.md) [derivative](../../../../../../derivative.md) would be an additional compatibility choice, valid only when this right-hand side vanishes.

There are also literal direct-data compatibility qualifications in the printed setup. The initial total [scalar field](../../../../../../scalar-field.md) is $\overline\theta=-\operatorname{erf}(30y)$, whose wall [derivative](../../../../../../derivative.md) is $-60e^{-900}/\sqrt\pi\ne0$. It is extraordinarily small but mathematically not zero. Thus exact initial scalar data and exact zero wall flux are incompatible for a classical solution smooth at $t=0$. One may use a parabolic [mild solution of an abstract Cauchy problem](../../../../../../mild-solution-of-an-abstract-cauchy-problem.md) with the boundary condition enforced for $t>0$, or replace the initial profile by an exactly compatible smooth one; these are conventions, not an equality $e^{-900}=0$. The reference [scalar field](../../../../../../scalar-field.md) is also not a stationary profile of the [diffusion equation](../../../../../../diffusion-equation-split.md) at finite $Pe$: the full $\Delta\Theta$ term must be retained.

The [pressure compatibility at a no-slip wall](../../../../../../pressure-compatibility-at-a-no-slip-wall.md) is similarly important. Direct normal momentum gives $\partial_yp=\nu\Delta u_y-Ri_B\theta$. The separately imposed zero [pressure](../../../../../../pressure.md) [derivative](../../../../../../derivative.md) requires this right side to vanish. It is not automatic for arbitrary fixed-energy initial [velocities](../../../../../../velocity.md). For example, the divergence-free no-slip field generated by the periodic [stream function](../../../../../../stream-function.md) $S=A(1-y^2)^2\sin(\alpha x)$ with $\alpha=\pi/L_x>0$ has $u_x=\partial_yS$, $u_y=-\partial_xS$ and $\Delta u_y|_{y=\pm1}=-8A\alpha\cos(\alpha x)\ne0$, while $\theta(0)=0$. With $A\ne0$ adjusted to any positive energy, no classical solution smooth up to the initial wall can satisfy that extra [pressure](../../../../../../pressure.md) condition. The displayed adjoints are the formal necessary equations along admissible smooth trajectories; a well-posed physical formulation normally determines [pressure](../../../../../../pressure.md) from [incompressible flow](../../../../../../incompressible-flow.md) and normal momentum, rather than imposing independent homogeneous [pressure](../../../../../../pressure.md) flux for every control.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
