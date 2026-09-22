<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [instantaneous recycling approximation](../../../../../instantaneous-recycling-approximation.md) with a well-mixed gas reservoir, constant [stellar yield](../../../../../stellar-yield.md) $p$, no gas inflow, and an irreversible [galactic outflow](../../../../../galactic-outflow.md). Let $M_s$ be the mass locked into long-lived stars and remnants after prompt recycling, and put $\psi(t)=\dot M_s(t)\geq0$. The yield $p$ is the newly synthesized mass of heavy elements returned to the gas per unit increase of $M_s$. Thus $M_h$ in $Z=M_h/M_g$ denotes the heavy-element mass in the gas, excluding metals already locked into stars.

Assume $M_s(0)=0$, $M_g(0)=M_0$, and $Z(0)=Z_0$; initially pristine gas means $Z_0=0$. Take the outflow rate to be $\alpha\psi$ with constant $\alpha\geq0$, and assume its metallicity equals the current [gas-phase metallicity](../../../../../gas-phase-metallicity.md) $Z$. This is the well-mixed [leaky-box model of galactic chemical evolution](../../../../../leaky-box-model-of-galactic-chemical-evolution.md). The parameter $\alpha$ is a [mass-loading factor](../../../../../mass-loading-factor.md) relative to the net rate of locking mass into stars. If a gross [star formation rate](../../../../../star-formation-rate.md) $\Psi$ and a prompt returned fraction $\mathscr R$ are used instead, $\psi=(1-\mathscr R)\Psi$ and a wind rate $\eta\Psi$ corresponds to $\alpha=\eta/(1-\mathscr R)$.

[Conservation of mass](../../../../../mass-conservation.md) gives

$$
\dot M_g=-(1+\alpha)\psi,
\qquad
M_g(t)=M_0-(1+\alpha)M_s(t),
$$

and the baryonic mass remaining in the box is $M_g+M_s=M_0-\alpha M_s$. Newly made metals enter the gas at rate $p\psi$, while pre-existing metals are locked into stars at rate $Z\psi$ and leave in the wind at rate $\alpha Z\psi$. Hence

$$
\frac{dM_h}{dt}=[p-(1+\alpha)Z]\psi.
$$

Using $M_h=ZM_g$ and the product rule,

$$
M_g\dot Z+Z\dot M_g=[p-(1+\alpha)Z]\psi
\quad\Longrightarrow\quad
\boxed{\dot Z=\frac{p\psi}{M_g}.}
$$

The cancellation expresses the fact that a well-mixed wind removes gas and metals in the same proportion, while fresh stellar production raises the abundance in the remaining gas.

Divide this equation by $\dot M_g=-(1+\alpha)\psi$ along the evolving reservoir, or integrate in time through intervals with no [star formation](../../../../../star-formation.md). The resulting [gas-phase metallicity](../../../../../gas-phase-metallicity.md) is

$$
\boxed{Z(t)=Z_0+\frac{p}{1+\alpha}\ln\frac{M_0}{M_g(t)}
=Z_0+\frac{p}{1+\alpha}\ln\left[\frac1{1-(1+\alpha)M_s(t)/M_0}\right].}
$$

Equivalently, its fully explicit dependence on a prescribed net [star formation rate](../../../../../star-formation-rate.md) is

$$
Z(t)=Z_0+\frac{p}{1+\alpha}
\ln\left[\frac{M_0}{M_0-(1+\alpha)\int_0^t\psi(t')\,dt'}\right],
$$

valid while $M_g(t)>0$. With pre-existing stars, replace $M_s(t)$ in the gas-mass relation by $M_s(t)-M_s(0)$. Without specifying $\psi(t)$ or a gas-consumption law, the model fixes $Z$ as a function of gas mass but does not determine a unique function of time.

For the [closed-box model of galactic chemical evolution](../../../../../closed-box-model-of-galactic-chemical-evolution.md), set $\alpha=0$. Then $M_g=M_0-M_s$ and

$$
\boxed{Z_{\rm closed}=Z_0+p\ln\frac{M_0}{M_g}.}
$$

At the same remaining fraction $g=M_g/M_0$ of the initial gas reservoir, the leaky box has the logarithmic coefficient $p/(1+\alpha)$, lower than the true [stellar yield](../../../../../stellar-yield.md) by the wind factor. This coefficient is often called an [effective yield](../../../../../effective-yield.md), but the definition of the gas fraction must be specified.

In particular, the observable [gas fraction of a galaxy](../../../../../gas-fraction-of-a-galaxy.md) is often $\mu=M_g/(M_g+M_s)$, using the mass still present, rather than $g$. In our initially star-free model,

$$
\mu=\frac{(1+\alpha)g}{1+\alpha g},\qquad
g=\frac{\mu}{1+\alpha(1-\mu)}.
$$

Therefore

$$
\boxed{Z_{\rm leaky}(\mu)=Z_0+\frac{p}{1+\alpha}
\ln\left[\frac{1+\alpha(1-\mu)}\mu\right],\qquad
Z_{\rm closed}(\mu)=Z_0+p\ln\frac1\mu.}
$$

For $0<\mu<1$ and $\alpha>0$, the leaky-box enrichment is smaller at the same $\mu$: $\ln[1+\alpha(1-\mu)]\leq\alpha(1-\mu)<\alpha\ln(1/\mu)$. If [effective yield](../../../../../effective-yield.md) is defined observationally as $(Z-Z_0)/\ln(1/\mu)$, it is consequently not simply the constant $p/(1+\alpha)$ at all $\mu$.

As an explicit time example, choose a [linear gas-consumption law](../../../../../linear-gas-consumption-law.md) $\psi=\epsilon M_g$, with constant $\epsilon>0$. The mass and metallicity equations give

$$
M_g=M_0e^{-(1+\alpha)\epsilon t},\qquad
M_s=\frac{M_0}{1+\alpha}\left(1-e^{-(1+\alpha)\epsilon t}\right),\qquad
\boxed{Z(t)=Z_0+p\epsilon t.}
$$

The closed box with the same $\epsilon$ has the same metallicity at a given time, while the leaky box exhausts its gas faster. Thus a comparison at fixed time depends on the chosen [star formation rate](../../../../../star-formation-rate.md), even though the comparison at fixed gas fraction above is unambiguous.

Finally, the assumption about wind metallicity is essential. If the expelled gas has abundance $Z_w$ instead, its metal-loss rate is $\alpha Z_w\psi$, and the same bookkeeping yields

$$
M_g\dot Z=[p+\alpha(Z-Z_w)]\psi.
$$

A wind enriched relative to the ambient gas lowers the enrichment rate; the logarithmic solution derived above applies to $Z_w=Z$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
