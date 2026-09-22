<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the well-mixed [natural ventilation](../../../../../natural-ventilation.md) model for a distributed floor source. Let the building height be $H_b$, its volume be $\mathcal V$, its [temperature](../../../../../temperature.md) excess be $\theta$, and the exterior [mass density](../../../../../density.md) be $\rho$. Let $\alpha_T$ be the [coefficient of thermal expansion](../../../../../coefficient-of-thermal-expansion.md), so [reduced gravity](../../../../../reduced-gravity-split.md) is $g'=g\alpha_T\theta$. Convert the total [heat](../../../../../heat.md) input $Q$ to the temperature-volume flux $\mathcal H=Q/(\rho c_p)$, where $c_p$ is [specific heat capacity](../../../../../specific-heat-capacity.md). If the quoted [heat](../../../../../heat.md) flux is per floor area, first multiply it by that area.

For [effective opening area for pressure-driven ventilation](../../../../../effective-opening-area-for-pressure-driven-ventilation.md), define the equal-opening hydraulic coefficient $K_A$ such that the signed throughflow $q$ obeys $q|q|=K_A\Pi$, with $\Pi$ the total driving [pressure](../../../../../pressure.md) divided by [mass density](../../../../../density.md). In the effective-area convention of question 6, each opening has discharge $A\sqrt{\delta p/\rho}$, so $K_A=A^2/2$. The usual physical-area orifice law instead gives $K_A=C_d^2A^2$; that prefactor does not affect the stability conclusions.

Set $W=\Delta P/\rho>0$ and $G_T=g\alpha_T H_b$. Positive $q$ denotes entry at the floor and exit at the roof. [hydrostatic pressure](../../../../../hydrostatic-pressure.md) and wind combine to give

$$
q|q|=K_A(G_T\theta+W)\quad\text{for assisting wind},\qquad
q|q|=K_A(G_T\theta-W)\quad\text{for opposing wind}.
$$

Because the inflowing air is at exterior [temperature](../../../../../temperature.md) in either direction, the [heat](../../../../../heat.md) budget is

$$
\mathcal V\dot\theta=\mathcal H-|q|\theta.
$$

The [well-mixed ventilation temperature balance](../../../../../well-mixed-ventilation-temperature-balance.md) at steady state is therefore

$$
\boxed{\theta^2(G_T\theta+W)=\frac{\mathcal H^2}{K_A}\quad\text{(assisting)},\qquad
\theta^2|G_T\theta-W|=\frac{\mathcal H^2}{K_A}\quad\text{(opposing)}}.
$$

All roots must satisfy $\theta>0$ and their appropriate flow-direction inequality; squaring a [pressure](../../../../../pressure.md) relation without imposing those conditions could add spurious branches.

The assisting case has a unique positive solution and it is stable. For opposing wind, define $\theta_w=W/G_T$. There is always one solution with $\theta>\theta_w$, a buoyancy-dominated upward flow. Below $\theta_w$, the heat-removal curve is $R(\theta)=\sqrt{K_A}\theta\sqrt{W-G_T\theta}$. It is zero at both endpoints, and its maximum occurs at $\theta=2\theta_w/3$:

$$
\boxed{R_{\max}=\frac{2\sqrt{K_A}W^{3/2}}{3\sqrt3\,G_T}}.
$$

For $0<\mathcal H<R_{\max}$ there are two downward-flow roots as well as the upward-flow root. Equivalently, setting $y=G_T\theta/W$ and $\varepsilon=G_T\mathcal H/(\sqrt{K_A}W^{3/2})$, the equilibrium curve is

$$
\boxed{y\sqrt{|y-1|}=\varepsilon,\qquad 0<\varepsilon<\frac{2}{3\sqrt3}}.
$$

For [linear stability analysis](../../../../../linear-stability.md) of the [opposing-wind ventilation bistability](../../../../../opposing-wind-ventilation-bistability.md), linearize the [heat](../../../../../heat.md) budget: the eigenvalue is $-R'(\theta)/\mathcal V$. The cooler downward root has $0<\theta<2\theta_w/3$ and $R'>0$, so it is stable. The warmer downward root has $2\theta_w/3<\theta<\theta_w$ and $R'<0$, so it is unstable and separates the two basins. The upward root has $R'>0$ and is stable. At $\mathcal H=R_{\max}$ the two downward roots merge at a [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md); above that value only the upward equilibrium remains.

For [ventilation switching under wind and heating changes](../../../../../ventilation-switching-under-wind-and-heating-changes.md), increasing wind [pressure](../../../../../pressure.md) or decreasing [heat](../../../../../heat.md) input both reduce $\varepsilon$, so both can create the pair of wind-driven equilibria. They nevertheless have different physical and transient effects. On the hot upward branch, implicit differentiation of $\mathcal H=\sqrt{K_A}\theta\sqrt{G_T\theta-W}$ shows that increasing $W$ increases $\theta$, while decreasing $\mathcal H$ decreases $\theta$. Both reduce the upward ventilation rate, but only a wind change shifts $\theta_w$.

Under slow parameter variation, a state follows its current stable branch while that branch persists; the upward branch does not disappear when wind increases or heating decreases. A sufficiently large abrupt wind increase can raise $\theta_w$ beyond the current [temperature](../../../../../temperature.md) and place that state below the new unstable threshold, causing flow reversal and cooling towards the wind-dominated equilibrium. A jump insufficient to cross its basin boundary returns to the upward equilibrium.

At fixed $W$, reducing a still-positive [heat](../../../../../heat.md) input cannot force an initially upward-flow state through $\theta_w$: at that boundary the [temperature](../../../../../temperature.md) balance has $\dot\theta=\mathcal H/\mathcal V>0$. Thus [heat](../../../../../heat.md) reduction alone does not cause that reversal in this model. Conversely, decreasing wind or increasing [heat](../../../../../heat.md) from the stable downward branch eventually destroys it at the fold and forces a switch to the upward branch, giving history dependence. **Wind strengthening and [heat](../../../../../heat.md) reduction have the same effect on the steady dimensionless control parameter, but not the same [temperature](../../../../../temperature.md) change or switching dynamics.** These stability statements use quasi-steady opening flow and a single well-mixed [temperature](../../../../../temperature.md); other stratification or airflow-inertia models require their own stability analysis.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
