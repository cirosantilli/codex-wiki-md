<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interstellar shocks arise when relative flow is supersonic: stellar winds, [supernova](../../../../supernova.md) ejecta, colliding clouds and gas moving through strong disturbances can drive them. Neighboring compressive [characteristics](../../../../characteristic-of-a-field.md) steepen or a fast flow encounters material it cannot decelerate through upstream sound communication. A thin dissipative front then converts directed [kinetic energy](../../../../kinetic-energy.md) into thermal [energy](../../../../energy-split.md) and increases [entropy](../../../../entropy-split.md).

Integrate [mass](../../../../mass.md), normal [momentum](../../../../momentum-split.md) and total [energy](../../../../energy-split.md) conservation through a planar steady shock in its rest frame. With no [mass](../../../../mass.md) source, negligible external impulse across the thin layer and no radiative [energy](../../../../energy-split.md) loss, their normal fluxes are respectively

$$
j=\rho u,\qquad p+\rho u^2,\qquad
j\left(h+\frac{u^2}{2}\right).
$$

For a [perfect gas](../../../../ideal-gas-split.md) of constant [adiabatic index](../../../../heat-capacity-ratio.md), $h=\gamma p/[(\gamma-1)\rho]$. Equality of the fluxes on the two sides yields the three [Rankine-Hugoniot conditions](../../../../rankine-hugoniot-conditions.md) in the question. Adiabatic means no [energy](../../../../energy-split.md) escapes this control [volume](../../../../volume.md); it does not make the shock isentropic.

In the strong-shock limit, let $r=\rho_2/\rho_1=u_1/u_2$ and neglect $p_1$. [Momentum](../../../../momentum-split.md) conservation gives $p_2=\rho_1u_1^2(1-1/r)$. Substitution into [energy](../../../../energy-split.md) conservation gives

$$
\frac{2\gamma}{\gamma-1}(r-1)+1=r^2,
\qquad
(r-1)\left(r-\frac{\gamma+1}{\gamma-1}\right)=0.
$$

The nontrivial compressive root is

$$
\boxed{\frac{\rho_2}{\rho_1}=\frac{u_1}{u_2}=\frac{\gamma+1}{\gamma-1}.}
$$

The $r=1$ root describes no shock. A [monatomic gas](../../../../monatomic-gas.md) has the familiar compression four.

For identical colliding clouds in their center-of-momentum frame, [reflection symmetry](../../../../reflection-symmetry.md) fixes the contact plane and the uniform compressed material on either side at rest. The unshocked clouds still approach at speeds $\pm V$; their supersonic upstream flow has not received a smooth [pressure](../../../../pressure-split.md) adjustment ahead of the shock. Let the right shock move to the right at speed $S$. In its own frame the upstream and downstream normal speed magnitudes are $V+S$ and $S$. The same [shock compression ratio](../../../../shock-compression-ratio.md) therefore gives

$$
\frac{V+S}{S}=\frac{\gamma+1}{\gamma-1},\qquad
\boxed{S=\frac{\gamma-1}{2}V.}
$$

This is the [shock speed in a symmetric cloud collision](../../../../shock-speed-in-a-symmetric-cloud-collision.md). For $\gamma=5/3$, the shocks move outward at $V/3$, not at the upstream speed or the relative cloud speed $2V$. As a check, the post-shock [pressure](../../../../pressure-split.md) is $p_2=(\gamma+1)\rho_1V^2/2$; in the monatomic case $p_2/\rho_2=V^2/3$, giving specific internal [energy](../../../../energy-split.md) $V^2/2$, exactly the initial bulk [kinetic energy](../../../../kinetic-energy.md) per unit cloud [mass](../../../../mass.md) when brought to rest.

<a id="3/image-symmetric-cloud-collision-stationary-compressed-gas-and-two-outward-moving-shocks"></a>
![](../../../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1-symmetric-cloud-shocks.png)

**[Figure 3](#3/image-symmetric-cloud-collision-stationary-compressed-gas-and-two-outward-moving-shocks). Symmetric cloud collision: stationary compressed gas and two outward-moving shocks**.

When a shock reaches a cloud's rear boundary, its supply of cold upstream gas ends. If the surrounding [pressure](../../../../pressure-split.md) is low, the hot compressed gas expands outward and a rarefaction travels back into it, converting thermal [energy](../../../../energy-split.md) into motion and cooling the gas. A sustained uniform stationary shocked region is no longer the solution. Interaction with an appreciable exterior medium can instead drive another outward disturbance; the boundary [pressure](../../../../pressure-split.md) determines that part of the evolution. The stated adiabatic model provides no radiative mechanism that would keep a permanently cold dense sheet at the contact.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
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
