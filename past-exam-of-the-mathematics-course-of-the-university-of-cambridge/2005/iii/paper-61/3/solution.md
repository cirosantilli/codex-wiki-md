<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [natural units](../../../../../natural-units.md) and the unreduced [Planck mass](../../../../../planck-mass.md) $M_P=G^{-1/2}$; it is $\sqrt{8\pi}$ times the [reduced Planck mass](../../../../../reduced-planck-mass.md). A homogeneous canonical [inflaton](../../../../../inflaton.md) has $\rho_\phi=\dot\phi^2/2+V$ and $P_\phi=\dot\phi^2/2-V$. [Vacuum domination by a scalar field](../../../../../vacuum-domination-by-a-scalar-field.md) requires $\dot\phi_i^2/2\ll V(\phi_i)$, with other matter and the curvature term negligible in the [Friedmann equation](../../../../../friedmann-equations.md). The [equation-of-state parameter](../../../../../equation-of-state-parameter.md) is then near $-1$, and the [Friedmann acceleration equation](../../../../../friedmann-acceleration-equation.md) gives [accelerating expansion](../../../../../accelerating-expansion-of-the-universe.md).

For sustained [slow-roll inflation](../../../../../slow-roll-approximation.md), [Hubble friction](../../../../../hubble-friction.md) must dominate the [inflaton](../../../../../inflaton.md) acceleration: $|\ddot\phi|\ll3H|\dot\phi|$, with the [scalar potential](../../../../../scalar-potential.md) changing only slightly in one [Hubble time](../../../../../hubble-time.md). In terms of the [potential slow-roll parameter](../../../../../potential-slow-roll-parameter.md) and [second potential slow-roll parameter](../../../../../second-potential-slow-roll-parameter.md), this requires

