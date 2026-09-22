# Thermal equilibration of two finite bodies

↑ **Parent:** [Thermal equilibrium](thermal-equilibrium.md)

Consider two rigid bodies forming an [isolated system](isolated-system.md), with fixed composition and constant whole-body [heat capacity at constant volume](heat-capacity-at-constant-volume.md) values $C_1=1\,\mathrm{kJ\,K^{-1}}$ and $C_2=3\,\mathrm{kJ\,K^{-1}}$. Their initial [temperatures](temperature.md) are $T_{1,0}=300\,\mathrm K$ and $T_{2,0}=400\,\mathrm K$. Assume each body remains internally uniform, their contact stores negligible [energy](energy.md), no [phase transition](phase-transition.md) occurs and no [work](work.md) is done or extracted. These are stipulated model values, not material measurements.

Because $dU_i=C_i\,dT_i$, write $U_i=a_i+C_iT_i$ with arbitrary fixed reference constants $a_i$. The conserved relative [internal energy](internal-energy.md) is

$$
E=U_1+U_2-a_1-a_2=C_1T_1+C_2T_2=1500\,\mathrm{kJ}.
$$

This is an [energy](energy.md) reference convention, not a claim about actual [heat capacities](heat-capacity.md) down to zero [temperature](temperature.md). At [thermal equilibrium](thermal-equilibrium.md) the two [temperatures](temperature.md) equal $T_f$, so the [first law of thermodynamics](first-law-of-thermodynamics.md) gives

$$
T_f=\frac{C_1T_{1,0}+C_2T_{2,0}}{C_1+C_2}=375\,\mathrm K,\qquad
\Delta U_1=75\,\mathrm{kJ},\qquad \Delta U_2=-75\,\mathrm{kJ}.
$$

The larger [heat capacity](heat-capacity.md) pulls the common [temperature](temperature.md) closer to its initial value: body 1 warms by $75\,\mathrm K$, while body 2 cools by $25\,\mathrm K$.

<a id="image-two-finite-bodies-approach-thermal-equilibrium-at-375-mathrm-k"></a>
![](thermal-equilibrium-two-bodies.png)

**[Figure 23](#image-two-finite-bodies-approach-thermal-equilibrium-at-375-mathrm-k). Two finite bodies approach thermal equilibrium at $375\,\mathrm K$**. Ideal model with $C_1=1$ and $C_2=3\,\mathrm{kJ\,K^{-1}}$ and contact conductance $G=0.1\,\mathrm{kJ\,s^{-1}\,K^{-1}}$. The weighted [temperature](temperature.md) stays at $375\,\mathrm K$ and the relative [internal energy](internal-energy.md) stays at $1500\,\mathrm{kJ}$; the plotted curves are model predictions.

To predict a timescale, stipulate a constant contact conductance $G=1/R_{\rm th}=0.1\,\mathrm{kJ\,s^{-1}\,K^{-1}}$, the reciprocal of the contact's [thermal resistance](thermal-resistance.md). The rate of [heat transfer](heat-transfer.md) into body 1 is $G(T_2-T_1)$, giving

$$
C_1\dot T_1=G(T_2-T_1),\qquad C_2\dot T_2=-G(T_2-T_1).
$$

Adding proves conservation of $E$. Subtracting gives [exponential decay](exponential-decay.md) of the [temperature](temperature.md) difference, with [time constant](time-constant.md)

$$
\tau=\frac{C_1C_2}{G(C_1+C_2)}=7.5\,\mathrm s,\qquad
T_2-T_1=100\,\mathrm K\,e^{-t/\tau},
$$

and therefore

$$
T_1(t)=375\,\mathrm K-75\,\mathrm K\,e^{-t/\tau},\qquad
T_2(t)=375\,\mathrm K+25\,\mathrm K\,e^{-t/\tau}.
$$

Exact equality is approached as $t\to\infty$ in this ideal model. Changing $G$ changes the rate but not $T_f$: equilibrium and the speed of reaching it are separate predictions. Real bodies can have internal [temperature gradients](temperature-gradient.md), changing [heat capacities](heat-capacity.md) and contact losses, so the plotted $7.5\,\mathrm s$ is an assumed model timescale.

## ↑ Ancestors (6)

1. [Thermal equilibrium](thermal-equilibrium.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Entropy maximization under thermal contact](entropy-maximization-under-thermal-contact.md)
