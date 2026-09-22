<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\theta=T-T_e$ and use the [Boussinesq approximation](../../../../../boussinesq-approximation.md) for air, $\rho_e-\rho\simeq\rho\theta/T_e$. A uniformly heated, well-mixed room has the buoyancy pressure difference $\Delta p_b=\rho gH\theta/T_e$ between its openings. Let $C_o$ denote the combined hydraulic coefficient of the two equal openings, so the [effective opening area for pressure-driven ventilation](../../../../../effective-opening-area-for-pressure-driven-ventilation.md) gives

$$
V=C_oA\sqrt{\frac{gH\theta}{T_e}}.
$$

For example, if each orifice has conventional discharge coefficient $C_d$ in $V=C_dA\sqrt{2\Delta p/\rho}$, the two pressure losses add and $C_o=C_d$. The question's coefficient is the prefactor in the final heat-load law; define $c=(2C_o^2)^{1/3}$. This explicitly states the numerical loss-coefficient convention. Steady [heat](../../../../../heat.md) balance is $Q=\rho C_pV\theta$. Eliminating $\theta$ gives

$$
\boxed{V_0=cA^{2/3}\left(\frac{gHQ}{2\rho C_pT_e}\right)^{1/3},\qquad
\theta_0=\frac{Q}{\rho C_pV_0}.}
$$

Here $Q$ is total heating power and $C_p$ is [specific heat capacity at constant pressure](../../../../../specific-heat-capacity-at-constant-pressure.md). Writing $c=C_d$ without this conversion would incorrectly change the power of the discharge coefficient.

After the reduction, cooler newly heated air occupies the bottom and displaces the old warmer air upward. Use the ideal two-layer [displacement ventilation](../../../../../displacement-ventilation.md) model: each layer is well mixed, the upper layer remains at $\theta_0$, walls have negligible heat capacity, and the sharp interface is advected without exchange between the layers. Let the lower layer have depth $h$ and excess temperature $\theta$. Integrating the hydrostatic [buoyancy](../../../../../buoyancy.md) over the full height gives

$$
\Delta p_b=\frac{\rho g}{T_e}\{h\theta+(H-h)\theta_0\},
\qquad
\boxed{V=C_oA\left[\frac g{T_e}\{h\theta+(H-h)\theta_0\}\right]^{1/2}.}
$$

The room's excess thermal energy is $E_T=\rho C_pA_r[h\theta+(H-h)\theta_0]$. The floor supplies $\lambda Q$, incoming air has zero excess temperature, and the ceiling removes $\rho C_pV\theta_0$. Thus the required [heat](../../../../../heat.md) balance is

$$
\boxed{\rho C_pA_r\frac d{dt}[h(\theta-\theta_0)]=-\rho C_pV\theta_0+\lambda Q.}
$$

This moving-interface energy term must include the loss of old upper-layer volume; balancing only the lower-layer temperature would miss it.

For a genuine reduction assume $0<\lambda<1$. Set

$$
s=\frac{V_0t}{A_rH},\qquad \eta=\frac hH,\qquad x=\eta\left(1-\frac\theta{\theta_0}\right).
$$

The integrated buoyancy factor is $H\theta_0(1-x)$, so $V/V_0=\sqrt{1-x}$. Since $Q=\rho C_pV_0\theta_0$, the thermal balance becomes the [ventilation after a heating reduction](../../../../../ventilation-after-a-heating-reduction.md) equation

$$
\boxed{\frac{dx}{ds}=\sqrt{1-x}-\lambda,\qquad x(0)=0.}
$$

The material interface also moves with the upward displacement velocity, $A_r\dot h=V$. Therefore $\eta_s=\sqrt{1-x}$, and subtracting the two equations gives

$$
\boxed{\eta=x+\lambda s,\qquad \eta\frac\theta{\theta_0}=\lambda s.}
$$

The second relation is also the lower-layer energy balance: its total excess energy increases at rate $\lambda Q$. It does not assume its temperature stays constant. Since $x_s>0$ until $x=1-\lambda^2$, the solution remains $0\leq x<1-\lambda^2$, and $V/V_0\geq\lambda$. Hence $\eta_s\geq\lambda$, so the lower layer reaches $\eta=1$ in finite time $s_H\leq1/\lambda$. Also $\eta_s\leq1$, so $s_H\geq1$.

An explicit implicit solution is useful. Put $y=\sqrt{1-x}$, which decreases from $1$ toward $\lambda$. Separation gives

$$
s=2(1-y)+2\lambda\log\frac{1-\lambda}{y-\lambda}.
$$

Filling occurs when $1=1-y_H^2+\lambda s_H$, so $\lambda s_H=y_H^2$ and $\theta_H/\theta_0=y_H^2$. These relations determine the exit time and the continuous temperature at that time. For complete switch-off $\lambda=0$, the limiting solution is $y=1-s/2$, $x=\eta=s-s^2/4$ for $0\leq s\leq2$, so the cold lower layer fills the room at $s_H=2$ even though its final ventilation rate is zero.

After the interface exits, the whole room is well mixed. For $z=\theta/\theta_0$, the [natural ventilation](../../../../../natural-ventilation.md) rate is $V=V_0\sqrt z$, and the [well-mixed ventilation temperature balance](../../../../../well-mixed-ventilation-temperature-balance.md) becomes

$$
\boxed{\frac{dz}{ds}=\lambda-z^{3/2},\qquad z(s_H)=y_H^2.}
$$

Equivalently, $\rho C_pA_rH\dot\theta=\lambda Q-\rho C_pC_oA\sqrt{gH/T_e}\,\theta^{3/2}$. The heat-removal term is strictly increasing in $\theta\geq0$, so every nonnegative solution tends to the unique stable equilibrium

$$
\boxed{T_\infty=T_e+\lambda^{2/3}\Delta T_0,\qquad V_\infty=\lambda^{1/3}V_0.}
$$

For $\lambda=0$ the final temperature is $T_e$. The unchanged-load case $\lambda=1$ has no distinct new temperature layer and is outside the reduction scenario.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
