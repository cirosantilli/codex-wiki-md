<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $K$ be intrinsic [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md), $\phi$ the mobile pore fraction, and let $h$ measure thickness normal to the sloping cap. Define cold and reservoir-temperature properties by

$$
\begin{aligned}
\rho_c&=\rho_w-\Delta\rho+\alpha\Delta T,&\delta_c&=\rho_w-\rho_c=\Delta\rho-\alpha\Delta T, &\mu_c&=\mu_0+\lambda\Delta T,\\
\rho_h&=\rho_w-\Delta\rho,&\delta_h&=\Delta\rho,&\mu_h&=\mu_0.
\end{aligned}
$$

The imposed inequality makes $\delta_c>0$, so the cold fluid is still buoyant. Assume $K>0$, $\sin\theta>0$, positive densities and viscosities, and the usual positive thermal-expansion and [viscosity](../../../../../dynamic-viscosity.md) coefficients. Away from localized fronts, neglect the along-current thickness gradient. Hydrostatic water pressure and [Darcy's law](../../../../../darcy-law.md) then give the upslope [Darcy velocities](../../../../../darcy-velocity.md)

$$
\boxed{u_c=\frac{K\delta_cg\sin\theta}{\mu_c},\qquad
u_h=\frac{K\delta_hg\sin\theta}{\mu_h}.}
$$

Typically $u_h>u_c$: warming increases [buoyancy](../../../../../buoyancy.md) and decreases [dynamic viscosity](../../../../../dynamic-viscosity.md).

**Current depths and the moving [moving thermal front in a porous current](../../../../../moving-thermal-front-in-a-porous-current.md).** For this [slope-driven porous gravity current](../../../../../slope-driven-porous-gravity-current.md), the injected [mass flux](../../../../../mass-flux.md) per unit well length fixes the cold plateau thickness:

$$
\boxed{h_c=\frac{Q}{\rho_cu_c}=\frac{Q\mu_c}{\rho_cK\delta_cg\sin\theta}.}
$$

The [moving thermal front in a porous current](../../../../../moving-thermal-front-in-a-porous-current.md) moves at $V_T=\Gamma u_c$. Since $u_c$ is explicitly a [Darcy velocity](../../../../../darcy-velocity.md), the fluid mass stored per unit horizontal area is $\phi\rho h$. Apply [mass conservation](../../../../../mass-conservation.md) across the moving [moving thermal front in a porous current](../../../../../moving-thermal-front-in-a-porous-current.md):

$$
\rho_h(u_h-\phi V_T)h_h=\rho_c(u_c-\phi V_T)h_c.
$$

Writing $\gamma=\phi\Gamma$ and $r=u_c/u_h$, this gives the distal warm depth

$$
\boxed{h_h=\frac{Q(1-\gamma)}{\rho_h(u_h-\gamma u_c)}
=\frac{Q}{\rho_hu_h}\frac{1-\gamma}{1-\gamma r}.}
$$

For a retarded [moving thermal front in a porous current](../../../../../moving-thermal-front-in-a-porous-current.md) take $0\leq\gamma<1$; otherwise this two-plateau geometry needs reconsideration. The factor $(1-\gamma)/(1-\gamma r)$ is important: the distal [mass flux](../../../../../mass-flux.md) is not generally $Q$, because mass is being stored as the cold region replaces the warm region. Setting the two fluxes equal would silently assume a stationary [moving thermal front in a porous current](../../../../../moving-thermal-front-in-a-porous-current.md).

If the model absorbs [porosity](../../../../../porosity.md) into storage and uses [pore velocity](../../../../../pore-velocity.md) as its transport speed, the same formulas use $\gamma=\Gamma$. The explicit Darcy convention in the PDF instead gives $\gamma=\phi\Gamma$; [porosity](../../../../../porosity.md) must be specified or absorbed consistently. In the stationary-front limit $\gamma=0$, the two steady depths reduce to $Q/(\rho_cu_c)$ and $Q/(\rho_hu_h)$. In the [Boussinesq approximation](../../../../../boussinesq-approximation.md), use a common reference density in the mass factors while retaining $\delta_c,\delta_h$ in the driving force.

**Leakage thresholds.** A normal thickness $h_i$ generates cap overpressure $\Pi_i=\delta_i g h_i\cos\theta$. Before leakage modifies the current, the two plateau values are

$$
\Pi_c=\frac{Q\mu_c\cot\theta}{\rho_cK},\qquad
\Pi_h=\frac{Q\mu_h\cot\theta}{\rho_hK}\frac{1-\gamma}{1-\gamma r}.
$$

For the [caprock leakage threshold](../../../../../caprock-leakage-threshold.md) $\Delta p>0$, the candidate critical mass-injection rates are therefore

$$
\boxed{Q_c^*=\frac{\Delta p\,\rho_cK\tan\theta}{\mu_c},\qquad
Q_h^*=\frac{\Delta p\,\rho_hK\tan\theta}{\mu_h}
\frac{1-\gamma r}{1-\gamma}.}
$$

Cold-only leakage occurs for $Q_c^*\leq Q<Q_h^*$, provided $Q_c^*<Q_h^*$. Both plateaus can leak once $Q\geq\max(Q_c^*,Q_h^*)$. In the usual common-density approximation, $\mu_c>\mu_h$ and $r<1$ ensure $Q_c^*<Q_h^*$, giving the expected sequence: no leakage, cold-only leakage, then leakage from both cold and warm regions. Without that approximation the ordering must be checked; the given inequality $\Delta\rho>\alpha\Delta T$ alone does not establish it. These are onset criteria computed on the nonleaking current, not a post-leakage mass budget.

For small slopes $\cos\theta\simeq1$ and $\tan\theta\simeq\sin\theta\simeq\theta$. If another thickness convention is used, its hydrostatic column and projected flux must be changed consistently; one should not mix a normal thickness with a vertical-pressure formula lacking the cosine.

**Cross-current [heat conduction](../../../../../thermal-conduction.md).** Heat transfer from the warm formation makes temperature vary across the [carbon dioxide](../../../../../carbon-dioxide.md) depth and introduces a warming time controlled by thickness, thermal diffusivity and the surrounding rock's heat capacity. It smooths the sharp thermal adjustment and causes gradual changes in [buoyancy](../../../../../buoyancy.md), [viscosity](../../../../../dynamic-viscosity.md) and the velocity profile. The cold fluid generally warms, becomes more mobile and requires less depth to carry a prescribed [mass flux](../../../../../mass-flux.md); the enhanced cold-region overpressure and its distinct leakage zone tend to shrink. Warming may occur before a parcel reaches the idealized advective [moving thermal front in a porous current](../../../../../moving-thermal-front-in-a-porous-current.md), especially for a thin current. A single supplied $\Gamma$ no longer describes all heat transport. Quantitative depths and thresholds then require a coupled temperature equation and thermal boundary data; their exact changes cannot be inferred from the linear property laws alone.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
