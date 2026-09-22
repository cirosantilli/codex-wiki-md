<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The rest state is $\rho=\rho_0$, $p=p_0$, $\mathbf u=\mathbf0$. At [linear order](../../../../linear-order.md) in the perturbations, the [continuity equation](../../../../continuity-equation.md), [Euler momentum equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) and the given [equation of state](../../../../equation-of-state.md) become

$$
\rho'_t+\rho_0\nabla\cdot\mathbf u=0,\qquad
\rho_0\mathbf u_t=-\nabla p'=-c^2\nabla\rho'.
$$

For the acoustic component take $\mathbf u=\nabla\phi$. This is consistent with initially zero [vorticity](../../../../vorticity-split.md), since taking the [curl](../../../../curl.md) of the linear momentum equation gives $\partial_t(\nabla\times\mathbf u)=0$. Any pre-existing linear vortical component is time independent and is separate from the potential oscillations being sought.

Spatial integration of $\rho_0\nabla\phi_t=-c^2\nabla\rho'$ gives $\rho_0\phi_t+c^2\rho'=K(t)$. Adding a function of time to the [velocity potential](../../../../velocity-potential.md) removes $K(t)$ without altering the [velocity field](../../../../velocity-field.md). Hence

$$
\boxed{\rho'=-\frac{\rho_0}{c^2}\phi_t,\qquad p'=-\rho_0\phi_t.}
$$

Substitute the first relation into [mass conservation](../../../../mass-conservation.md):

$$
-\frac{\rho_0}{c^2}\phi_{tt}+\rho_0\nabla^2\phi=0.
$$

Thus the [velocity potential](../../../../velocity-potential.md) satisfies the [wave equation](../../../../wave-equation-split.md)

$$
\boxed{\phi_{tt}-c^2\nabla^2\phi=0.}
$$

Differentiating that equation in time and using the same density-potential relation gives

$$
\boxed{\rho'_{tt}-c^2\nabla^2\rho'=0.}
$$

Alternatively, differentiate the linear [continuity equation](../../../../continuity-equation.md) in time and take the [divergence](../../../../divergence.md) of the linear momentum equation. The coefficient $c$ is the [sound speed](../../../../speed-of-sound.md), since $dp/d\rho=c^2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
