<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrating the radial [velocity](../../../../velocity.md) over the thickness gives the radial [volume flux per unit width](../../../../volume-flux-per-unit-width.md):

$$
q_r=\int_0^h v_r\,dz
=\frac{\rho gh_r+\gamma\kappa_r}{2\mu}
\left[\frac{h^3}{3}-h^3\right]
=-\frac{h^3}{3\mu}\left(\rho gh_r+\gamma\kappa_r\right).
$$

The full [volumetric flow rate](../../../../volumetric-flow-rate.md) across a cylindrical surface, positive outward, is

$$
\boxed{Q(r,t)=2\pi r q_r=-\frac{2\pi r h^3}{3\mu}\left(\rho gh_r+\gamma\kappa_r\right).}
$$

An annulus of radial thickness $dr$ contains [volume](../../../../volume.md) $2\pi rh\,dr$ to leading order. Its rate of gain equals incoming minus outgoing [volume flux](../../../../volumetric-flow-rate.md), so

$$
2\pi r h_t\,dr=Q(r,t)-Q(r+dr,t)=-Q_r\,dr+o(dr).
$$

Dividing and taking $dr\to0$ yields the axisymmetric [thin-film equation](../../../../thin-film-equation.md):

$$
\boxed{h_t=\frac1r\partial_r\left[\frac{rh^3}{3\mu}\left(\rho gh_r+\gamma\kappa_r\right)\right].}
$$

The equation assumes no evaporation or injection through the boundaries. Integrating it over the whole drop also verifies [conservation of mass](../../../../mass-conservation.md) when the edge carries zero [volume flux](../../../../volumetric-flow-rate.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
