# Physiological fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Physiological fluid dynamics studies the motion of fluids in biological systems, including blood flow in elastic arteries, flow through deformable vessels, and liquid layers lining airways. Wall compliance couples [pressure](pressure.md) to geometry, so wave propagation and mechanical feedback are as important as [viscosity](dynamic-viscosity.md).

**Table of contents**

- [Lubrication model of a compliant translating plug](#lubrication-model-of-a-compliant-translating-plug)
  - [Force-free pressure drop of an annular lubrication plug](#force-free-pressure-drop-of-an-annular-lubrication-plug)
    - [Small-speed compliant-plug lubrication asymptotics](#small-speed-compliant-plug-lubrication-asymptotics)
- [Annular inviscid-core displacement](#annular-inviscid-core-displacement)
  - [Forced annular displacement equation](#forced-annular-displacement-equation)
    - [Opposite propagation directions in the annular displacement equation](#opposite-propagation-directions-in-the-annular-displacement-equation)
- [Peristaltic pumping](#peristaltic-pumping)
  - [Weak peristaltic pumping of a collapsible tube](#weak-peristaltic-pumping-of-a-collapsible-tube)
- [Collapsible tube flow](#collapsible-tube-flow)
  - [Choking by wall thickness in an elastic tube](#choking-by-wall-thickness-in-an-elastic-tube)
  - [Subcritical tube flow](#subcritical-tube-flow)
  - [Supercritical tube flow](#supercritical-tube-flow)
  - [Elastic jump in a quadratic pressure-area tube](#elastic-jump-in-a-quadratic-pressure-area-tube)
  - [Spatial attraction of a uniform downhill tube flow](#spatial-attraction-of-a-uniform-downhill-tube-flow)
  - [Friction-induced instability of a collapsible-tube flow](#friction-induced-instability-of-a-collapsible-tube-flow)
  - [Pressure-area law of a collapsible tube](#pressure-area-law-of-a-collapsible-tube)
    - [Tube wave speed](#tube-wave-speed)
- [Arterial pressure wave](#arterial-pressure-wave)
  - [Bifurcation reflection of an arterial pressure wave](#bifurcation-reflection-of-an-arterial-pressure-wave)
    - [Pressure-flow phase lag from one arterial reflection](#pressure-flow-phase-lag-from-one-arterial-reflection)
  - [Reflection of an arterial pressure wave](#reflection-of-an-arterial-pressure-wave)
  - [Wave transfer matrix of an arterial segment](#wave-transfer-matrix-of-an-arterial-segment)
    - [Wave transmission through a resistively loaded arterial loop](#wave-transmission-through-a-resistively-loaded-arterial-loop)
  - [Characteristic admittance of an arterial wave](#characteristic-admittance-of-an-arterial-wave)

## Lubrication model of a compliant translating plug

↑ **Parent:** [Physiological fluid dynamics](physiological-fluid-dynamics.md)

For a freely translating compliant body separated from a cylindrical wall by a thin [lubrication](viscous-fluid-flow.md#lubrication-theory) gap $h$, the body frame has wall speed $-U$ and body surface speed zero. The local axial flow is $w=-U(1-y/h)+p_xy(y-h)/(2\mu)$, so its flux per circumference is $-Uh/2-p_xh^3/(12\mu)=-Q$. Rearranging proves the displayed pressure gradient. A linear compliance $p=p_0+\alpha(r_0-r)$ couples this flow to deformation. Specified end pressures and zero net axial body force close the problem.

### Force-free pressure drop of an annular lubrication plug

↑ **Parent:** [Lubrication model of a compliant translating plug](#lubrication-model-of-a-compliant-translating-plug)

The pressure force on a plug-and-film control volume is $\pi a^2\Delta p$. Its opposing wall traction is $2\pi a\mu\int w_y(0)\,dx$, where $w_y(0)=4U/h-6Q/h^2$. Equating them for a freely moving body proves the displayed formula. Writing $s=2Q/U$, $h=sH$ and $x=\sqrt{s/\kappa}X$ converts it into $H(-\widetilde L)-H(\widetilde L)=C\lambda\int[4/(3H)-1/H^2]dX$, with $C=s/a$ and $\lambda=6\mu U/(\alpha\sqrt\kappa s^{5/2})$.

#### Small-speed compliant-plug lubrication asymptotics

↑ **Parent:** [Force-free pressure drop of an annular lubrication plug](#force-free-pressure-drop-of-an-annular-lubrication-plug)

For $H_X+\lambda(H^{-2}-H^{-3})=X$, small $\lambda$ gives $H_0=(b^2+X^2)/2$. In the large-domain limit its inverse-power integrals are $I_1=2\pi/b$, $I_2=2\pi/b^3$ and $I_3=3\pi/b^5$. The force-free condition is $I_2-I_3=C(4I_1/3-I_2)$, or $2b^2-3=C(8b^4/3-2b^2)$. Expanding the root near $b^{-2}=2/3$ proves the displayed minus sign and leading pressure drop. The absolute downstream pressure relative to the elastic reference pressure fixes $s$ and therefore closes the speed-pressure relation.

## Annular inviscid-core displacement

↑ **Parent:** [Physiological fluid dynamics](physiological-fluid-dynamics.md)

For a long, weak, axisymmetric indentation of an annular [fully developed flow](viscous-fluid-flow.md#fully-developed-flow), use $r=R+y$ and scale normal velocity by the inverse longitudinal scale ratio. The leading [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md) give zero longitudinal pressure gradient and $u_0u_{1x}+v_1u_0'=0$. Together with $u_{1x}+(rv_1)_y/r=0$, this yields $\psi_1=A u_0$, hence the displayed displacement fields. Thin [viscous boundary layers](viscous-fluid-flow.md#viscous-boundary-layer) enforce tangential wall conditions separately.

### Forced annular displacement equation

↑ **Parent:** [Annular inviscid-core displacement](#annular-inviscid-core-displacement)

A distinguished annular indentation limit has $\lambda^{-2}=O(\epsilon)$, $\lambda St=O(\epsilon)$ and $Re\gg\lambda\epsilon^{-3}$. Define $\beta=\lambda St/\epsilon$, $\sigma=(\lambda^2\epsilon)^{-1}\int_0^1u_0^2/(R+y)\,dy$, $\alpha_1=\gamma_0/R+\gamma_1/(R+1)$ and $\alpha_2=\gamma_0^2/R^2-\gamma_1^2/(R+1)^2$. Radial inertia supplies the pressure difference $\sigma A_{xx}$ between the walls. The axial momentum limits and the moving-wall condition supply its derivative, giving the displayed forced [KdV equation](integrable-systems.md#korteweg-de-vries-equation). This reduction assumes the [viscous boundary layers](viscous-fluid-flow.md#viscous-boundary-layer) remain thin and their displaced flux is smaller than $O(\epsilon^2)$.

#### Opposite propagation directions in the annular displacement equation

↑ **Parent:** [Forced annular displacement equation](#forced-annular-displacement-equation)

With no forcing, the linear [dispersion relation](dispersion-relation.md) has positive [phase velocity](dispersion-relation.md#phase-velocity) $\sigma k^2/(\beta\alpha_1)$ and [group velocity](dispersion-relation.md#group-velocity) three times this. A decaying permanent wave with $\xi=x+ct$ instead obeys $\sigma(A')^2=A^2(\beta\alpha_1c+\alpha_2A/3)$. For positive coefficients a nonzero homoclinic wave requires $c>0$ and is negative, travelling upstream. Its inverse width is $k_s=\frac12\sqrt{\beta\alpha_1c/\sigma}$. The opposite directions reflect the nonlinear amplitude-dependent propagation speed.

## Peristaltic pumping

↑ **Parent:** [Physiological fluid dynamics](physiological-fluid-dynamics.md)

[Peristaltic pumping](#peristaltic-pumping) transports fluid by a travelling deformation or travelling external [pressure](pressure.md) acting on a tube. With wave coordinate $X=x-ct$, [mass conservation](continuum-mechanics.md#mass-conservation) makes the relative flux $Q=\alpha(u-c)$ constant. The laboratory flux is $\alpha u=c\alpha+Q$, so a negative relative flux does not rule out forward mean pumping.

### Weak peristaltic pumping of a collapsible tube

↑ **Parent:** [Peristaltic pumping](#peristaltic-pumping)

For negligible inertia, periodic forcing $p_e=\epsilon P_e\sin kX$, resistance $R\propto\alpha^{-n}$ and prescribed mean area $\alpha_0$, write $Q=-c\alpha_0+\epsilon^2Q_2+\cdots$. First-order area obeys $\widetilde P'_0\alpha_1'+R_0c\alpha_1/\alpha_0=-kP_e\cos kX$. Its mean square is $P_e^2/[2(\widetilde P_0'^2+(R_0c/(k\alpha_0))^2)]$. Averaging the second-order friction balance gives $Q_2=c(n+1)\langle\alpha_1^2\rangle/\alpha_0$, proving the displayed forward pumping rate. Periodicity entails zero mean [pressure](pressure.md) drop; the mean-area convention fixes the expansion's otherwise free constant.

## Collapsible tube flow

↑ **Parent:** [Physiological fluid dynamics](physiological-fluid-dynamics.md)

A one-dimensional collapsible tube model couples area $\alpha$, mean axial [velocity](classical-mechanics.md#velocity) $u$ and internal [pressure](pressure.md) $p$: $\alpha_t+(\alpha u)_x=0$ and $u_t+uu_x=-p_x-R(\alpha)u$. A wall relation specifies internal minus external [pressure](pressure.md) as a function of area. Decreasing area generally increases the friction coefficient $R$, while positive wall stiffness gives real small-amplitude [wave speed](wave-equation.md#wave-speed).

### Choking by wall thickness in an elastic tube

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

For steady uniform-density inviscid flow with pressure law $p=p_0+k(r-R)$ and a prescribed thickness $h$, mass conservation and the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) give $h/R=1-s^{-1/2}+\lambda(1-s^2)/4$, where $s=u/V$ and $\lambda=2\rho V^2/(kR)$. The function has a unique maximum at $s=\lambda^{-2/5}$, producing the displayed choking bound. Below it there are two positive roots; continuity from the upstream state selects the lower-speed root for $\lambda<1$ and higher-speed root for $\lambda>1$. At $\lambda=1$, the maximum is zero and any positive prescribed thickness is incompatible with this model.

### Subcritical tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

A positive [collapsible tube flow](#collapsible-tube-flow) is subcritical when its [characteristic speeds](transport-equation.md#characteristic-speed) $u+c$ and $u-c$ have opposite signs. A downstream boundary can then send information upstream. For a quadratic pressure-area law and fixed dimensionless flux $q$, this corresponds to $A/A_0>\sqrt q$.

### Supercritical tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

A positive [collapsible tube flow](#collapsible-tube-flow) is supercritical when both [characteristic speeds](transport-equation.md#characteristic-speed) $u\pm c$ are positive relative to the wall. Information then propagates downstream on both branches. For a quadratic pressure-area law and fixed dimensionless flux $q$, the condition is $A/A_0<\sqrt q$.

### Elastic jump in a quadratic pressure-area tube

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

An elastic jump is a short transition from a fast, narrow supercritical [collapsible tube flow](#collapsible-tube-flow) to a slower, wider subcritical flow. Neglecting body force and distributed friction across the jump conserves flux and the momentum flux shown above. Distinct upstream and downstream areas therefore obey $\alpha_2^3+\alpha_1\alpha_2^2+\alpha_1^2\alpha_2=3q^2/\alpha_1$. The flux function has its unique minimum at $\alpha=\sqrt q$, so an upstream state below this value has one conjugate state above it. The jump dissipates mechanical energy; it does not conserve a Bernoulli constant.

### Spatial attraction of a uniform downhill tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

For $p=P_0+\rho c_0^2\alpha^2/2$ and constant flux $c_0A_0q$, a downhill [collapsible tube flow](#collapsible-tube-flow) obeys the displayed steady equation. Uniform area satisfies $qR(\alpha_1)=\beta$. Since $R'<0$, linearizing about this root gives downstream exponential decay precisely when $\alpha_1^2<q$. This is spatial stability of a steady inlet-value problem, not a guarantee of temporal stability of the driven flow. The [wave speed](wave-equation.md#wave-speed) is $c_0\alpha$, so the stable spatial branch is supercritical.

### Friction-induced instability of a collapsible-tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

Let $R(\alpha)\propto\alpha^{-n}$, with $n>0$, and use disturbances $e^{i(kx-\omega t)}$ about uniform [velocity](classical-mechanics.md#velocity) $U$. The intrinsic [frequency](wave.md#frequency) is $\nu=\omega-kU$. Linearized [mass conservation](continuum-mechanics.md#mass-conservation) and the decrease in friction as area grows give the displayed [dispersion relation](dispersion-relation.md). For nonzero $k$ and positive flow, one branch grows exactly when $nU>c_0$. At $nU=c_0$, one branch is neutral, $\nu=kc_0$, while the other remains damped, $\nu=-kc_0-iR_0$. The maintained external-[pressure gradient](fluid-mechanics.md#pressure-gradient) supplies the energy; positive friction alone does not imply linear stability of a driven flow.

### Pressure-area law of a collapsible tube

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

The [pressure-area law of a collapsible tube](#pressure-area-law-of-a-collapsible-tube) describes transverse mechanical equilibrium of a deformable tube wall. On a stable branch $\widetilde P'(\alpha)>0$. Linearizing mass and momentum conservation about a stationary uniform tube gives the displayed [wave speed](wave-equation.md#wave-speed). External [pressure](pressure.md) is prescribed separately and is not part of the elastic wall stiffness.

#### Tube wave speed

↑ **Parent:** [Pressure-area law of a collapsible tube](#pressure-area-law-of-a-collapsible-tube)

Linearizing area conservation and the axial momentum equation of a [collapsible tube flow](#collapsible-tube-flow) gives waves travelling relative to the fluid at speeds $\pm c$, where the displayed relation uses the area derivative at fixed external pressure. For $p=P_0+\rho c_0^2(A/A_0)^2/2$, it gives $c=c_0A/A_0$.

## Arterial pressure wave

↑ **Parent:** [Physiological fluid dynamics](physiological-fluid-dynamics.md)

A small [pressure](pressure.md) disturbance in an elastic artery propagates through the coupled inertia of blood and compliance of the wall. If $\mathcal A$ is the undisturbed area, $\rho$ the [mass density](fluid-mechanics.md#density) and $c$ the [wave speed](wave-equation.md#wave-speed), the linearized equations give $c^2=\mathcal A/\rho\,dp/d\mathcal A$. A travelling [pressure](pressure.md) amplitude $p_+$ carries flow amplitude $\mathcal A p_+/(\rho c)$; the oppositely travelling wave has the opposite flow sign.

### Bifurcation reflection of an arterial pressure wave

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

At a lossless vascular junction, [pressure](pressure.md) continuity and [volumetric flow rate](fluid-mechanics.md#volumetric-flow-rate) balance give $1+r=t$ and $Y_1(1-r)=Y_dt$, where $Y_d$ is the sum of daughter [characteristic admittances of an arterial wave](#characteristic-admittance-of-an-arterial-wave). Eliminating transmission amplitude $t$ gives the displayed [reflection coefficient](partial-differential-equation.md#reflection-coefficient). A decrease in total area yields positive reflection if parent and daughter wave speeds are equal; differing stiffnesses require comparison of the admittances rather than areas alone.

#### Pressure-flow phase lag from one arterial reflection

↑ **Parent:** [Bifurcation reflection of an arterial pressure wave](#bifurcation-reflection-of-an-arterial-pressure-wave)

For incident and reflected harmonic [arterial pressure waves](#arterial-pressure-wave) with real $0<r<1$, the local [pressure](pressure.md) and flow phasors are proportional to $1+re^{-i\vartheta}$ and $1-re^{-i\vartheta}$. Their maximum-time difference is the displayed phase lag, on the branch $0<\vartheta<\pi$. Here $\vartheta=2\omega d/c$ is the round-trip phase to the reflector. Its derivative has the sign of $\cos\vartheta$. Raising the [wave speed](wave-equation.md#wave-speed) reduces the lag when $0<\vartheta<\pi/2$, but increases it when $\pi/2<\vartheta<\pi$. This conditional harmonic model does not establish an age trend for arbitrary vascular geometry or measurement stations beyond the sole reflector.

### Reflection of an arterial pressure wave

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

A [hydraulic resistance](fluid-mechanics.md#hydraulic-resistance) $R$ imposes $q=p/R$. Combining this with forward and backward [arterial pressure waves](#arterial-pressure-wave), $p=p_++p_-$ and $q=Y(p_+-p_-)$, gives the displayed [reflection coefficient](partial-differential-equation.md#reflection-coefficient). A matched load $RY=1$ has no reflected [pressure](pressure.md) wave, while a closed end has [reflection coefficient](partial-differential-equation.md#reflection-coefficient) one. At a network junction the combined downstream input admittance replaces $1/R$.

### Wave transfer matrix of an arterial segment

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

For time dependence $e^{i\omega t}$ and a segment of length $\ell$, let $\beta=\omega\ell/c$. Adding the forward and backward [arterial pressure waves](#arterial-pressure-wave) gives the displayed upstream-to-downstream matrix. The flow orientation is downstream at both ends. At a junction, [pressure](pressure.md) is continuous and incoming [volumetric flow rates](fluid-mechanics.md#volumetric-flow-rate) balance outgoing ones.

#### Wave transmission through a resistively loaded arterial loop

↑ **Parent:** [Wave transfer matrix of an arterial segment](#wave-transfer-matrix-of-an-arterial-segment)

Consider two identical two-segment paths from an inlet to a distal junction, with equal resistive beds at the two intermediate junctions and the distal junction. The segment transfer matrix and junction flow balances determine all [pressures](pressure.md). If one inlet branch is removed and the beds are weakly loading the waves, the remaining segments form a three-segment chain with an effectively closed far end. The altered reflection pattern can raise peripheral oscillatory flow amplitudes even though a branch was lost; the incident wave amplitude, rather than total inlet [pressure](pressure.md) or flow, is the prescribed forcing.

### Characteristic admittance of an arterial wave

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

The [characteristic admittance of an arterial wave](#characteristic-admittance-of-an-arterial-wave) relates the [volumetric flow rate](fluid-mechanics.md#volumetric-flow-rate) of a travelling [arterial pressure wave](#arterial-pressure-wave) to its [pressure](pressure.md). For forward and backward amplitudes, $p=p_++p_-$ and $q=Y(p_+-p_-)$. It is the reciprocal of characteristic [pressure](pressure.md)-to-flow impedance, and should not be confused with the reciprocal [hydraulic resistance](fluid-mechanics.md#hydraulic-resistance) of a steadily resistive segment.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)
