<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a [conforming finite element space](../../../conforming-finite-element-space.md) $V_h\subset H_0^1(\Omega)$ with the prescribed [basis](../../../basis.md), and write $u_h(x,y,t)=\sum_jU_j(t)\phi_j(x,y)$. Testing the [advection-diffusion equation](../../../advection-diffusion-equation.md) by $\phi_i$ and applying [integration by parts](../../../integration-by-parts.md) to its diffusion term gives

$$
\sum_j\left(\int_\Omega\phi_j\phi_i\right)\dot U_j
=\sum_j\left[\int_\Omega\phi_i(\partial_x\phi_j+\partial_y\phi_j)-\int_\Omega\nabla\phi_i\cdot\nabla\phi_j\right]U_j.
$$

Thus

$$
\boxed{M\dot U=PU,\quad M_{ij}=\int_\Omega\phi_i\phi_j,\quad
P_{ij}=\int_\Omega\phi_i(\partial_x\phi_j+\partial_y\phi_j)-\int_\Omega\nabla\phi_i\cdot\nabla\phi_j.}
$$

Here $M$ is the [mass matrix](../../../mass-matrix.md); it is a [symmetric positive-definite matrix](../../../symmetric-positive-definite-matrix.md) because the [basis](../../../basis.md) is [linearly independent](../../../linear-independence.md). The initial vector represents the chosen finite element approximation to $g$, for example its [orthogonal projection](../../../orthogonal-projection.md).

For any coefficient vector $U$, put $v_h=\sum_jU_j\phi_j$. The [skew symmetry of Galerkin advection](../../../skew-symmetry-of-galerkin-advection.md) with constant drift $(1,1)$ gives

$$
\int_\Omega v_h(\partial_xv_h+\partial_yv_h)
=\frac12\int_{\partial\Omega}v_h^2(n_x+n_y)=0
$$

because the [Sobolev trace](../../../trace-operator.md) of $v_h$ vanishes. Consequently

$$
\boxed{U^TPU=-\int_\Omega|\nabla v_h|^2\leq0.}
$$

Along the solution, $\int_\Omega u_h^2=U^TMU$. The constant [symmetric matrix](../../../symmetric-matrix.md) $M$ and the semidiscrete equations therefore give

$$
\boxed{\frac d{dt}\int_\Omega u_h^2=2U^TM\dot U=2U^TPU=-2\int_\Omega|\nabla u_h|^2\leq0.}
$$

The [L2 norm](../../../l2-norm.md) of the spatial finite element solution is nonincreasing. The constant drift transports it without changing this energy; the diffusion term dissipates it. Any subsequent [time-stepping method](../../../time-stepping-method.md) must be chosen to preserve an appropriate discrete stability estimate.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2011](../../2011-split.md)
3. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../split.md)
4. [Finite element methods for partial differential equations course of the University of Oxford](../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
