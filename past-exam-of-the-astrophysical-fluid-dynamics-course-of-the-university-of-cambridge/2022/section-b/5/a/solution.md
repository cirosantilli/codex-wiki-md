<h1 id="section-b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Rankine-Hugoniot conditions](../../../../../rankine-hugoniot-conditions.md) follow by integrating [conservation laws](../../../../../conservation-law.md) across a thin moving layer, then letting its macroscopic thickness tend to zero. For example, normal [momentum conservation](../../../../../momentum-conservation.md) in one dimension has the conservative form

$$
\partial_t(\rho u)+\partial_x(\rho u^2+p)=0.
$$

For a [shock wave](../../../../../shock-wave.md) moving at speed $V$, integrate over a control interval whose endpoints move with the discontinuity. The [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) gives

$$
\boxed{V[\rho u]=[\rho u^2+p],}
$$

where $[f]=f_R-f_L$ denotes the difference of limiting states. [Mass conservation](../../../../../mass-conservation.md) similarly gives $V[\rho]=[\rho u]$. If $v=u-V$ is the normal [velocity](../../../../../velocity.md) in the [shock frame](../../../../../shock-frame.md), combining the two relations yields

$$
\boxed{[\rho v]=0,\qquad[p+\rho v^2]=0.}
$$

The same construction applied to [conservation of energy](../../../../../conservation-of-energy.md), for a non-radiating [normal shock wave](../../../../../normal-shock-wave.md) with nonzero mass flux, gives $[h+v^2/2]=0$, where $h$ is the [specific enthalpy](../../../../../specific-enthalpy.md). An [equation of state](../../../../../equation-of-state.md) closes these relations, and the physical compression branch has increasing [entropy](../../../../../entropy-split.md).

Finite [dynamic viscosity](../../../../../dynamic-viscosity-split.md) replaces the ideal discontinuity by a thin smooth transition. A viscous [stress](../../../../../stress.md) contributes a derivative to the momentum flux inside the layer and converts directed [kinetic energy](../../../../../kinetic-energy.md) into internal [energy](../../../../../energy-split.md). If its gradients vanish in the uniform far states, the same limiting [Rankine-Hugoniot conditions](../../../../../rankine-hugoniot-conditions.md) still hold there. Balancing nonlinear transport with viscous diffusion gives a thickness of order $\nu/|u_L-u_R|$ in the [viscous Burgers equation](../../../../../viscous-burgers-equation.md), where $\nu$ is the [kinematic viscosity](../../../../../kinematic-viscosity.md).

## ↑ Ancestors (14)

1. [A](../a.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
