<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathbf U_h=\Gamma z\,\mathbf u_h(x,y)$ denote the actual horizontal [velocity field](../../../../velocity-field.md). With constant nonzero [Coriolis parameter](../../../../coriolis-parameter.md) $f_0$, [geostrophic balance](../../../../geostrophic-balance.md) and [hydrostatic balance](../../../../hydrostatic-balance.md), using [pressure](../../../../pressure-split.md) per reference [density](../../../../density.md) $\pi$, give

$$
f_0\mathbf e_z\mathbin\times\mathbf U_h=-\nabla_h\pi,
\qquad \pi_z=b.
$$

Differentiate the first equation in $z$ to obtain [thermal-wind balance](../../../../thermal-wind.md):

$$
f_0\Gamma\mathbf e_z\mathbin\times\mathbf u_h=-\nabla_h b.
$$

Taking the [dot product](../../../../dot-product.md) with $\mathbf U_h$ proves

$$
\boxed{\mathbf U_h\cdot\nabla_h b=0.}
$$

Thus the horizontal [velocity](../../../../velocity.md) is tangent to the horizontal [buoyancy](../../../../buoyancy.md) contours at every height. For a fluid whose thermal [equation of state](../../../../equation-of-state.md) makes horizontal [buoyancy](../../../../buoyancy.md) contours coincide with horizontal [temperature](../../../../temperature-split.md) contours, there is no horizontal [advection](../../../../advection.md) across those contours. In a dry [terrestrial atmosphere](../../../../terrestrial-atmosphere.md), use [potential temperature](../../../../potential-temperature.md) as the materially conserved thermal variable. A salinity contribution to [buoyancy](../../../../buoyancy.md) would require separate treatment before interpreting the result as a statement about [temperature](../../../../temperature-split.md).

The usual statement about net meridional [heat transport](../../../../heat-transport.md) also follows explicitly. Introduce a horizontal [streamfunction](../../../../stream-function.md) $\Psi$ such that $\mathbf u_h=(-\Psi_y,\Psi_x)$. Integration of [thermal-wind balance](../../../../thermal-wind.md) gives

$$
b=f_0\Gamma\Psi+b_0(z),\qquad
v=\Gamma z\Psi_x,
$$

and hence

$$
vb=\partial_x\left[\Gamma z\left(\frac{f_0\Gamma}{2}\Psi^2+b_0\Psi\right)\right].
$$

For a zonally [periodic function](../../../../periodic-function.md) $\Psi$, or vanishing endpoint contributions, the zonal integral is zero. Likewise, the anomalous [eddy buoyancy flux](../../../../eddy-buoyancy-flux.md) is

$$
\boxed{\overline{v'b'}=f_0\Gamma^2z\,\overline{\Psi'_x\Psi'}=0.}
$$

The required correlation between meridional [velocity](../../../../velocity.md) and thermal anomaly is absent. A nonzero vertical [phase](../../../../phase-waves.md) tilt, as in the next part, permits that correlation.

**Qualification of the wording.** The result does not say that the local [heat flux](../../../../heat-flux-density.md) vector $b\mathbf U_h$ vanishes, or that an arbitrary open-domain integral vanishes without [boundary conditions](../../../../boundary-condition.md). For a concrete counterexample to that literal reading, take $\mathbf u_h=(0,1)$ and $b=f_0\Gamma x+N^2z$. These satisfy the displayed [thermal-wind balance](../../../../thermal-wind.md), but $vb=\Gamma z(f_0\Gamma x+N^2z)$ is generally nonzero. What the hypotheses alone guarantee is zero transport across horizontal [buoyancy](../../../../buoyancy.md) contours; the vanishing zonally integrated [heat transport](../../../../heat-transport.md) uses the stated endpoint condition.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
