# Draining tank with constant cross-sectional area

↑ **Parent:** [Torricelli's law](torricelli-s-law.md)

Take a reservoir with constant horizontal cross-sectional [area](surface-area.md) $A$, one small [orifice](orifice.md) of [area](surface-area.md) $a$, no inflow, and constant stipulated [discharge coefficient](discharge-coefficient.md) $C_d>0$. Let the initial head be $H>0$. For constant [mass density](density.md) $\rho$, the stored [mass](mass.md) above the outlet level is $\rho Ah$ and outgoing [mass flow rate](mass-flow-rate.md) is $\rho Q$. [Mass conservation](mass-conservation.md) cancels $\rho$ and gives the [initial value problem](initial-value-problem.md)

$$
A\frac{dh}{dt}=-Q,
\qquad \frac{dh}{dt}=-k\sqrt h,
\qquad h(0)=H,
\qquad k=\frac{C_da}{A}\sqrt{2g}.
$$

The downward [speed](speed.md) of the [free surface](free-surface.md) is $Q/A$, smaller than the ideal jet [speed](speed.md) by the factor $C_da/A$. Thus a small opening relative to the reservoir supports the negligible-surface-[velocity](velocity.md) assumption.

For $h>0$, [separation of variables](separation-of-variables.md) or the [chain rule](chain-rule.md) gives $d\sqrt h/dt=-k/2$. Integrating yields

$$
T=\frac{2\sqrt H}{k}=\frac{A}{C_da}\sqrt{\frac{2H}{g}},
\qquad
h(t)=\begin{cases}H(1-t/T)^2,&0\le t\le T,\\0,&t\ge T,\end{cases}
$$



$$
Q(t)=\begin{cases}Q_0(1-t/T),&0\le t\le T,\\0,&t\ge T,\end{cases}
\qquad Q_0=C_da\sqrt{2gH}.
$$

The model reaches zero head in finite time even though [volumetric flow rate](volumetric-flow-rate.md) tends to zero. Extending the squared expression beyond $T$ would make head grow again and violate the original [ordinary differential equation](ordinary-differential-equation.md). The zero-head continuation enforces no further outflow. For an elevated side opening, zero head means the surface has reached that opening, leaving [fluid](fluid.md) below it; $T$ is not the time to remove every drop from such a tank.

For an original synthetic example, stipulate

$$
A=0.100\ \mathrm{m^2},\quad a=1.00\times10^{-4}\ \mathrm{m^2},\quad
C_d=0.620,\quad H=0.250\ \mathrm m,\quad g=9.81\ \mathrm{m\,s^{-2}}.
$$

The initial [volume](volume.md) above outlet level is $AH=0.0250\ \mathrm{m^3}=25.0\ \mathrm L$. The initial ideal jet [speed](speed.md) is $2.215\ \mathrm{m\,s^{-1}}$, the initial [volumetric flow rate](volumetric-flow-rate.md) is $Q_0=0.1373\ \mathrm{L\,s^{-1}}$, and the predicted zero-head time is $T=364.1\ \mathrm s$. These are consequences of stipulated parameters, not experimental measurements. At $t=T/2=182.1\ \mathrm s$, head is $H/4=0.0625\ \mathrm m$, stored [volume](volume.md) is $6.25\ \mathrm L$, and [volumetric flow rate](volumetric-flow-rate.md) is $Q_0/2=0.06866\ \mathrm{L\,s^{-1}}$. Half the initial [volume](volume.md) has already left at $t=T(1-1/\sqrt2)=106.7\ \mathrm s$.

<a id="image-constant-area-drainage-quadratic-head-and-linearly-declining-discharge"></a>
![](torricelli-draining-tank-height-and-flow.png)

**[Figure 10](#image-constant-area-drainage-quadratic-head-and-linearly-declining-discharge). Constant-area drainage: quadratic head and linearly declining discharge**. Original synthetic trajectories for the stipulated [draining tank with constant cross-sectional area](draining-tank-with-constant-cross-sectional-area.md), with $A=0.100\ \mathrm{m^2}$, $a=10^{-4}\ \mathrm{m^2}$, $C_d=0.620$, $H=0.250\ \mathrm m$ and $g=9.81\ \mathrm{m\,s^{-2}}$. The model remains at zero head and zero [volumetric flow rate](volumetric-flow-rate.md) after $T$. The shaded [area](surface-area.md) under the flow curve represents $25.0\ \mathrm L$.

An independent [mass conservation](mass-conservation.md) check integrates the outgoing [volumetric flow rate](volumetric-flow-rate.md):

$$
\int_0^tQ(s)\,ds
=Q_0\left(t-\frac{t^2}{2T}\right)
=A[H-h(t)]\quad(0\le t\le T),
\qquad \int_0^TQ(s)\,ds=\frac{Q_0T}{2}=AH.
$$

Multiply both sides by [mass density](density.md) to obtain discharged [mass](mass.md). A [dimensional analysis](dimensional-analysis.md) check gives $[k]=\mathrm{m^{1/2}\,s^{-1}}$, $[Q]=\mathrm{m^3\,s^{-1}}$ and $[T]=\mathrm s$. The triangular [area](surface-area.md) under $Q(t)$ explains why the initial-rate estimate $AH/Q_0$ is only half the actual model time. Doubling $A$ doubles $T$; doubling $a$ or $C_d$ halves $T$, within the same assumptions.

This finite-time result is an idealized prediction. The constant $C_d$ and [quasi-steady approximation](quasi-steady-approximation.md) need not survive very small head or the initial startup. Appreciable [viscosity](dynamic-viscosity-split.md) in a narrow outlet tube requires a different [pressure](pressure-split.md) balance, as in [Poiseuille flow](hagen-poiseuille-equation.md); appreciable [surface tension](surface-tension-split.md) can prevent zero head altogether.

## ↑ Ancestors (5)

1. [Torricelli's law](torricelli-s-law.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Discharge measurement in a draining tank](discharge-measurement-in-a-draining-tank.md)
- [Draining tank with constant cross-sectional area](draining-tank-with-constant-cross-sectional-area.md)