$$
\epsilon_V=\frac{M_P^2}{16\pi}\left(\frac{V'}V\right)^2\ll1,\qquad |\eta_V|=\left|\frac{M_P^2}{8\pi}\frac{V''}V\right|\ll1.
$$

For the quartic [scalar potential](../../../../../scalar-potential.md),

$$
\epsilon_V=\frac{M_P^2}{\pi\phi^2},\qquad \eta_V=\frac{3M_P^2}{2\pi\phi^2}.
$$

Thus $|\phi_i|\gg M_P$ supplies a broad [slow-roll](../../../../../slow-roll-approximation.md) range when $\lambda\ll1$. At an initial density of order the Planck density, potential domination gives

$$
\boxed{\phi_i^2\sim\frac{2M_P^2}{\sqrt\lambda},\qquad V_i\sim M_P^4,}
$$

so both [potential slow-roll parameters](../../../../../potential-slow-roll-parameter.md) are small for small $\lambda$. Small initial [kinetic energy](../../../../../kinetic-energy.md) is a separate condition; the height of the [scalar potential](../../../../../scalar-potential.md) alone does not enforce it. These classical equations describe the post-Planck evolution under the model assumptions, rather than resolving [quantum gravity](../../../../../quantum-gravity.md) at the initial endpoint.

Take $\phi_i>0$; the negative branch follows by the symmetry $\phi\mapsto-\phi$. Dropping [kinetic energy](../../../../../kinetic-energy.md) from the [Friedmann equation](../../../../../friedmann-equations.md) and acceleration from the [inflaton equation of motion](../../../../../inflaton-equation-of-motion.md) gives

$$
H\simeq\frac1{M_P}\sqrt{\frac{2\pi\lambda}{3}}\,\phi^2,\qquad 3H\dot\phi\simeq-\lambda\phi^3.
$$

Writing $b=M_P\sqrt{\lambda/(6\pi)}$, the [quartic-potential slow-roll solution](../../../../../quartic-potential-slow-roll-solution.md) is

$$
\boxed{\phi(t)\simeq\phi_i e^{-b(t-t_i)},\qquad a(t)\simeq a_i\exp\left[\frac{\pi\phi_i^2}{M_P^2}\left(1-e^{-2b(t-t_i)}\right)\right].}
$$

Indeed, $\dot\phi\simeq-b\phi$, and integrating $H=\dot a/a$ gives $\log(a/a_i)=\pi(\phi_i^2-\phi^2)/M_P^2$. These expressions apply during [slow-roll inflation](../../../../../slow-roll-approximation.md); their formal late-time saturation must not be used beyond the end of that approximation.

The exact end of [accelerating expansion](../../../../../accelerating-expansion-of-the-universe.md) is $\epsilon_H=-\dot H/H^2=1$, equivalently $\dot\phi^2=V$ for the scalar-dominated flat model. The [quartic-inflation endpoint estimate](../../../../../quartic-inflation-endpoint-estimate.md) uses the leading potential condition $\epsilon_V\simeq1$, giving

$$
\boxed{|\phi_e|\sim M_P,\qquad |\phi_e|\simeq\frac{M_P}{\sqrt\pi}\ \text{using }\epsilon_V=1.}
$$

The numerical coefficient is an endpoint estimate: the [slow-roll approximation](../../../../../slow-roll-approximation.md) breaks down there. Imposing $|\eta_V|=1$ estimates when slow roll loses accuracy and gives a different order-one coefficient, not a different exact acceleration condition.

The [slow-roll e-fold count](../../../../../slow-roll-e-fold-count.md) is

$$
N\simeq\frac{8\pi}{M_P^2}\int_{\phi_e}^{\phi_i}\frac{V}{V'}\,d\phi=\frac{\pi}{M_P^2}(\phi_i^2-\phi_e^2).
$$

The [quartic-inflation expansion from Planck density](../../../../../quartic-inflation-expansion-from-planck-density.md) combines this initial estimate with the conventional endpoint to give

$$
\boxed{N\sim\frac{2\pi}{\sqrt\lambda}-1,\qquad \frac{a_e}{a_i}\sim\exp\left(\frac{2\pi}{\sqrt\lambda}-1\right).}
$$

For small $\lambda$ the dominant term is enormous; the order-one endpoint uncertainty does not affect that conclusion.

To estimate the [reheating temperature](../../../../../reheating-temperature.md), assume prompt, efficient [reheating](../../../../../reheating.md) converts the end-of-inflation energy into a thermal radiation bath. With the same endpoint convention, $V_e\simeq\lambda M_P^4/(4\pi^2)$, and equating this to the radiation [energy density](../../../../../energy-density.md) gives

$$
\frac{\pi^2}{30}g_*T_R^4\sim\frac{\lambda M_P^4}{4\pi^2},\qquad \boxed{T_R\sim\left(\frac{15\lambda}{2\pi^4g_*}\right)^{1/4}M_P\sim\lambda^{1/4}g_*^{-1/4}M_P.}
$$

The [quartic-inflation prompt-reheating estimate](../../../../../quartic-inflation-prompt-reheating-estimate.md) fixes the scaling; the endpoint [kinetic energy](../../../../../kinetic-energy.md) changes the coefficient by order one. Without an inflaton coupling and its thermalization history, $V$ alone cannot specify the actual [reheating temperature](../../../../../reheating-temperature.md).

Finally, during [cosmic inflation](../../../../../cosmic-inflation-split.md) the [comoving Hubble radius](../../../../../comoving-hubble-radius.md) decreases:

$$
\frac d{dt}\frac1{aH}=-\frac{1-\epsilon_H}{a}<0.
$$

An initially causally connected patch is enlarged enough that the present observable region can lie within it. Its portions may subsequently be far outside one another's Hubble radii while retaining their common earlier thermal history. This solves the [horizon problem](../../../../../horizon-problem.md) if the [number of e-folds](../../../../../number-of-e-folds.md) is sufficiently large, conventionally of order sixty for the relevant thermal history; $N\sim2\pi/\sqrt\lambda$ can readily exceed that. The necessary count depends on [reheating](../../../../../reheating.md) and later expansion. The causal mechanism and the conversion back to a hot universe are discussed in [David Tong's account of inflation](https://www.davidtong.org/teaching/cosmology/cosmohtml/S1#S1.SS5).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
