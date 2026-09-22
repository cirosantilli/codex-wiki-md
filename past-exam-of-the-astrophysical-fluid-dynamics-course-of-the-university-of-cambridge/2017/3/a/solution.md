<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in the rest frame of a thin planar [shock wave](../../../../shock-wave.md), with normal upstream and downstream velocities $u_1,u_2>0$. Assume a steady flow, negligible gravitational change across its thickness, no radiative energy loss, and negligible viscous stress and heat flux at the two remote faces of a control volume. Dissipation within the shock is permitted and is essential to the physical discontinuity.

Integrating [mass conservation](../../../../mass-conservation.md) through that volume gives equal [mass flux](../../../../mass-flux.md) per unit area:

$$
\boxed{\rho_1u_1=\rho_2u_2=j.}
$$

The dimensions of $j$ are $\mathrm{kg\,m^{-2}\,s^{-1}}$. The normal momentum entering minus that leaving must balance the [pressure](../../../../pressure-split.md) forces. Equivalently, the conserved normal [momentum flux](../../../../momentum-flux.md) is $p+\rho u^2$, giving

$$
\boxed{p_1+\rho_1u_1^2=p_2+\rho_2u_2^2.}
$$

For [conservation of energy](../../../../conservation-of-energy.md), matter advects kinetic and internal energy while [pressure](../../../../pressure-split.md) performs work at rate $pu$ per unit area. Writing $\epsilon$ for [specific internal energy](../../../../specific-internal-energy.md), the [energy flux](../../../../energy-flux.md) is $\rho u(u^2/2+\epsilon)+pu$. With [specific enthalpy](../../../../specific-enthalpy.md) $h=\epsilon+p/\rho$, its conservation gives

$$
\boxed{\frac{u_1^2}{2}+h_1=\frac{u_2^2}{2}+h_2.}
$$

The division by $j$ is valid for a genuine through-flow shock. Together these are the three [Rankine-Hugoniot conditions](../../../../rankine-hugoniot-conditions.md). The conserved [energy flux](../../../../energy-flux.md) has units $\mathrm{W\,m^{-2}}$, and both momentum fluxes have units of [pressure](../../../../pressure-split.md).

For a calorically perfect [ideal gas](../../../../ideal-gas-split.md), $\epsilon=p/[(\gamma-1)\rho]$ and $h=\gamma p/[(\gamma-1)\rho]$. The three jump conditions can be combined explicitly. Put $r=\rho_2/\rho_1$, so $u_2=u_1/r$ and

$$
p_2=p_1+\rho_1u_1^2(1-r^{-1}).
$$

Substitute these into the enthalpy equation and use $\mathcal M_1^2=\rho_1u_1^2/(\gamma p_1)$, with the upstream [adiabatic sound speed](../../../../adiabatic-sound-speed.md). Besides the trivial no-shock root $r=1$, the physical compression root is

$$
\boxed{r=\frac{(\gamma+1)\mathcal M_1^2}{(\gamma-1)\mathcal M_1^2+2},\qquad
\frac{p_2}{p_1}=\frac{2\gamma\mathcal M_1^2-(\gamma-1)}{\gamma+1}.}
$$

For unchanged composition, $T_2/T_1=(p_2/p_1)/r$. A compressive shock has $\mathcal M_1>1$ and increases the [specific entropy](../../../../specific-entropy.md). Thus an adiabatic shock conserves total energy but is not an [isentropic process](../../../../isentropic-process.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
