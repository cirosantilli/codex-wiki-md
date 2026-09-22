<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the physical [magnetic field](../../../../magnetic-field-split.md) as $\mathbf B_{\rm phys}$ and use the constant [mass density](../../../../density.md) $\rho_0$ to introduce [Alfvén velocity](../../../../alfven-velocity.md) units, $\mathbf B=\mathbf B_{\rm phys}/\sqrt{\mu_0\rho_0}$. If $P$ is the fluid's mechanical [pressure](../../../../pressure-split.md), the [magnetohydrodynamic total pressure](../../../../magnetohydrodynamic-total-pressure.md) per unit [mass density](../../../../density.md) is $p=P/\rho_0+B^2/2$. The [ideal magnetohydrodynamic equations](../../../../ideal-magnetohydrodynamic-equations.md) then reduce to

$$
\boxed{
\begin{aligned}
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u
&=-\nabla p+(\mathbf B\cdot\nabla)\mathbf B,\\
\partial_t\mathbf B+(\mathbf u\cdot\nabla)\mathbf B
&=(\mathbf B\cdot\nabla)\mathbf u,\\
\nabla\cdot\mathbf u&=0,\qquad \nabla\cdot\mathbf B=0.
\end{aligned}}
$$

The first equation is [momentum conservation](../../../../momentum-conservation.md): the [magnetic pressure](../../../../magnetic-pressure.md) has been included in $p$, leaving [magnetic tension](../../../../magnetic-tension.md) explicitly. The second is the [ideal magnetohydrodynamic induction equation](../../../../ideal-magnetohydrodynamic-induction-equation.md), expressing [magnetic flux freezing](../../../../magnetic-flux-freezing.md). The last two equations impose [incompressibility](../../../../incompressible-flow.md) and the [solenoidal magnetic-field constraint](../../../../solenoidal-magnetic-field-constraint.md).

The model assumes a smooth conducting-fluid continuum with constant [mass density](../../../../density.md) and constant [magnetic permeability](../../../../permeability-electromagnetism.md), nonrelativistic [velocity](../../../../velocity.md), and scales on which a single-fluid description is appropriate. Negligible [electrical resistivity](../../../../electrical-resistivity.md) removes [magnetic diffusion](../../../../magnetic-diffusion.md); negligible [viscosity](../../../../dynamic-viscosity-split.md) removes viscous [momentum diffusion](../../../../momentum-diffusion.md). Equivalently, the [magnetic Reynolds number](../../../../magnetic-reynolds-number.md) and the [Reynolds number](../../../../reynolds-number.md) are large on the scales being retained. The low-frequency approximation neglects the [displacement current](../../../../displacement-current.md); Hall and other kinetic corrections to [Ohm's law](../../../../ohm-s-law.md) are absent. [Incompressibility](../../../../incompressible-flow.md) is an imposed approximation, commonly justified when the [Mach number](../../../../mach-number.md) is small. There is no independently evolved thermodynamic [pressure](../../../../pressure-split.md): $p$ enforces the [incompressibility condition](../../../../incompressible-flow.md). We omit external body forces; a conservative one could instead be absorbed into $p$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
